--- 
type: server
repo_url: https://github.com/waldzellai/mcp-agent-ts
name: Agent TS MCP Server
owner: waldzellai
stars: 2
last_updated: 2025-02-28
status: active
official: false
verified: true
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

### Installing via Smithery

To install Agent TS MCP Server for Claude Desktop automatically via [Smithery](https://smithery.ai/server/@waldzellai/mcp-agent-ts):

```bash
npx -y @smithery/cli install @waldzellai/mcp-agent-ts --client claude
```

## Usage

### Creating a Workflow

```typescript
import { BaseWorkflow } from '@waldzell/mcp-agent-ts';

class MyDataProcessingWorkflow extends BaseWorkflow {
 constructor() {
 super('my-workflow', 'Data Processing');

 this.addStep({
 id: 'extract',
 name: 'Data Extraction',
 execute: async (context) => {
 // Implement data extraction logic
 return { data: ['item1', 'item2'] };
 }
 });

 this.addStep({
 id: 'transform',
 name: 'Data Transformation',
 execute: async (context) => {
 // Implement data transformation logic
 return { transformedData: ['ITEM1', 'ITEM2'] };
 }
 });
 }
}

async function runWorkflow() {
 const workflow = new MyDataProcessingWorkflow();
 const results = await workflow.execute();
 console.log(results);
}
```

### Logging

```typescript
import { debug, info, warn, error } from '@waldzell/mcp-agent-ts';

// Log with different levels
debug('Debugging information', { userId: 123 });
info('System started');
warn('Potential issue detected');
error('Critical error occurred');
```

### CLI Usage

```bash
# Start the MCP Agent
npx mcp-agent start

# List available tools
npx mcp-agent list-tools

# Set log level
npx mcp-agent log-level debug
```

## Dependencies

- Node.js >= 16
- TypeScript >= 4.5
- MCP framework

## Related Servers

- None currently listed