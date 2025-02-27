Templater Alignment Plan

## Overview

This plan outlines the changes needed to adapt our templates to work with the Templater plugin's syntax and functionality.

# Data Structures

Server Creation Data

```js
const serverData = {
  url: "https://github.com/owner/repo",
  owner: "owner",
  title: "Human-readable title",
  description: "Description from inbox",
  status: "active",
  official: false,
  sources: ["inbox"],
  features: [],
  installation: "npm install",
  usage: "// Example code",
  dependencies: [],
  related: [],
};
```

Tag Creation Data

```js
const tagData = {
  id: "category/tag-name",
  name: "Human-Readable Tag Name",
  description: "Brief description",
  long_description: "More detailed description",
  servers: [],
  related_tags: [],
};
```

Source Creation Data

```js
const sourceData = {
  id: "source/source-id",
  name: "Source Name",
  url: "https://example.com/source",
  curator: "Curator name",
  description: "Source description",
  servers: [],
  unique_servers: [],
};
```

Implementation Steps
Update Templates

Convert all templates to use Templater's <% %> syntax
Implement proper frontmatter structure
Add dynamic content rendering
Modify Processing Script

Update data preparation for frontmatter
Ensure proper data types for arrays and objects
Add validation for required fields
Testing

Test template rendering with sample data
Verify array handling
Check date formatting
Batch Processing Updates

Adapt batch processing for new format
Update status tracking
Implement error handling
Documentation

Update processing instructions
Document frontmatter requirements
Add examples for common operations
Key Features
Uses Templater's <% %> syntax for dynamic content
Leverages tp.frontmatter for data access
Utilizes tp.date for timestamp generation
Maintains proper markdown structure
Supports array handling through JavaScript methods

```

```

```

```

```

```
