---
type: server
repo_url: https://github.com/MatthewDailey/figma-mcp
name: Figma MCP Server
owner: MatthewDailey
stars: 15
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_012.md"]
tags:
  [
    "status/active",
    "category/design",
    "integration/figma",
    "tech/rest-api",
    "purpose/design-analysis",
    "purpose/collaboration",
  ]
---

# Figma MCP Server

#status/active #category/design #integration/figma #tech/rest-api #purpose/design-analysis #purpose/collaboration

## Description

Interact with Figma design files through the Figma REST API for design analysis, feedback, and collaboration.

## Features

- Figma API integration
- Design file access
- Design analysis
- Feedback management
- Collaboration tools
- File version control
- Component tracking
- Style management
- Comment handling
- Team permissions

## Installation

```bash
npm install @matthewdailey/figma-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "figma": {
      "command": "npx",
      "args": ["@matthewdailey/figma-mcp"],
      "env": {
        "FIGMA_ACCESS_TOKEN": "your-access-token",
        "TEAM_ID": "your-team-id",
        "CACHE_DURATION": "3600",
        "WEBHOOK_URL": "your-webhook-url"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Figma API access
- REST client
- Cache system
- Webhook handler

## Related Servers

- [Figma Context MCP](https://github.com/GLips/Figma-Context-MCP) - Cursor integration for Figma
- [Figma Server](https://github.com/TimHolden/figma-mcp-server) - Alternative Figma implementation
