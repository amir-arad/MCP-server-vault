---
type: server
repo_url: https://github.com/mahawi1992/mcp-documentation-server
name: Documentation MCP Server
owner: mahawi1992
stars: 4
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_010.md"]
tags:
  [
    "status/active",
    "category/documentation",
    "purpose/web-scraping",
    "purpose/documentation-management",
    "purpose/programming-support",
    "tech/web",
  ]
---

# Documentation MCP Server

#status/active #category/documentation #purpose/web-scraping #purpose/documentation-management #purpose/programming-support #tech/web

## Description

A smart documentation server that provides AI-assisted code improvement and documentation management through Claude Desktop integration. Manages up-to-date documentation scraped from the web to support your programming workflows. Keeps local copies of documentation synchronized with online sources.

## Features

- **AI Documentation Guide**: Maintains and updates documentation knowledge base
- **AI Code Assistant**: Analyzes and improves code quality
- **Framework Support**:
  - React.js
  - Next.js (with App Router)
  - Python
  - Vue.js
  - Angular
  - Node.js
- **Brave Search Integration**: Smart documentation search and retrieval
- **Learning System**: Improves suggestions over time
- Web documentation scraping
- Documentation versioning
- Automatic updates
- Local caching
- Search functionality
- Content organization
- Multiple source support
- Offline access
- Version comparison
- Change tracking

## Installation

```bash
npm install -g mcp-documentation-server
```

## Usage

Configure Claude Desktop (config.json):

```json
{
  "mcpServers": {
    "documentation": {
      "command": "npx",
      "args": ["-y", "mcp-documentation-server"],
      "env": {
        "BRAVE_API_KEY": "<YOUR_BRAVE_API_KEY>"
      }
    }
  }
}
```

Start using with Claude:

```
Claude, search documentation for Next.js App Router
```

For detailed setup instructions, see [Claude Desktop Setup Guide](https://github.com/mahawi1992/mcp-documentation-server/blob/main/docs/CLAUDE_DESKTOP_SETUP.md)

## Dependencies

- Node.js >= 16
- Storage space for caching
- Internet connection for updates
- Web scraping libraries
- Search indexing engine
