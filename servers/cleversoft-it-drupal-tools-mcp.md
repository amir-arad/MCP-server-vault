---
type: server
repo_url: https://github.com/Cleversoft-IT/drupal-tools-mcp
name: Drupal Tools MCP Server
owner: Cleversoft-IT
stars: 0
last_updated: 2025-02-07
status: active
official: false
verified: false
sources: ["inbox/batch_010.md"]
tags: ["status/active", "category/cms", "integration/drupal", "tech/typescript", "purpose/note-management", "purpose/tool-management"]
---

# Drupal Tools MCP Server

#status/active #category/cms #integration/drupal #tech/typescript #purpose/note-management #purpose/tool-management

## Description

This TypeScript-based MCP server allows users to manage and interact with a note system through Model Context Protocol, enabling note creation and summarization with URIs and metadata.

## Features

- Note system management
- URI-based interactions
- Metadata management
- Note creation tools
- Content summarization
- Note organization
- Search functionality
- Export capabilities
- Version control
- Backup management

## Installation

```bash
npm install @cleversoft-it/drupal-tools-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "drupal-tools": {
      "command": "npx",
      "args": ["@cleversoft-it/drupal-tools-mcp"],
      "env": {
        "STORAGE_PATH": "./storage",
        "DRUPAL_ROOT": "/var/www/html",
        "BACKUP_INTERVAL": "86400"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- TypeScript
- Drupal >= 9.0
- Storage system
- URI handling libraries
- Metadata processing tools

## Related Servers

- [Drupal MCP Server](https://github.com/Omedia/mcp-server-drupal) - Main Drupal integration
- [Drupal Modules MCP](https://github.com/Cleversoft-IT/drupal-modules-mcp) - Module management system