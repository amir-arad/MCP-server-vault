---
type: server
repo_url: https://github.com/aaronsb/confluence-cloud-mcp
name: Confluence Cloud MCP Server
owner: aaronsb
stars: 6
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/productivity",
    "integration/confluence",
    "tech/cloud",
    "purpose/content-management",
    "purpose/space-management",
    "tech/typescript",
    "tech/nodejs",
    "tech/docker"
  ]
---

# Confluence Cloud MCP Server

#status/active #category/productivity #integration/confluence #tech/cloud #purpose/content-management #purpose/space-management #tech/typescript #tech/nodejs #tech/docker

## Description

Enables AI assistants to interact with Confluence Cloud for managing spaces, pages, and content via the Model Context Protocol (MCP). Features automated content format conversion and comprehensive API integration through a standardized interface.

## Features

- Space management (list, details)
- Page operations (create, read, update)
- Content format conversion (Confluence to Markdown)
- Search functionality with CQL
- Template support
- Label management
- Permission control
- Version tracking
- Multi-architecture support (amd64, arm64)
- Automated CI/CD pipeline

## Installation

```bash
# Using Docker (Recommended)
docker run --rm -i \
  -e CONFLUENCE_API_TOKEN=your-api-token \
  -e CONFLUENCE_EMAIL=your-email@domain.com \
  -e CONFLUENCE_DOMAIN=your-domain.atlassian.net \
  ghcr.io/aaronsb/confluence-cloud-mcp:latest

# Or via npm
npm install @aaronsb/confluence-cloud-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "confluence-cloud": {
      "command": "docker",
      "args": ["run", "--rm", "-i", "ghcr.io/aaronsb/confluence-cloud-mcp:latest"],
      "env": {
        "CONFLUENCE_DOMAIN": "your-domain.atlassian.net",
        "CONFLUENCE_EMAIL": "your-email@domain.com",
        "CONFLUENCE_API_TOKEN": "your-api-token",
        "BATCH_SIZE": "50",
        "RETRY_ATTEMPTS": "3"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Docker (for containerized deployment)
- Confluence Cloud account
- API token
- TypeScript runtime
- Content processor
- Permission manager
- Version controller

## Related Servers

- mouhamadalmounayar/mcp-confluence
- zereight/confluence-mcp
- ks-gen-ai/confluence-mcp-server