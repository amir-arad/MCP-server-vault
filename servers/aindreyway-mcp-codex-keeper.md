---
type: server
repo_url: https://github.com/aindreyway/mcp-codex-keeper
name: Codex Keeper MCP Server
owner: aindreyway
stars: 41
last_updated: 2025-02-20
status: active
official: false
verified: false
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/knowledge-base",
    "purpose/documentation",
    "purpose/best-practices",
    "category/ai",
    "purpose/curation",
  ]
---

# Codex Keeper MCP Server

#status/active #category/knowledge-base #purpose/documentation #purpose/best-practices #category/ai #purpose/curation

## Description

Serves as a guardian of development knowledge, providing AI assistants with curated access to latest documentation and best practices. This server maintains and organizes development knowledge for easy access and reference.

## Features

- Knowledge curation
- Documentation access
- Best practices management
- Version tracking
- Content organization
- Search capabilities
- Update notifications
- Access control
- Content validation
- Integration support

## Installation

```bash
npm install @aindreyway/mcp-codex-keeper
```

## Usage

```javascript
{
  "mcpServers": {
    "codex-keeper": {
      "command": "npx",
      "args": ["@aindreyway/mcp-codex-keeper"],
      "env": {
        "KNOWLEDGE_BASE": "./knowledge",
        "UPDATE_INTERVAL": "86400",
        "SOURCES": "github,stackoverflow,docs",
        "MAX_AGE": "30d",
        "VALIDATION_ENABLED": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Knowledge base system
- Search engine
- Content validator
- Update manager
- Integration APIs

## Related Servers

- davidvc/code-knowledge-mcptool
- nahmanmate/code-research-mcp-server
- modelcontextprotocol-docs-server
