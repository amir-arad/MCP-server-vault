# Alignment Plan: Templates and Processing Instructions

## Overview

This plan outlines the necessary changes to align the templates in the `templates/` folder with the processing instructions in `MCP-Server-Processing-Prompt-3.md`. The goal is to ensure compatibility and produce the desired results when processing MCP server entries.

## Current Issues

1. **Field Naming Inconsistencies**

   - Instructions use "title", template uses "name"
   - Instructions pass single "sources" string, template expects array
   - Instructions use "description" field not directly mapped in template

2. **Missing Required Template Fields**

   - Template requires fields not provided in instructions:
     - stars
     - last_updated
     - verified

3. **Content Structure Requirements**

   - Templates expect structured content sections not addressed in instructions

4. **Source Template Utilization**
   - Source template exists but is not referenced in processing instructions

## Proposed Solutions

### 1. Update Server Template

**Option A: Modify Template to Match Instructions**

````markdown
---
repo_url: {{url}}
owner: {{owner}}
name: {{title}}
description: {{description}}
stars: 0
last_updated: {{current_date}}
status: {{status}}
verified: false
sources:
  - {{sources}}
tags:
  {{#each tags}}
  - {{this}}
  {{/each}}
---

# {{title}}

## Description

{{description}}

## Features

- Feature 1
- Feature 2
- Feature 3

## Installation

```bash
# Installation commands
```
````

## Usage

```javascript
// Usage example
```

## Dependencies

- Dependency 1
- Dependency 2

## Related Servers

- [Related Server 1](https://github.com/owner/related-repo-1)
- [Related Server 2](https://github.com/owner/related-repo-2)

````

**Option B: Update Processing Instructions**

```markdown
execute_template(
  name: "templates/server.md",
  createFile: true,
  targetPath: "servers/owner-repo.md",
  arguments: {
    "repo_url": "https://github.com/owner/repo",
    "owner": "owner",
    "name": "Human-readable title",
    "stars": "0",
    "last_updated": "YYYY-MM-DD", // Use current date function
    "status": "active",
    "verified": "false",
    "sources": ["inbox"],
    "description": "Description from inbox",
    "tags": ["tag1", "tag2", "tag3"]
  }
)
````

### 2. Update Tag Template

**Option A: Simplify Tag Template**

```markdown
---
type: tag
id: { { tag } }
name: { { tag_name } }
description: { { description } }
servers_count: 0
related_tags: []
---

# {{tag_name}}

{{description}}

## Description

{{description}}

## Servers with this tag

<!-- This section can be auto-generated through queries -->

## Related Tags

<!-- Links to related tag records -->
```

**Option B: Enhance Processing Instructions**

```markdown
execute_template(
name: "templates/tag.md",
createFile: true,
targetPath: "tags/category/tag-name.md",
arguments: {
"type": "tag",
"id": "category/tag-name",
"name": "Human-Readable Tag Name", // Derived from tag-name
"description": "Brief description of tag purpose",
"servers_count": "0",
"related_tags": "[]"
}
)
```

### 3. Incorporate Source Template

Add processing instructions for source template:

```markdown
execute_template(
name: "templates/source.md",
createFile: true,
targetPath: "tags/source/source-name.md",
arguments: {
"type": "tag",
"id": "source/source-id",
"name": "Source Name",
"url": "https://example.com/source",
"last_checked": "YYYY-MM-DD", // Use current date function
"servers_count": "0",
"curator": "Curator name"
}
)
```

## Implementation Plan

### Phase 1: Template Alignment

1. **Choose Approach**:

   - Determine whether to modify templates or instructions (recommend Option B for both)
   - Consider backward compatibility with existing records

2. **Update Templates**:
   - Make necessary changes to templates based on chosen approach
   - Test with sample data to ensure proper rendering

### Phase 2: Processing Instructions Update

1. **Revise MCP-Server-Processing-Prompt-3.md**:

   - Update execute_template calls with correct parameter mapping
   - Add helper functions for:
     - Current date generation
     - Tag name formatting
     - Source array handling

2. **Add Source Template Processing**:
   - Include instructions for source template usage
   - Define when and how source records should be created/updated

### Phase 3: Content Generation

1. **Define Content Generation Rules**:

   - Create guidelines for generating structured content sections
   - Implement placeholder text that can be replaced later

2. **Metadata Management**:
   - Develop process for updating servers_count
   - Establish related_tags management approach

### Phase 4: Testing and Validation

1. **Create Test Cases**:

   - Sample GitHub URLs
   - Various tag categories
   - Different source types

2. **Validate Output**:
   - Ensure generated files match expected format
   - Verify all required fields are populated
   - Check content structure integrity

## Recommended Approach

Based on the analysis, the recommended approach is:

1. **Update Processing Instructions** rather than modifying templates

   - This preserves existing template structure
   - Allows for backward compatibility
   - Provides more flexibility in parameter mapping

2. **Add Helper Functions** for dynamic content generation

   - Current date formatting
   - Tag name humanization
   - Array handling for sources and tags

3. **Implement Source Template Processing** to complete the workflow

   - Track sources properly
   - Enable source-based queries

4. **Create Content Generation Guidelines** for structured sections
   - Define what should be included in each section
   - Provide placeholder text that can be refined later
