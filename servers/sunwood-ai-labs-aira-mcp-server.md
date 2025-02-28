---
type: server
repo_url: https://github.com/Sunwood-ai-labs/aira-mcp-server
name: Aira MCP Server
owner: Sunwood-ai-labs
stars: 1
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_001.md"]
tags:
  [
    "status/active",
    "category/version-control",
    "integration/git",
    "purpose/commit-messages",
  ]
---

# Aira MCP Server

#status/active #category/version-control #integration/git #purpose/commit-messages

## Description

A Model Context Protocol server for creating commit messages from git staged files.

## Features

- Git staged file analysis
- Automated commit message generation
- Conventional commits support
- Multi-language support
- Change type detection
- Scope identification
- Breaking change detection
- Message formatting

## Installation

```bash
npm install @sunwood-ai-labs/aira-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "aira": {
      "command": "npx",
      "args": ["@sunwood-ai-labs/aira-mcp"],
      "env": {
        "GIT_PATH": ".git",
        "COMMIT_STYLE": "conventional",
        "MAX_MESSAGE_LENGTH": "72",
        "INCLUDE_SCOPE": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Git >= 2.0
- Local git repository

## Related Servers

- None currently listed
