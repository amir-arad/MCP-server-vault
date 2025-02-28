---
type: server
repo_url: https://github.com/westsideori/cursor-a11y-mcp
name: Cursor Accessibility MCP Server
owner: westsideori
stars: 0
last_updated: 2025-02-12
status: active
official: false
verified: false
sources: ["inbox/batch_008.md"]
tags:
  [
    "status/active",
    "category/accessibility",
    "tech/puppeteer",
    "purpose/testing",
    "tech/wcag",
    "purpose/compliance",
  ]
---

# Cursor Accessibility MCP Server

#status/active #category/accessibility #tech/puppeteer #purpose/testing #tech/wcag #purpose/compliance

## Description

Integrates accessibility testing capabilities using Puppeteer to perform automated WCAG compliance checks and generate remediation suggestions for web applications.

## Features

- WCAG compliance testing
- Automated checks
- Remediation suggestions
- Accessibility scanning
- Report generation
- Issue detection
- Compliance tracking
- Test automation
- Screenshot capture
- Documentation support

## Installation

```bash
npm install @westsideori/cursor-a11y-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "cursor-a11y": {
      "command": "npx",
      "args": ["@westsideori/cursor-a11y-mcp"],
      "env": {
        "WCAG_LEVEL": "AA",
        "SCAN_INTERVAL": "3600",
        "SCREENSHOT_PATH": "./screenshots",
        "REPORT_FORMAT": "html",
        "IGNORE_RULES": "none"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Puppeteer
- WCAG test suite
- Report generator
- Screenshot tool
- HTML analyzer

## Related Servers

- justasmonkev-mcp-accessibility-scanner
- modelcontextprotocol-testing-server
- modelcontextprotocol-accessibility-server
