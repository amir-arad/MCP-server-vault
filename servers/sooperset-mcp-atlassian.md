---
type: server
repo_url: https://github.com/sooperset/mcp-atlassian
name: Atlassian MCP Server
owner: sooperset
stars: 83
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_003.md"]
tags:
  [
    "status/active",
    "category/productivity",
    "integration/atlassian",
    "integration/confluence",
    "integration/jira",
    "tech/python",
  ]
---

# Atlassian MCP Server

#status/active #category/productivity #integration/atlassian #integration/confluence #integration/jira

## Description

Model Context Protocol (MCP) server for Atlassian Cloud products (Confluence and Jira). This integration is designed specifically for Atlassian Cloud instances and does not support Atlassian Server or Data Center deployments.

## Features

- Confluence integration
- Jira integration
- Cloud-specific support
- Document management
- Issue tracking
- Content creation
- Search capabilities
- Permission handling

## Installation

```bash
npm install @sooperset/mcp-atlassian
```

## Usage

```javascript
{
  "mcpServers": {
    "atlassian": {
      "command": "npx",
      "args": ["@sooperset/mcp-atlassian"],
      "env": {
        "ATLASSIAN_DOMAIN": "your-domain.atlassian.net",
        "ATLASSIAN_EMAIL": "your-email",
        "ATLASSIAN_API_TOKEN": "your-api-token",
        "DEFAULT_SPACE": "TEAM"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Atlassian Cloud account
- API token
- Cloud instance access

## Related Servers

- None currently listed
