---
type: server
repo_url: https://github.com/TheSethRose/Fetch-Browser
name: Fetch Browser MCP Server
owner: TheSethRose
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_011.md"]
tags:
  [
    "status/active",
    "category/web",
    "purpose/web-scraping",
    "integration/google",
    "tech/headless-browser",
    "purpose/content-analysis",
    "tech/typescript",
    "tech/puppeteer"
  ]
---

# Fetch Browser MCP Server

#status/active #category/web #purpose/web-scraping #integration/google #tech/headless-browser #purpose/content-analysis #tech/typescript #tech/puppeteer

## Description

Fetch Browser enables headless web content retrieval and Google searching without API keys, supporting multiple output formats for web scraping and content analysis tasks. It leverages Puppeteer for browser automation and provides tools for extracting structured data from web pages and search results.

## Features

- Headless browsing
- Google search integration
- No API key requirement
- Multiple output formats
- Content scraping
- Search automation
- Format conversion
- Result filtering
- Error handling
- Rate limiting
- Structured data extraction
- Automatic retries
- Configurable search limits
- Universal content fetching

## Installation

```bash
# Install dependencies
npm install

# Build the project
npm run build

# Start the server
npm start
```

## Usage

```javascript
{
  "mcpServers": {
    "fetch-browser": {
      "command": "npx",
      "args": ["@thesethrose/fetch-browser"],
      "env": {
        "HEADLESS": "true",
        "OUTPUT_FORMAT": "json",
        "SEARCH_LIMIT": "10",
        "USER_AGENT": "Mozilla/5.0"
      }
    }
  }
}

// Available Tools
google_search:
  - query: Search query
  - responseType: Output format (markdown, json, html, text)
  - maxResults: Number of results (1-100)
  - topic: Search topic (web, news)

fetch_url:
  - url: URL to fetch
  - responseType: Output format (markdown, json, html, text)
  - timeout: Request timeout (milliseconds)
```

## Dependencies

- Node.js >= 14
- Puppeteer
- Chrome/Chromium
- TypeScript
- Network connectivity
- Storage space

## Related Servers

- modelcontextprotocol/fetch-server