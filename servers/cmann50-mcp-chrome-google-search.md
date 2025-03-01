---
type: server
repo_url: https://github.com/cmann50/mcp-chrome-google-search
name: Chrome Google Search MCP Server
owner: cmann50
stars: 10
last_updated: 2025-03-01
status: active
official: false
verified: true
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/search",
    "integration/chrome",
    "integration/google",
    "tech/macos",
    "purpose/web-extraction",
  ]
---

# Chrome Google Search MCP Server

#status/active #category/search #integration/chrome #integration/google #tech/macos #purpose/web-extraction

## Description

Enables Google search and webpage content extraction via Chrome for macOS, allowing access to both unauthenticated and authenticated content, and integrates with Claude for secure and automated browsing tasks.

## Features

- Google search integration
- Webpage content extraction
- Authenticated browsing
- Search result parsing
- Content scraping
- Cookie management
- Session handling
- Screenshot capture
- PDF generation
- Security controls

## Installation

```bash
npm install @cmann50/mcp-chrome-google-search
```

## Usage

```javascript
{
  "mcpServers": {
    "chrome-search": {
      "command": "npx",
      "args": ["@cmann50/mcp-chrome-google-search"],
      "env": {
        "CHROME_PATH": "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome",
        "GOOGLE_COOKIES": "path/to/cookies.json",
        "MAX_RESULTS": "10",
        "SAFE_SEARCH": "moderate",
        "TIMEOUT": "30000"
      }
    }
  }
}
```

## Dependencies

- macOS
- Google Chrome
- Node.js >= 20
- Chrome DevTools Protocol
- Google account (optional)
- Cookie manager

## Related Servers

- modelcontextprotocol-puppeteer-server
- hrmeetsingh-mcp-browser-automation
- saik0s-mcp-browser-use
