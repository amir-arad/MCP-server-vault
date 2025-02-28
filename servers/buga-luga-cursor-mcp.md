---
type: server
repo_url: https://github.com/Buga-luga/cursor-mcp
name: Cursor Editor MCP Server
owner: Buga-luga
stars: 26
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_008.md"]
tags:
  [
    "status/active",
    "category/development",
    "integration/cursor",
    "purpose/code-analysis",
    "purpose/indexing",
    "tech/real-time",
    "tech/typescript",
    "tech/nodejs",
    "integration/claude",
    "purpose/ai-assistance"
  ]
---

# Cursor Editor MCP Server

#status/active #category/development #integration/cursor #purpose/code-analysis #purpose/indexing #tech/real-time #tech/typescript #tech/nodejs #integration/claude #purpose/ai-assistance

## Description

A TypeScript-based MCP server that enables seamless integration between Claude AI and desktop applications through Cursor IDE. The server facilitates real-time code indexing, analysis, and bi-directional communication, supporting concurrent sessions and automatic reconnection. It serves as a bridge between Claude's AI capabilities and desktop software, enabling enhanced AI-powered development workflows.

## Features

- Real-time code indexing
- AI-powered code analysis
- Bi-directional communication
- Concurrent session support
- Auto reconnection handling
- Code navigation tools
- Symbol lookup system
- Change tracking
- Session management
- Error handling
- Context-aware suggestions
- Windows automation
- IDE integration
- Real-time assistance
- Development workflow optimization

## Installation

```bash
# Global installation
npm install -g mcp-cursor

# Local installation
git clone https://github.com/Buga-luga/cursor-mcp.git
cd cursor-mcp
npm install

# Configure environment
cp .env.example .env
# Set workspace path in .env:
DEFAULT_WORKSPACE_PATH=C:/Users/YourUsername/Documents/cursor-workspaces
```

## Usage

```javascript
// Configuration
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

// Claude MCP Configuration
{
  "name": "cursor",
  "type": "mcp",
  "config": {
    "server": "https://glama.ai/mcp/servers/4fg1gxbcex",
    "capabilities": ["cursor_control", "window_management"]
  }
}
```

## Dependencies

- Node.js >= 18
- TypeScript runtime
- Cursor IDE
- Code indexer
- Analysis engine
- WebSocket client
- Session manager
- Windows API
- Claude AI integration
- Event handlers
- Real-time processors

## Related Servers

- kleneway-awesome-cursor-mpc-server
- norbinsh/cursor-mcp-trivy
- westsideori/cursor-a11y-mcp
- modelcontextprotocol-ide-server