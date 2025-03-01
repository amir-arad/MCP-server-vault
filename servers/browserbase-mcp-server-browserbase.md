--- 
type: server
repo_url: https://github.com/browserbase/mcp-server-browserbase
name: Browserbase MCP Server
owner: browserbase
stars: 156
last_updated: 2025-03-01
status: active
official: false
verified: true
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/automation",
    "integration/puppeteer",
    "integration/stagehand",
    "purpose/browser-automation",
  ]
---

# Browserbase MCP Server

#status/active #category/automation #integration/puppeteer #integration/stagehand #purpose/browser-automation

## Description

This server provides cloud browser automation capabilities using Browserbase, Puppeteer, and Stagehand. This server enables LLMs to interact with web pages, take screenshots, and execute JavaScript in a cloud browser environment.

## Features

- Cloud browser automation
- Puppeteer integration
- Stagehand support
- Web page interaction
- Screenshot capture
- JavaScript execution
- Cloud environment
- Browser management

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
        "BROWSERBASE_API_KEY": "your-api-key",
        "CLOUD_REGION": "us-east-1",
        "BROWSER_TYPE": "chrome",
        "CONCURRENT_SESSIONS": "5"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Browserbase account
- API credentials
- Cloud access

## Related Servers

- hrmeetsingh/mcp-browser-automation
- Saik0s/mcp-browser-use
- JovaniPink/mcp-browser-use