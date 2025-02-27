---
type: server
repo_url: https://github.com/aborroy/alfresco-mcp-poc
name: Alfresco POC MCP Server
owner: aborroy
stars: 2
last_updated: 2025-02-11
status: active
official: false
verified: false
sources: ["inbox/batch_001.md"]
tags: ["status/active", "category/content-management", "integration/alfresco", "purpose/document-processing"]
---

# Alfresco POC MCP Server

#status/active #category/content-management #integration/alfresco #purpose/document-processing

## Description

Integrates Alfresco's content management, enabling intelligent document processing and automated metadata extraction.

## Features

- Alfresco integration
- Document processing
- Metadata extraction
- Content management
- Automated tagging
- Document classification
- Version control
- Permission management

## Installation

```bash
npm install @aborroy/alfresco-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "alfresco": {
      "command": "npx",
      "args": ["@aborroy/alfresco-mcp"],
      "env": {
        "ALFRESCO_URL": "http://your-alfresco-instance",
        "ALFRESCO_USERNAME": "admin",
        "ALFRESCO_PASSWORD": "admin",
        "PROCESS_TIMEOUT": "300"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Alfresco instance
- Authentication credentials
- Content Services API access

## Related Servers

- None currently listed