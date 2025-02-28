---
type: server
repo_url: https://github.com/mcprouter/exa-ai-mcp-server
name: Exa AI MCP Server
owner: mcprouter
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_011.md"]
tags:
  [
    "status/active",
    "category/search",
    "integration/exa",
    "category/ai",
    "purpose/web-search",
    "purpose/content-generation",
    "tech/typescript"
  ]
---

# Exa AI MCP Server

#status/active #category/search #integration/exa #category/ai #purpose/web-search #purpose/content-generation #tech/typescript

## Description

Integrates with Exa's API to enable web searches for AI models, enhancing tasks like research, fact-checking, and content generation with current data. It provides a tool for AI models to access and utilize real-time web information.

## Features

- Web search integration
- AI model support
- Research assistance
- Fact-checking
- Content generation
- Search filtering
- Result ranking
- Data validation
- Query optimization
- Context preservation
- Exa API integration
- TypeScript implementation

## Installation

```bash
bun install
```

## Usage

```javascript
{
  "mcpServers": {
    "exa-ai": {
      "command": "bun",
      "args": ["run", "index.ts"],
      "env": {
        "EXA_API_KEY": "your-api-key",
        "MAX_RESULTS": "10",
        "SEARCH_TIMEOUT": "30000",
        "CACHE_DURATION": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 18
- Exa API access
- Network connectivity
- Cache storage
- Rate limiting system
- Bun runtime

## Related Servers

- exa-labs/exa-mcp-server