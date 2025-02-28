---
type: server
repo_url: https://github.com/nahmanmate/code-research-mcp-server
name: Code Research MCP Server
owner: nahmanmate
stars: 13
last_updated: 2025-02-18
status: active
official: false
verified: false
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/research",
    "purpose/documentation",
    "integration/stackoverflow",
    "integration/mdn",
    "integration/github",
  ]
---

# Code Research MCP Server

#status/active #category/research #purpose/documentation #integration/stackoverflow #integration/mdn #integration/github

## Description

Facilitates searching and accessing programming resources across platforms like Stack Overflow, MDN, GitHub, npm, and PyPI, aiding LLMs in finding code examples and documentation.

## Features

- Multi-platform search
- Documentation access
- Code example retrieval
- Resource aggregation
- Result filtering
- Content caching
- Query optimization
- Source attribution
- Rating integration
- Answer validation

## Installation

```bash
npm install @nahmanmate/code-research-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "code-research": {
      "command": "npx",
      "args": ["@nahmanmate/code-research-mcp"],
      "env": {
        "STACKOVERFLOW_KEY": "your-so-key",
        "GITHUB_TOKEN": "your-github-token",
        "CACHE_TTL": "3600",
        "MAX_RESULTS": "10",
        "PLATFORMS": "stackoverflow,mdn,github,npm,pypi"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Platform APIs
- Cache system
- Search engine
- Content parser
- Result aggregator

## Related Servers

- modelcontextprotocol-docs-server
- afrise-academic-search-mcp-server
- blazickjp-arxiv-mcp-server
