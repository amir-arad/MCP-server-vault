---
type: server
repo_url: https://github.com/yosider/cosense-mcp-server
name: Cosense Pipeline MCP Server
owner: yosider
stars: 3
last_updated: 2025-02-02
status: active
official: false
verified: false
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/middleware",
    "integration/cosense",
    "integration/claude",
    "purpose/pipeline",
    "purpose/command-processing",
  ]
---

# Cosense Pipeline MCP Server

#status/active #category/middleware #integration/cosense #integration/claude #purpose/pipeline #purpose/command-processing

## Description

The cosense-mcp-server facilitates the integration with Claude Desktop by serving as a middleware command pipeline server, allowing for interaction with projects in cosense.

## Features

- Command pipeline
- Middleware processing
- Claude integration
- Project interaction
- Command routing
- Pipeline management
- Error handling
- Event processing
- Status tracking
- Result formatting

## Installation

```bash
npm install @yosider/cosense-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "cosense-pipeline": {
      "command": "npx",
      "args": ["@yosider/cosense-mcp"],
      "env": {
        "COSENSE_URL": "your-cosense-url",
        "CLAUDE_API_KEY": "your-claude-key",
        "PIPELINE_TIMEOUT": "30000",
        "MAX_RETRIES": "3",
        "LOG_LEVEL": "info"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Claude API access
- Cosense account
- Pipeline processor
- Command router
- Event handler

## Related Servers

- funwarioisii/cosense-mcp-server
- modelcontextprotocol-pipeline-server
- modelcontextprotocol-middleware-server
