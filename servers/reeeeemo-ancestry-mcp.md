---
type: server
repo_url: https://github.com/reeeeemo/ancestry-mcp
name: Ancestry MCP Server
owner: reeeeemo
stars: 9
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_002.md"]
tags:
  [
    "status/active",
    "category/genealogy",
    "purpose/data-analysis",
    "tech/gedcom",
  ]
---

# Ancestry MCP Server

#status/active #category/genealogy #purpose/data-analysis #tech/gedcom

## Description

Allows the AI to read .ged files and genetic data.

## Features

- GEDCOM file parsing
- Genetic data analysis
- Family tree visualization
- Relationship mapping
- Data validation
- Format conversion
- Ancestry tracking
- Metadata extraction

## Installation

```bash
npm install @reeeeemo/ancestry-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "ancestry": {
      "command": "npx",
      "args": ["@reeeeemo/ancestry-mcp"],
      "env": {
        "GEDCOM_PATH": "./family-tree.ged",
        "GENETIC_DATA_PATH": "./dna-data",
        "MAX_GENERATIONS": "10",
        "INCLUDE_MEDIA": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- GEDCOM parser
- Genetic data analysis tools
- File system access

## Related Servers

- None currently listed
