---
type: server
repo_url: https://github.com/qpd-v/mcp-DEEPwebresearch
name: Deep Web Research MCP Server
owner: qpd-v
stars: 17
last_updated: 2025-02-19
status: active
official: false
verified: false
sources: ["inbox/batch_009.md"]
tags:
  [
    "status/active",
    "category/research",
    "integration/google",
    "purpose/web-research",
    "integration/claude",
    "tech/screenshots",
  ]
---

# Deep Web Research MCP Server

#status/active #category/research #integration/google #purpose/web-research #integration/claude #tech/screenshots

## Description

The MCP Web Research Server enables real-time web research with Claude by integrating Google search, capturing webpage content and screenshots, and tracking research sessions.

## Features

- Google search integration
- Webpage content capture
- Screenshot generation
- Session tracking
- Research history
- Content analysis
- Result filtering
- Data organization
- Export capabilities
- Progress tracking

## Installation

```bash
npm install @qpd-v/deep-web-research-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "web-research": {
      "command": "npx",
      "args": ["@qpd-v/deep-web-research-mcp"],
      "env": {
        "GOOGLE_API_KEY": "your-api-key",
        "SCREENSHOT_PATH": "./screenshots",
        "SESSION_TTL": "3600",
        "MAX_DEPTH": "3",
        "SAVE_CONTENT": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Google Search API
- Screenshot tool
- Content extractor
- Session manager
- Storage system

## Related Servers

- modelcontextprotocol-search-server
- ozamatash/deep-research-mcp
- ssdeanx/deep-research-mcp
