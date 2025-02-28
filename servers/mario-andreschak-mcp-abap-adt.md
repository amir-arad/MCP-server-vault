---
type: server
repo_url: https://github.com/mario-andreschak/mcp-abap-adt
name: ABAP ADT MCP Server
owner: mario-andreschak
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_001.md"]
tags:
  [
    "status/active",
    "category/development",
    "integration/sap",
    "tech/abap",
    "purpose/development",
  ]
---

# ABAP ADT MCP Server

#status/active #category/development #integration/sap #tech/abap #purpose/development

## Description

An MCP server that integrates with SAP ABAP systems via ADT (ABAP Development Tools), enabling AI models to perform ABAP development tasks like code generation and system analysis. Think of it as a bridge that lets tools like Cline (a VS Code extension) talk to your ABAP system and retrieve information like source code, table structures, and more. It's like having a remote control for your ABAP development environment!

## Features

- ABAP code generation
- System analysis capabilities
- Integration with SAP systems
- ABAP Development Tools (ADT) integration
- AI-assisted development workflows

## Installation

To install MCP ABAP Development Tools Server for Cline automatically via [Smithery](https://smithery.ai/server/@mario-andreschak/mcp-abap-adt):

```bash
npx -y @smithery/cli install @mario-andreschak/mcp-abap-adt --client cline
```

### Manual Installation

1.  Clone the Repository:

    - Using Git (command line):

      1.  Open a terminal (command prompt or Terminal).
      2.  Navigate to the directory where you want to store the project. For example, to put it on your Desktop:

          ```bash
          cd Desktop
          ```

      3.  Clone the repository:

          ```bash
          git clone https://github.com/mario-andreschak/mcp-abap-adt
          ```

      4.  Change into the project directory:

          ```bash
          cd mcp-abap-adt  # Or whatever the folder name is
          ```

    - Using GitHub Desktop:
      1.  Open GitHub Desktop.

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
