---
type: server
repo_url: https://github.com/bmorphism/babashka-mcp-server
name: Babashka MCP Server
owner: bmorphism
stars: 1
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_003.md"]
tags: ["status/active", "category/scripting", "tech/clojure", "purpose/automation", "tech/babashka", "tech/javascript"]
---

# Babashka MCP Server

#status/active #category/scripting #tech/clojure #purpose/automation #tech/babashka #tech/javascript

## Description

A Model Context Protocol server for interacting with Babashka, a native Clojure interpreter for scripting. Enables execution and management of Babashka scripts with features like caching, command history access, and configurable timeouts for enhanced scripting workflows.

## Features

- Execute Babashka code through MCP tools
- Cache recent command results
- Access command history through MCP resources
- Configurable command timeouts
- Command execution with optional timeout settings
- Resource management for script results
- Support for Babashka language features
- Error handling and reporting

## Installation

```bash
# Install dependencies
npm install

# Build the MCP server
npm run build
```

## Usage

```javascript
{
  "mcpServers": {
    "babashka": {
      "command": "npx",
      "args": ["@bmorphism/babashka-mcp"],
      "env": {
        "BABASHKA_PATH": "bb",
        "CACHE_TTL": "3600",
        "HISTORY_SIZE": "100",
        "EXECUTION_TIMEOUT": "30000"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Babashka runtime
- MCP SDK
- TypeScript (for development)

## Related Servers

- None currently listed