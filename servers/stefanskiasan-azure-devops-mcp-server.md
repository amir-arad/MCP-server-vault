---
type: server
repo_url: https://github.com/stefanskiasan/azure-devops-mcp-server
name: Azure DevOps MCP Server
owner: stefanskiasan
stars: 5
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_003.md"]
tags: ["status/active", "category/devops", "integration/azure", "integration/azure-devops", "purpose/development", "tech/typescript", "tech/nodejs"]
---

# Azure DevOps MCP Server

#status/active #category/devops #integration/azure #integration/azure-devops #purpose/development #tech/typescript #tech/nodejs

## Description

A Model Context Protocol (MCP) server that provides integration with Azure DevOps services, allowing Cline to interact with work items, boards, pipelines, pull requests, wikis, and projects. This server enables comprehensive management of Azure DevOps resources through a standardized interface.

## Features

- Work Item Management:
  - Get work item details by ID
  - Query work items using WIQL
  - Create new work items (Bug, Task, User Story)
  - Update existing work items
- Board Management:
  - List available boards in the project
- Pipeline Operations:
  - List all pipelines in the project
  - Trigger pipeline execution
- Pull Request Handling:
  - List pull requests
  - Create new pull requests
  - Update existing pull requests
  - Get pull request details
- Wiki Management:
  - List all wikis in the project
  - Get wiki page content
  - Create new wikis
  - Create or update wiki pages
- Project Management:
  - List all projects in the Azure DevOps organization

## Installation

```bash
# Install via Smithery (recommended)
npx -y @smithery/cli install @stefanskiasan/azure-devops-mcp-server --client claude

# Or manual installation
git clone https://github.com/stefanskiasan/azure-devops-mcp-server.git
cd azure-devops-mcp-server
npm install
npm run build
```

## Usage

```javascript
{
  "mcpServers": {
    "azure-devops": {
      "command": "node",
      "args": ["/path/to/azure-devops-mcp-server/build/index.js"],
      "env": {
        "AZURE_DEVOPS_ORG": "your-organization",
        "AZURE_DEVOPS_PAT": "your-personal-access-token",
        "AZURE_DEVOPS_PROJECT": "your-project-name"
      },
      "disabled": false,
      "autoApprove": []
    }
  }
}
```

## Dependencies

- Node.js v20 LTS or higher
- Azure DevOps account
- Personal Access Token (PAT) with appropriate scopes:
  - Code (read, write) - For Pull Request operations
  - Work Items (read, write) - For Work Item management
  - Build (read, execute) - For Pipeline operations
  - Wiki (read, write) - For Wiki operations
  - Project and Team (read) - For Project and Board information

## Related Servers

- mashriram/azure_mcp_server - General Azure services integration
- ZubeidHendricks/azure-onenote-mcp-server - Microsoft OneNote integration
- dkmaker/mcp-azure-tablestorage - Azure Table Storage integration
- modelcontextprotocol/github-server - Similar integration for GitHub