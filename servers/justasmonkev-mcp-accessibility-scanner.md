---
type: server
repo_url: https://github.com/JustasMonkev/mcp-accessibility-scanner
name: Accessibility Scanner MCP Server
owner: JustasMonkev
stars: 1
last_updated: 2025-02-01
status: active
official: false
verified: false
sources: ["inbox/batch_001.md"]
tags: ["status/active", "category/accessibility", "category/testing", "tech/playwright", "purpose/web-testing"]
---

# Accessibility Scanner MCP Server

#status/active #category/accessibility #category/testing #tech/playwright #purpose/web-testing

## Description

Enables automated web accessibility scans for WCAG compliance using Playwright and Axe-core, providing visual and JSON reports with remediation guidance.

## Features

- Automated WCAG compliance scanning
- Playwright-based testing
- Axe-core integration
- Visual and JSON reporting
- Remediation guidance
- Batch URL processing

## Installation

```bash
npm install @justasmonkev/mcp-accessibility-scanner
```

## Usage

```javascript
{
  "mcpServers": {
    "accessibility-scanner": {
      "command": "npx",
      "args": ["@justasmonkev/mcp-accessibility-scanner"],
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

## Dependencies

- Node.js >= 16
- Playwright
- Axe-core
- Chrome or Chromium browser

## Related Servers

- None currently listed