---
type: server
repo_url: https://github.com/westsideori/cursor-a11y-mcp
name: Cursor Accessibility MCP Server
owner: westsideori
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_008.md"]
tags:
  [
    "status/active",
    "category/accessibility",
    "tech/puppeteer",
    "purpose/testing",
    "tech/wcag",
    "purpose/compliance",
    "tech/javascript",
    "tech/axe-core",
    "tech/react",
    "purpose/automation"
  ]
---

# Cursor Accessibility MCP Server

#status/active #category/accessibility #tech/puppeteer #purpose/testing #tech/wcag #purpose/compliance #tech/javascript #tech/axe-core #tech/react #purpose/automation

## Description

A JavaScript-based MCP server that provides automated accessibility testing capabilities through a command-line interface. The server uses axe-core and Puppeteer to perform comprehensive WCAG compliance checks on web applications, generating detailed violation reports and remediation suggestions.

## Features

- WCAG compliance testing
- Automated accessibility checks
- Detailed violation reporting
- Impact level assessment
- Issue descriptions
- Documentation links
- Element identification
- Failure summaries
- Screenshot capture
- HTML analysis
- React integration
- Local testing support
- Custom URL testing
- Remediation guidance

## Installation

```bash
# Install main dependencies
npm install

# Install test site dependencies
cd test-site
npm install
cd ..

# Build and start
npm run build
npm start
```

## Usage

```javascript
// Configuration
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

// Example Test URL
http://localhost:5000/test-page
```

## Dependencies

- Node.js >= 16
- Puppeteer ^24.1.1
- axe-core
- React ^18.2.0
- React DOM ^18.2.0
- MCP SDK ^1.4.1
- Zod ^3.24.1
- HTML analyzer
- Screenshot tool
- Report generator
- WCAG test suite

## Related Servers

- justasmonkev-mcp-accessibility-scanner
- modelcontextprotocol-testing-server
- modelcontextprotocol-accessibility-server
- buga-luga-cursor-mcp