---
type: server
repo_url: https://github.com/modelcontextprotocol/servers/src/puppeteer
name: Puppeteer
owner: modelcontextprotocol
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
tags:
  [
    "category/web-scraping",
    "status/official",
    "purpose/development",
    "tech/typescript",
  ]
---

# Puppeteer

#category/web-scraping #status/official #purpose/development #tech/typescript

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
