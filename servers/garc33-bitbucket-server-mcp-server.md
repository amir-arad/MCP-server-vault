---
type: server
repo_url: https://github.com/garc33/bitbucket-server-mcp-server
name: Bitbucket Server MCP Server
owner: garc33
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/version-control",
    "integration/bitbucket",
    "purpose/code-review",
    "tech/javascript",
  ]
---

# Bitbucket Server MCP Server

#status/active #category/version-control #integration/bitbucket #purpose/code-review

## Description

Facilitates interaction with Bitbucket Server for pull request management using the MCP protocol, supporting operations such as creating, merging, commenting, and reviewing pull requests.

## Features

- Pull request management
- Code review tools
- Comment handling
- Merge operations
- Review workflows
- Branch management
- Conflict resolution
- Status tracking

## Installation

```bash
npm install @garc33/bitbucket-server-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "bitbucket": {
      "command": "npx",
      "args": ["@garc33/bitbucket-server-mcp"],
      "env": {
        "BITBUCKET_URL": "https://your-bitbucket-server",
        "BITBUCKET_USERNAME": "your-username",
        "BITBUCKET_PASSWORD": "your-password",
        "DEFAULT_PROJECT": "your-project"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Bitbucket Server instance
- Authentication credentials
- Project permissions

## Related Servers

- None currently listed
