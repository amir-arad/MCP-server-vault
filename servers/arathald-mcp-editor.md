---
type: server
repo_url: https://github.com/arathald/mcp-editor
name: Editor MCP Server
owner: arathald
stars: 3
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_010.md"]
tags:
  [
    "status/active",
    "category/development",
    "tech/typescript",
    "integration/anthropic",
    "purpose/file-editing",
    "purpose/safety",
  ]
---

# Editor MCP Server

#status/active #category/development #tech/typescript #integration/anthropic #purpose/file-editing #purpose/safety

## Description

A TypeScript MCP server port of Anthropic's filesystem editing tools, allowing file manipulation via client-approved operations without automated writes to prevent system harm.

## Features

- Safe file manipulation
- Client approval system
- Operation validation
- Write prevention safeguards
- File system monitoring
- Change tracking
- Operation logging
- Rollback capabilities
- Access control
- Error handling

## Installation

```bash
npm install @arathald/mcp-editor
```

## Usage

```javascript
{
  "mcpServers": {
    "editor": {
      "command": "npx",
      "args": ["@arathald/mcp-editor"],
      "env": {
        "ALLOWED_PATHS": "./src,./config",
        "REQUIRE_APPROVAL": "true",
        "LOG_LEVEL": "info"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- TypeScript
- File system access
- Logging system
- Client approval mechanism

## Related Servers

- None currently listed
