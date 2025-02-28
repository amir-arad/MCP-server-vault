---
type: server
repo_url: https://github.com/wonderwhy-er/ClaudeComputerCommander
name: Claude Computer Commander MCP Server
owner: wonderwhy-er
stars: 40
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/system",
    "purpose/automation",
    "purpose/process-management",
    "tech/terminal",
    "tech/filesystem",
  ]
---

# Claude Computer Commander MCP Server

#status/active #category/system #purpose/automation #purpose/process-management #tech/terminal #tech/filesystem

## Description

Integrates terminal and filesystem capabilities for executing system commands, managing processes, and performing advanced file operations on the local system.

## Features

- System command execution
- Process management
- File operations
- Directory handling
- Permission management
- Environment control
- Job scheduling
- Output capture
- Error handling
- Resource monitoring

## Installation

First, ensure you've downloaded and installed the [Claude Desktop app](https://claude.ai/download) and you have [npm installed](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm).

### Option 1: Installing via Smithery

To install Desktop Commander for Claude Desktop automatically via [Smithery](https://smithery.ai/server/@wonderwhy-er/desktop-commander):

```bash
npx -y @smithery/cli install @wonderwhy-er/desktop-commander --client claude
```

### Option 2: Install trough npx

Just run this in terminal

```bash
npx @wonderwhy-er/desktop-commander setup
```

Restart Claude if running

### Option 3: Add to claude_desktop_config by hand

Add this entry to your claude_desktop_config.json (on Mac, found at ~/Library/Application\\ Support/Claude/claude_desktop_config.json):

```json
{
  "mcpServers": {
    "desktop-commander": {
      "command": "npx",
      "args": ["-y", "@wonderwhy-er/desktop-commander"]
    }
  }
}
```

Restart Claude if running

### Option 4: Checkout locally

1.  Clone and build:

```bash
git clone https://github.com/wonderwhy-er/ClaudeComputerCommander.git
cd ClaudeComputerCommander
npm run setup
```

Restart Claude if running

The setup command will:

- Install dependencies
- Build the server
- Configure Claude's desktop app
- Add MCP servers to Claude's config if needed

## Usage

```javascript
{
  "mcpServers": {
    "computer-commander": {
      "command": "npx",
      "args": ["@wonderwhy-er/claude-computer-commander"],
      "env": {
        "ALLOWED_PATHS": "/home/user,/tmp",
        "MAX_PROCESSES": "10",
        "TIMEOUT": "30000",
        "LOG_LEVEL": "info",
        "SANDBOX_ENABLED": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Shell access
- Process manager
- File system API
- Permission handler
- Resource monitor

## Related Servers

- modelcontextprotocol-filesystem-server
- andre-jesus-claude-mcp
- shin-t-o-mcp-access
