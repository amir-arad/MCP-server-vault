---
type: server
repo_url: https://github.com/jasonjmcghee/claude-debugs-for-you
name: Claude Debug Assistant MCP Server
owner: jasonjmcghee
stars: 116
last_updated: 2025-02-21
status: active
official: false
verified: false
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/development",
    "integration/vscode",
    "purpose/debugging",
    "tech/debugger",
    "category/ai",
  ]
---

# Claude Debug Assistant MCP Server

#status/active #category/development #integration/vscode #purpose/debugging #tech/debugger #category/ai

## Description

Integrates with VS Code's debugging capabilities to enable interactive code debugging and expression evaluation. This MCP server enhances debugging workflows by providing AI-assisted analysis and suggestions during debugging sessions.

## Features

- Interactive debugging
- Expression evaluation
- Breakpoint management
- Variable inspection
- Call stack analysis
- Watch expressions
- Memory inspection
- Exception handling
- Debug console integration
- AI-powered suggestions

## Installation

```bash
npm install @jasonjmcghee/claude-debugs-for-you
```

## Usage

```javascript
{
  "mcpServers": {
    "claude-debug": {
      "command": "npx",
      "args": ["@jasonjmcghee/claude-debugs-for-you"],
      "env": {
        "VSCODE_EXTENSION_ID": "your-extension-id",
        "DEBUG_PORT": "5678",
        "LOG_LEVEL": "info",
        "AI_SUGGESTIONS": "true",
        "MAX_CALL_DEPTH": "50"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- VS Code
- Debug Adapter Protocol
- Claude API access
- Language servers
- Debug extensions

## Related Servers

- modelcontextprotocol-vscode-server
- kivo360-anthropic-mcp-code-analyzer
- skydeckai-mcp-server-aidd
