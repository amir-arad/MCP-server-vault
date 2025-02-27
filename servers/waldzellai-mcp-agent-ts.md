---
type: server
repo_url: https://github.com/waldzellai/mcp-agent-ts
name: Agent TS MCP Server
owner: waldzellai
stars: 0
last_updated: 2025-02-18
status: active
official: false
verified: false
sources: ["inbox/batch_001.md"]
tags: ["status/active", "category/development", "tech/typescript", "purpose/agent-framework"]
---

# Agent TS MCP Server

#status/active #category/development #tech/typescript #purpose/agent-framework

## Description

A TypeScript implementation of the MCP Agent framework, providing tools for building context-aware agents with advanced workflow management, logging, and execution capabilities.

## Features

- Context-aware agent framework
- Advanced workflow management
- Comprehensive logging system
- Execution capabilities
- TypeScript implementation
- Extensible architecture

## Installation

```bash
npm install @waldzellai/mcp-agent-ts
```

## Usage

```javascript
{
  "mcpServers": {
    "agent-ts": {
      "command": "npx",
      "args": ["@waldzellai/mcp-agent-ts"],
      "env": {
        "LOG_LEVEL": "info",
        "WORKFLOW_DIR": "./workflows",
        "MAX_CONCURRENT_TASKS": "5"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- TypeScript >= 4.5
- MCP framework

## Related Servers

- None currently listed