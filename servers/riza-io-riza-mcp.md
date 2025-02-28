---
type: server
repo_url: https://github.com/riza-io/riza-mcp
name: Riza
owner: riza-io
stars: 4
last_updated: 2025-02-28
status: active
official: true
verified: true
sources: ["inbox"]
tags:
  [
    "status/active",
    "status/official",
    "category/development",
    "category/ai",
    "tech/nodejs",
  ]
---

#status/active #status/official #category/development #category/ai

# Riza

## Description

Arbitrary code execution and tool-use platform for LLMs by [Riza](https://riza.io). This MCP server provides a secure and flexible environment for LLMs to execute code and use tools in a controlled manner.

## Features

- Secure code execution
- Tool integration framework
- LLM interaction capabilities
- Sandboxed environments
- Custom tool development
- Code analysis and validation
- Resource management
- Execution monitoring
- Error handling
- Tool usage analytics

## Installation

```bash
npm install @riza/mcp-server
```

## Usage

```javascript
import { RizaServer } from "@riza/mcp-server";

const server = new RizaServer({
  apiKey: "your-riza-api-key",
  environment: "production",
});

// Execute code in sandbox
const result = await server.execute({
  code: `
    function calculateSum(numbers) {
      return numbers.reduce((sum, n) => sum + n, 0);
    }
    calculateSum([1, 2, 3, 4, 5]);
  `,
  language: "javascript",
  timeout: 5000,
});

// Register custom tool
await server.registerTool({
  name: "data-processor",
  description: "Process and transform data",
  schema: {
    input: {
      type: "object",
      properties: {
        data: { type: "array" },
        operation: { type: "string" },
      },
    },
    output: {
      type: "array",
    },
  },
  handler: async (input) => {
    // Tool implementation
    return processData(input.data, input.operation);
  },
});

// Use tool with LLM
const toolResult = await server.useTool({
  tool: "data-processor",
  input: {
    data: [1, 2, 3, 4, 5],
    operation: "square",
  },
  llmContext: {
    model: "gpt-4",
    temperature: 0.7,
  },
});
```

## Dependencies

- Node.js >= 14.x
- Riza account
- Riza API key
- Docker (optional, for isolated execution)

## Related Servers

- None currently listed
