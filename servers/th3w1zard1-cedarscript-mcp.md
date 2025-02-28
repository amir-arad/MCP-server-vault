---
type: server
repo_url: https://github.com/th3w1zard1/cedarscript-mcp
name: CEDARScript MCP Server
owner: th3w1zard1
stars: 7
last_updated: 2025-01-27
status: active
official: false
verified: false
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/development",
    "tech/sql",
    "purpose/code-manipulation",
    "category/language",
  ]
---

# CEDARScript MCP Server

#status/active #category/development #tech/sql #purpose/code-manipulation #category/language

## Description

Implements CEDARScript, a SQL-like language for code manipulation. This server provides a specialized query language designed for programmatic code analysis, transformation, and manipulation.

## Features

- SQL-like syntax for code operations
- Code pattern matching
- AST manipulation
- Query optimization
- Code transformation rules
- Syntax validation
- Custom function support
- Code generation
- Refactoring capabilities
- Performance profiling

## Installation

```bash
npm install @th3w1zard1/cedarscript-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "cedarscript": {
      "command": "npx",
      "args": ["@th3w1zard1/cedarscript-mcp"],
      "env": {
        "CEDAR_SCRIPT_PATH": "./scripts",
        "MAX_QUERY_DEPTH": "10",
        "ENABLE_CACHE": "true",
        "DEBUG_MODE": "false"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- SQL parser
- AST manipulation library
- Code formatter
- Query executor
- Cache system (optional)

## Related Servers

- modelcontextprotocol-git-server
- kivo360-anthropic-mcp-code-analyzer
- skydeckai-mcp-server-aidd
