---
type: server
repo_url: https://github.com/mario-andreschak/mcp-abap-abap-adt-api
name: ABAP ADT API MCP Server
owner: mario-andreschak
stars: 2
last_updated: 2025-02-20
status: active
official: false
verified: false
sources: ["inbox/batch_001.md"]
tags: ["status/active", "category/development", "integration/sap", "tech/abap", "purpose/code-review"]
---

# ABAP ADT API MCP Server

#status/active #category/development #integration/sap #tech/abap #purpose/code-review

## Description

An MCP server that integrates with ABAP Development Tools (ADT) API to enable automated code reviews, intelligent transport management, and AI-assisted ABAP development.

## Features

- Automated ABAP code reviews
- Intelligent transport management
- AI-assisted ABAP development
- Integration with SAP systems via ADT
- Code analysis capabilities

## Installation

```bash
npm install @mario-andreschak/mcp-abap-abap-adt-api
```

## Usage

```javascript
{
  "mcpServers": {
    "abap-adt": {
      "command": "npx",
      "args": ["@mario-andreschak/mcp-abap-abap-adt-api"],
      "env": {
        "SAP_HOST": "your-sap-host",
        "SAP_CLIENT": "your-client-number",
        "SAP_USER": "your-username",
        "SAP_PASSWORD": "your-password"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- SAP NetWeaver >= 7.50
- ABAP Development Tools

## Related Servers

- mario-andreschak/mcp-abap-adt