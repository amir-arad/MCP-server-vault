---
type: server
repo_url: https://github.com/JetBrains/mcp-jetbrains
name: JetBrains MCP Proxy Server
owner: JetBrains
stars: 0
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
    "integration/jetbrains",
  ]
---

# JetBrains MCP Proxy Server

#status/active #status/official #category/development #integration/jetbrains

## Description

The server proxies requests from client to JetBrains IDE. This MCP server provides integration with JetBrains' suite of development tools, enabling AI agents to interact with and control JetBrains IDEs for enhanced development workflows.

## Features

- Proxies requests from client to JetBrains IDE.

## Install MCP Server plugin

[https://plugins.jetbrains.com/plugin/26071-mcp-server](https://plugins.jetbrains.com/plugin/26071-mcp-server)

## Usage with Claude Desktop

To use this with Claude Desktop, add the following to your `claude_desktop_config.json`. The full path on MacOS: `~/Library/Application\ Support/Claude/claude_desktop_config.json`, on Windows: `%APPDATA%/Claude/claude_desktop_config.json`.

```json
{
  "mcpServers": {
    "jetbrains": {
      "command": "npx",
      "args": ["-y", "@jetbrains/mcp-proxy"]
    }
  }
}
```

## Configuration

If you're running multiple IDEs with MCP server and want to connect to the specific one, add to the MCP server configuration:

```json
"env": {
  "IDE_PORT": "<port of IDE's built-in webserver>"
}
```

By default, we connect to IDE on 127.0.0.1 but you can specify a different address/host:

```json
"env": {
  "HOST": "<host/address of IDE's built-in webserver>"
}
```

To enable logging add:

```json
"env": {
  "LOG_ENABLED": "true"
}
```

## How to build

1. Tested on macOS
2. `brew install node pnpm`
3. Run `pnpm build` to build the project

## Dependencies

- Node.js >= 14.x
- JetBrains IDE installation
- JetBrains API key
- JetBrains Gateway (for remote development)

## Related Servers

- None currently listed
