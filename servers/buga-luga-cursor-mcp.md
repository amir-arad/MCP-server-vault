---
type: server
repo_url: https://github.com/Buga-luga/cursor-mcp
name: Cursor Editor MCP Server
owner: Buga-luga
stars: 26
last_updated: 2025-02-21
status: active
official: false
verified: false
sources: ["inbox/batch_008.md"]
tags:
  [
    "status/active",
    "category/development",
    "integration/cursor",
    "purpose/code-analysis",
    "purpose/indexing",
    "tech/real-time",
  ]
---

# Cursor Editor MCP Server

#status/active #category/development #integration/cursor #purpose/code-analysis #purpose/indexing #tech/real-time

## Description

Facilitates integration with the Cursor code editor by enabling real-time code indexing, analysis, and bi-directional communication with Claude, supporting concurrent sessions and automatic reconnection.

## Features

- Real-time code indexing
- Code analysis
- Bi-directional communication
- Concurrent sessions
- Auto reconnection
- Code navigation
- Symbol lookup
- Change tracking
- Session management
- Error handling

## Installation

```bash
npm install @buga-luga/cursor-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "cursor-editor": {
      "command": "npx",
      "args": ["@buga-luga/cursor-mcp"],
      "env": {
        "CURSOR_PATH": "/path/to/cursor",
        "MAX_SESSIONS": "5",
        "INDEX_INTERVAL": "1000",
        "AUTO_RECONNECT": "true",
        "LOG_LEVEL": "info"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Cursor editor
- Code indexer
- Analysis engine
- WebSocket client
- Session manager

## Related Servers

- kleneway-awesome-cursor-mpc-server
- norbinsh/cursor-mcp-trivy
- westsideori/cursor-a11y-mcp
