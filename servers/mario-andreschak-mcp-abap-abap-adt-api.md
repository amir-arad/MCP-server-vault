---
type: server
repo_url: https://github.com/mario-andreschak/mcp-abap-abap-adt-api
name: ABAP ADT API MCP Server
owner: mario-andreschak
stars: 2
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_001.md"]
tags: ["status/active", "category/development", "integration/sap", "tech/abap", "purpose/code-review", "tech/typescript", "integration/adt"]
---

# ABAP ADT API MCP Server

#status/active #category/development #integration/sap #tech/abap #purpose/code-review #tech/typescript #integration/adt

## Description

A Model Context Protocol (MCP) server designed to facilitate seamless communication between ABAP systems and MCP clients. This server wraps the abap-adt-api library to provide a comprehensive suite of tools for managing ABAP objects, handling transport requests, performing code analysis, and enhancing ABAP development workflows through AI-assisted capabilities.

## Features

- Authentication: Securely authenticate with ABAP systems
- Object Management: Create, read, update, and delete ABAP objects
- Transport Handling: Manage transport requests with tools like createTransport and transportInfo
- Code Analysis: Perform syntax checks and retrieve code completion suggestions
- Source Code Management: Get and set object source code with proper locking mechanisms
- Activation: Activate ABAP objects after modification
- Database Structure Inspection: Retrieve table and structure definitions
- Session Management: Handle session caching and termination
- Extensibility: Easily extend with additional tools and resources

## Installation

```bash
# Install via Smithery (recommended)
npx -y @smithery/cli install @mario-andreschak/mcp-abap-abap-adt-api --client claude

# Or manual installation
git clone https://github.com/mario-andreschak/mcp-abap-abap-adt-api.git
cd mcp-abap-abap-adt-api
npm install
npm run build
```

## Usage

```javascript
{
  "mcpServers": {
    "abap-adt": {
      "command": "node",
      "args": ["path/to/mcp-abap-abap-adt-api/dist/index.js"],
      "env": {
        "SAP_URL": "https://your-sap-server.com:44300",
        "SAP_USER": "your-username",
        "SAP_PASSWORD": "your-password",
        "SAP_CLIENT": "your-client-number",
        "SAP_LANGUAGE": "your-language-code"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- TypeScript
- SAP NetWeaver >= 7.50 with ADT (ABAP Development Tools) enabled
- Valid SAP credentials with appropriate permissions
- Internet connectivity to the SAP system

## Related Servers

- mario-andreschak/mcp-abap-adt - Simplified version of this server
- modelcontextprotocol/github-server - Similar pattern for GitHub integration
- stefanskiasan/azure-devops-mcp-server - Similar enterprise development integration