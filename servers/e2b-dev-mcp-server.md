---
type: server
repo_url: https://github.com/e2b-dev/mcp-server
name: E2B
owner: e2b-dev
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
tags: ["status/active", "status/official", "category/development"]
---

#status/active #status/official #category/development

# E2B

## Description

Run code in secure sandboxes hosted by [E2B](https://e2b.dev). This MCP server provides a secure environment for executing code in isolated sandboxes, ensuring safe and controlled code execution.

## Features

- Secure code execution in isolated sandboxes
- Integration with E2B's hosted infrastructure
- Safe environment for running untrusted code
- Controlled resource allocation and management

## Installation

```bash
npm install @e2b/mcp-server
```

## Usage

```javascript
import { Server } from "@e2b/mcp-server";

const server = new Server({
  apiKey: "your-e2b-api-key",
});

// Execute code in sandbox
await server.execute({
  code: 'console.log("Hello from sandbox!")',
  language: "javascript",
});
```

## Dependencies

- Node.js >= 14.x
- E2B API key

## Related Servers

- None currently listed
