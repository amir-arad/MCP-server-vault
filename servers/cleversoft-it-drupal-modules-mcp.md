---
type: server
repo_url: https://github.com/Cleversoft-IT/drupal-modules-mcp
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
    "purpose/module-management",
  ]
---

# Drupal Modules MCP Server

#status/active #category/cms #integration/drupal #tech/typescript #purpose/note-management #purpose/module-management

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

- Node.js 16 or higher

## Related Servers

- Drupal MCP Server - Main Drupal integration
