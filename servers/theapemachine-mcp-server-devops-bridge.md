---
type: server
repo_url: https://github.com/TheApeMachine/mcp-server-devops-bridge
name: Azure DevOps Bridge MCP Server
owner: TheApeMachine
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_009.md"]
tags:
  [
    "status/active",
    "category/devops",
    "integration/azure-devops",
    "purpose/project-management",
    "purpose/automation",
    "purpose/wiki",
  ]
---

To install Azure DevOps Bridge MCP Server for Claude Desktop automatically via [Smithery](https://smithery.ai/server/@TheApeMachine/mcp-server-devops-bridge):

```bash
npx -y @smithery/cli install @TheApeMachine/mcp-server-devops-bridge --client claude
```

# Azure DevOps Bridge MCP Server

#status/active #category/devops #integration/azure-devops #purpose/project-management #purpose/automation #purpose/wiki

## Description

Integrates with Azure DevOps to manage work items, wikis, and project tasks, enabling AI-driven project management and cross-service automation.

## Features

- Work item management
- Wiki integration
- Task tracking
- Project automation
- Cross-service sync
- Status updates
- Sprint planning
- Report generation
- Pipeline control
- Team collaboration

## Installation

```bash
npm install @theapemachine/devops-bridge-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "devops-bridge": {
      "command": "npx",
      "args": ["@theapemachine/devops-bridge-mcp"],
      "env": {
        "AZURE_PAT": "your-personal-access-token",
        "ORGANIZATION": "your-org",
        "PROJECT": "your-project",
        "SYNC_INTERVAL": "300",
        "WIKI_ENABLED": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Azure DevOps access
- API credentials
- Task manager
- Wiki processor
- Report generator

## Related Servers

- stefanskiasan-azure-devops-mcp-server
- modelcontextprotocol-azure-server
- modelcontextprotocol-devops-server
