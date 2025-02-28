---
type: server
repo_url: https://github.com/Cleversoft-IT/drupal-modules-mcp
name: Drupal Modules MCP Server
owner: Cleversoft-IT
stars: 0
last_updated: 2025-02-15
status: active
official: false
verified: false
sources: ["inbox/batch_010.md"]
tags: ["status/active", "category/cms", "integration/drupal", "tech/typescript", "purpose/note-management", "purpose/module-management"]
---

# Drupal Modules MCP Server

#status/active #category/cms #integration/drupal #tech/typescript #purpose/note-management #purpose/module-management

## Description

This TypeScript-based MCP server implements a simple notes system, allowing the creation, listing, and summarization of text notes using MCP concepts with note:// URIs and metadata.

## Features

- Note creation and management
- Note listing and organization
- Text summarization
- Metadata handling
- URI-based note access
- Note search capabilities
- Note categorization
- Content formatting
- Note export options
- Version tracking

## Installation

```bash
npm install @cleversoft-it/drupal-modules-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "drupal-modules": {
      "command": "npx",
      "args": ["@cleversoft-it/drupal-modules-mcp"],
      "env": {
        "NOTES_DIR": "./notes",
        "DRUPAL_ROOT": "/var/www/html",
        "METADATA_FORMAT": "json"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- TypeScript
- Drupal >= 9.0
- File system access
- JSON processing libraries
- Text processing tools

## Related Servers

- [Drupal MCP Server](https://github.com/Omedia/mcp-server-drupal) - Main Drupal integration