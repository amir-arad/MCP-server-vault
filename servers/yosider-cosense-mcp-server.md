---
type: server
repo_url: https://github.com/yosider/cosense-mcp-server
name: Cosense Pipeline MCP Server
owner: yosider
stars: 3
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/middleware",
    "integration/cosense",
    "integration/claude",
    "purpose/pipeline",
    "purpose/command-processing",
    "tech/typescript",
    "tech/javascript",
    "tech/jsr"
  ]
---

# Cosense Pipeline MCP Server

#status/active #category/middleware #integration/cosense #integration/claude #purpose/pipeline #purpose/command-processing #tech/typescript #tech/javascript #tech/jsr

## Description

A TypeScript-based MCP server that serves as a middleware command pipeline for interacting with Cosense projects. The server provides a standardized interface for page management, content search, and line insertion operations, with support for both public and private project access through session authentication.

## Features

- Page content retrieval and management
- Resource listing and discovery
- Content search capabilities
- Line insertion and text manipulation
- Command pipeline processing
- Session-based authentication
- Project interaction
- Command routing
- Error handling
- Status tracking
- Result formatting

## Installation

```bash
# Configure JSR registry first
echo "@jsr:registry=https://npm.jsr.io" >> ~/.npmrc  # Linux/macOS
echo "@jsr:registry=https://npm.jsr.io" >> $env:USERPROFILE\.npmrc  # Windows

# Install via npm
npm install @yosider/cosense-mcp

# Or build from source
git clone https://github.com/yosider/cosense-mcp-server.git
cd cosense-mcp-server
npm install
npm run build
```

## Usage

```javascript
{
  "mcpServers": {
    "cosense-pipeline": {
      "command": "npx",
      "args": ["@yosider/cosense-mcp"],
      "env": {
        "COSENSE_PROJECT_NAME": "your-project-name",
        "COSENSE_SID": "your-sid",  // Required for private projects
        "COSENSE_URL": "your-cosense-url",
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
- TypeScript runtime
- @cosense/std (via JSR)
- @cosense/types (via JSR)
- Cosense account
- Pipeline processor
- Command router
- Event handler
- MCP Inspector (for debugging)

## Related Servers

- funwarioisii/cosense-mcp-server (original project)
- modelcontextprotocol-pipeline-server
- modelcontextprotocol-middleware-server