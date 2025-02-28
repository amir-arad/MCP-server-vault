---
type: server
repo_url: https://github.com/bradfair/mcp-cline-personas
name: Cline Personas MCP Server
owner: bradfair
stars: 16
last_updated: 2025-02-18
status: active
official: false
verified: false
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/configuration",
    "purpose/persona-management",
    "tech/cline",
    "purpose/templates",
    "tech/rules",
  ]
---

# Cline Personas MCP Server

#status/active #category/configuration #purpose/persona-management #tech/cline #purpose/templates #tech/rules

## Description

An MCP server for managing and activating persona templates and components by writing to .clinerules files, supporting version tracking and file-based storage.

## Features

- Persona template management
- Component activation
- Rule file handling
- Version tracking
- Template storage
- Component organization
- Rule validation
- Template inheritance
- Change tracking
- Backup management

## Installation

```bash
npm install @bradfair/mcp-cline-personas
```

## Usage

```javascript
{
  "mcpServers": {
    "cline-personas": {
      "command": "npx",
      "args": ["@bradfair/mcp-cline-personas"],
      "env": {
        "RULES_PATH": "./.clinerules",
        "TEMPLATES_PATH": "./templates",
        "BACKUP_ENABLED": "true",
        "VERSION_CONTROL": "true",
        "AUTO_RELOAD": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Cline installation
- File system access
- Version control system
- Template engine
- Rule parser

## Related Servers

- modelcontextprotocol-cline-server
- maheshdoiphode/mcp-cline-project-content-server
- davidvc/code-knowledge-mcptool
