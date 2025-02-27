---
type: server
repo_url: https://github.com/browserbase/mcp-server-browserbase
name: mcp-server-browserbase
owner: browserbase
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources:
  - inbox
tags:
  - status/active
  - status/official
  - category/web-scraping
  - category/automation
  - purpose/development
---

# Browserbase MCP Server

#status/active #status/official #category/web-scraping #category/automation #purpose/development

## Description

Browserbase MCP Server enables cloud-based browser automation for web navigation, data extraction, form filling, and more. It provides a reliable and scalable solution for browser-based tasks without requiring local browser instances.

## Features

- Cloud-based browser automation
- Web navigation and interaction
- Data extraction capabilities
- Form filling automation
- Screenshot capture
- Network request monitoring
- Geolocation spoofing
- Proxy support

## Installation

```bash
npm install @browserbase/mcp-server
```

## Usage

```javascript
{
  "mcpServers": {
    "browserbase": {
      "command": "npx",
      "args": ["@browserbase/mcp-server"],
      "env": {
        "BROWSERBASE_API_KEY": "your-api-key"
      }
    }
  }
}
```

## Dependencies

- Node.js v16 or higher
- Browserbase account with API key

## Related Servers

- [Puppeteer](https://github.com/modelcontextprotocol/servers/tree/main/src/puppeteer)
- [Apify](https://github.com/apify/actors-mcp-server)
- [FireCrawl](https://github.com/mendableai/firecrawl-mcp-server)
