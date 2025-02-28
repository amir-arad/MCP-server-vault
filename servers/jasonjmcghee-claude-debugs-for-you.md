---
type: server
repo_url: https://github.com/jasonjmcghee/claude-debugs-for-you
name: Claude Debug Assistant MCP Server
owner: jasonjmcghee
stars: 116
last_updated: 2025-02-28
status: active
official: false
verified: true
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

## Getting Started

1. Download the extension from [releases](https://github.com/jasonjmcghee/claude-debugs-for-you/releases/) or [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=JasonMcGhee.claude-debugs-for-you)
2. Install the extension

- If using `.vsix` directly, go to the three dots in "Extensions" in VS Code and choose "Install from VSIX..."

3. Open a project containing a `.vscode/launch.json` with the first configuration setup to debug a specific file with `${file}`.
4. On startup, a popup will show that the debug server started and a path to the node binary

- This can be disabled in settings (e.g. once you've done it the first time or if you're using /sse)

### If using node process based method (required for Claude Desktop)

5. Copy the path of the node binary to `mcp-debug.js` in the popup

6. Paste the following (BUT UPDATE THE PATH TO THE COPIED ONE!) in your `claude_desktop_config.json` or edit accordingly if you use other MCP servers

```
{
  "mcpServers": {
    "debug": {
      "command": "node",
      "args": [        "/path/to/mcp-debug.js"
      ]
    }
  }
}
```

7. Start Claude desktop (or other MCP client)

- Note: You may need to restart it, if it was already running.
- You can skip this step if using Continue/Cursor or other built-in to VS Code

### If using `/sse` based method (e.g. Cursor)

4. Add the MCP server using the server URL of "[http://localhost:4711/sse](http://localhost:4711/sse)", or whatever port you setup in settings.

- You may need to hit "refresh" depending on client: this is required in Cursor

5. Start MCP client

- Note: You may need to restart it, if it was already running.
- You can skip this step if using Continue/Cursor or other built-in to VS Code

### You're ready to debug!

See [Run an Example](https://github.com/jasonjmcghee/claude-debugs-for-you#run-an-example) below, and/or watch a demo video.

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
