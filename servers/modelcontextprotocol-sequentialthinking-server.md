---
type: server
repo_url: https://github.com/modelcontextprotocol/servers/src/sequentialthinking
name: Sequential Thinking
owner: modelcontextprotocol
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
related_tags: ["category/ai", "status/official", "purpose/development", "tech/typescript"]
---

# Sequential Thinking

## Description

A reference MCP server that enables dynamic and reflective problem-solving through thought sequences. This server demonstrates advanced reasoning and problem decomposition capabilities.

## Features

- Dynamic thought sequence generation
- Problem decomposition
- Reflective analysis
- Context maintenance
- Hypothesis generation and testing
- Solution verification
- Thought revision capabilities

## Installation

```bash
npm install @modelcontextprotocol/sequentialthinking-server
```

## Usage

```javascript
import { Server } from '@modelcontextprotocol/sdk/server';
import { SequentialThinkingServer } from '@modelcontextprotocol/sequentialthinking-server';

const server = new SequentialThinkingServer({
  maxThoughts: 10,
  allowRevision: true
});
server.run();
```

## Dependencies

- @modelcontextprotocol/sdk
- TypeScript

## Related Servers

- Memory Server - For maintaining thought context
- PostgreSQL Server - For storing thought sequences