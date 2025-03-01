--- 
type: server
repo_url: https://github.com/modelcontextprotocol/servers
name: Puppeteer
owner: modelcontextprotocol
stars: 11500
last_updated: 2025-02-28
status: active
official: true
verified: true
sources: ["inbox"]
tags:
  [
    "category/web-scraping",
    "status/official",
    "purpose/development",
    "tech/typescript",
  ]
---

#category/web-scraping #status/official #purpose/development #tech/typescript

# Puppeteer

## Description

A reference MCP server that provides browser automation and web scraping capabilities using Puppeteer. This server enables programmatic control of a Chrome/Chromium browser instance.

## Features

- Browser automation
- Page navigation and interaction
- Screenshot capture
- PDF generation
- Network request interception
- DOM manipulation
- Performance monitoring

## Installation

```bash
npm install @modelcontextprotocol/puppeteer-server
```

## Usage

```javascript
import { Server } from "@modelcontextprotocol/sdk/server";
import { PuppeteerServer } from "@modelcontextprotocol/puppeteer-server";

const server = new PuppeteerServer({
  headless: true,
});
server.run();
```

## Dependencies

- @modelcontextprotocol/sdk
- puppeteer
- TypeScript

## Related Servers

- Fetch Server - For simple web content retrieval
- Memory Server - For caching scraped data