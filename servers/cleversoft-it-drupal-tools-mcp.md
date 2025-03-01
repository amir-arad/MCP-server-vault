---
type: server
repo_url: https://github.com/Cleversoft-IT/drupal-tools-mcp
name: Drupal Modules MCP Server
owner: Cleversoft-IT
stars: 0
last_updated: 2025-03-01
status: active
official: false
verified: true
sources: ["inbox/batch_010.md"]
tags:
  [
    "status/active",
    "category/cms",
    "integration/drupal",
    "tech/typescript",
    "purpose/note-management",
    "purpose/tool-management",
  ]
---

# Drupal Tools MCP Server

#status/active #category/cms #integration/drupal #tech/typescript #purpose/note-management #purpose/tool-management

## Description

Model Context Protocol (MCP) servers for Drupal development. Includes tools for querying Drupal.org module and interacting with Drush commands. Seamlessly integrates with Cline and other MCP-compatible clients to enhance Drupal development workflows.

## Features

- Drupal module information
- Querying Drupal.org module
- Interacting with Drush commands

## Installation

```bash
npm install
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

- Node.js 16 or higher

## Related Servers

- Drupal MCP Server - Main Drupal integration
