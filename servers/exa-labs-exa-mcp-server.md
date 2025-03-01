---
type: server
repo_url: https://github.com/exa-labs/exa-mcp-server
name: Exa MCP Server
owner: exa-labs
stars: 243
last_updated: 2025-02-28
status: active
official: true
verified: true
sources: ["inbox/batch_011.md"]
tags:
  [
    "status/active",
    "status/official",
    "category/search",
    "category/ai",
    "integration/exa",
    "purpose/web-search",
    "tech/javascript",
    "tech/typescript",
  ]
---

# Exa MCP Server

#status/active #status/official #category/search #category/ai #integration/exa #purpose/web-search

## Description

A Model Context Protocol (MCP) server lets AI assistants like Claude use the Exa AI Search API for web searches. This setup allows AI models to get real-time web information in a safe and controlled way.

## Features

- AI-powered web search
- Safe search controls
- Real-time information
- Search customization
- Result filtering
- Context preservation
- Rate limiting
- Error handling
- Cache management
- Analytics tracking

## Installation

```bash
npm install @exa-labs/exa-mcp-server
```

## Usage

```javascript
{
  "mcpServers": {
    "exa": {
      "command": "npx",
      "args": ["@exa-labs/exa-mcp-server"],
      "env": {
        "EXA_API_KEY": "your-api-key",
        "SAFE_SEARCH": "true",
        "RESULTS_PER_PAGE": "10",
        "CACHE_TTL": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Exa AI Search API access
- Network connectivity
- Cache storage
- Rate limiting system

## Related Servers

- [Exa AI Server](https://github.com/mcprouter/exa-ai-mcp-server) - Community Exa implementation
