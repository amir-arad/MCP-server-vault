---
type: server
repo_url: https://github.com/mario-andreschak/mcp-abap-adt
name: ABAP ADT MCP Server
owner: mario-andreschak
stars: 0
last_updated: 2025-02-20
status: active
official: false
verified: false
sources: ["inbox/batch_001.md"]
tags: ["status/active", "category/development", "integration/sap", "tech/abap", "purpose/development"]
---

# ABAP ADT MCP Server

#status/active #category/development #integration/sap #tech/abap #purpose/development

## Description

An MCP server that integrates with SAP ABAP systems via ADT (ABAP Development Tools), enabling AI models to perform ABAP development tasks like code generation and system analysis.

## Features

- ABAP code generation
- System analysis capabilities
- Integration with SAP systems
- ABAP Development Tools (ADT) integration
- AI-assisted development workflows

## Installation

```bash
npm install @mario-andreschak/mcp-abap-adt
```

## Usage

```javascript
{
  "mcpServers": {
    "abap-adt": {
      "command": "npx",
      "args": ["@mario-andreschak/mcp-abap-adt"],
      "env": {
        "SAP_SYSTEM_URL": "your-sap-system-url",
        "SAP_CLIENT": "your-client-number",
        "SAP_USERNAME": "your-username",
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

- mario-andreschak/mcp-abap-abap-adt-api