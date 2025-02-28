---
type: server
repo_url: https://github.com/andre-jesus/claude-mcp
name: Claude Terminal Monitor MCP Server
owner: andre-jesus
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/monitoring",
    "integration/terminal",
    "purpose/log-analysis",
    "purpose/debugging",
    "tech/typescript",
  ]
---

# Claude Terminal Monitor MCP Server

#status/active #category/monitoring #integration/terminal #purpose/log-analysis #purpose/debugging #tech/typescript

## Description

Integrates terminal monitoring capabilities, enabling real-time analysis of multiple terminal outputs for debugging, log review, and system monitoring.

## Features

- Multi-terminal monitoring
- Real-time log analysis
- Pattern matching
- Alert generation
- Output filtering
- Session recording
- Search capabilities
- Performance metrics
- Error detection
- Report generation

## Installation

```bash
npm install @andre-jesus/claude-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "terminal-monitor": {
      "command": "npx",
      "args": ["@andre-jesus/claude-mcp"],
      "env": {
        "TERMINAL_PATHS": "/dev/pts/0,/dev/pts/1",
        "LOG_PATH": "./logs",
        "PATTERN_FILE": "./patterns.json",
        "ALERT_THRESHOLD": "5",
        "RECORD_OUTPUT": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Terminal access
- PTY.js
- Log parser
- Pattern matcher
- Storage system

## Related Servers

- modelcontextprotocol-terminal-server
- macrat-mcp-ayd-server
- andre-jesus/system-monitor-mcp
