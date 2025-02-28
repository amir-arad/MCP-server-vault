---
type: server
repo_url: https://github.com/JustasMonkev/mcp-accessibility-scanner
name: Accessibility Scanner MCP Server
owner: JustasMonkev
stars: 1
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_001.md"]
tags: ["status/active", "category/accessibility", "category/testing", "tech/playwright", "purpose/web-testing", "tech/typescript", "integration/axe-core"]
---

# Accessibility Scanner MCP Server

#status/active #category/accessibility #category/testing #tech/playwright #purpose/web-testing #tech/typescript #integration/axe-core

## Description

A Model Context Protocol (MCP) server for performing automated accessibility scans of web pages using Playwright and Axe-core. This server enables comprehensive WCAG compliance checking with detailed reporting and remediation guidance, helping developers and content creators identify and fix accessibility issues.

## Features

- Full WCAG 2.1/2.2 compliance checking
- Automated web accessibility scanning
- Playwright-based testing for accurate rendering
- Axe-core integration for industry-standard accessibility rules
- Automatic screenshot capture with violation highlighting
- Detailed JSON reports with remediation guidance
- Visual reports for easy issue identification
- Configurable violation tag filtering

## Installation

```bash
# Clone repository
git clone https://github.com/JustasMonkev/mcp-accessibility-scanner.git
cd mcp-accessibility-scanner

# Install dependencies
npm install

# Build project (compiles TypeScript and installs Playwright browsers)
npm run prepare
```

## Usage

```javascript
{
  "mcpServers": {
    "accessibility-checker": {
      "command": "node",
      "args": [
        "path/to/mcp-accessibility-scanner/build/server.js"
      ],
      "env": {
        "SCAN_DEPTH": "2",
        "WCAG_LEVEL": "AA",
        "REPORT_FORMAT": "json,html",
        "CONCURRENT_SCANS": "5"
      }
    }
  }
}
```

The scanner exposes a single tool `scan_accessibility` that accepts:
- `url`: The webpage URL to scan
- `violationsTag`: Array of accessibility violation tags to check

## Dependencies

- Node.js >= 16
- TypeScript
- Playwright (automatically installed during build)
- Axe-core for accessibility testing
- Chrome or Chromium browser (installed by Playwright)

## Related Servers

- modelcontextprotocol/puppeteer-server - General web automation server
- fetch-mcp-server - Web content fetching server
- bmorphism-anti-bullshit-mcp-server - Content quality analysis server