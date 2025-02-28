---
type: server
repo_url: https://github.com/hugoduncan/mcp-clj
name: Clojure REPL MCP Server
owner: hugoduncan
stars: 0
last_updated: 2025-01-24
status: active
official: false
verified: false
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/development",
    "tech/clojure",
    "purpose/repl",
    "tech/sse",
    "purpose/data-analysis",
  ]
---

# Clojure REPL MCP Server

#status/active #category/development #tech/clojure #purpose/repl #tech/sse #purpose/data-analysis

## Description

Exposes Clojure REPL functionality over SSE transport, enabling remote code execution and interactive data analysis. This MCP server provides a secure interface for Clojure development and data manipulation.

## Features

- REPL integration
- SSE transport
- Code execution
- Data analysis
- Interactive development
- Session management
- Code completion
- Error handling
- History tracking
- Result streaming

## Installation

```bash
npm install @hugoduncan/mcp-clj
```

## Usage

```javascript
{
  "mcpServers": {
    "clojure-repl": {
      "command": "npx",
      "args": ["@hugoduncan/mcp-clj"],
      "env": {
        "REPL_PORT": "7888",
        "SSE_ENDPOINT": "/repl-events",
        "MAX_HISTORY": "1000",
        "TIMEOUT": "30000",
        "SECURE_MODE": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Clojure runtime
- SSE support
- REPL environment
- History manager
- Security handler

## Related Servers

- bmorphism-babashka-mcp-server
- bigsy/clojars-mcp-server
- modelcontextprotocol-repl-server
