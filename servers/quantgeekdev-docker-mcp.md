---
type: server
repo_url: https://github.com/QuantGeekDev/docker-mcp
name: Docker MCP
owner: QuantGeekDev
stars: 73
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_010.md"]
tags:
  [
    "status/active",
    "category/containerization",
    "integration/docker",
    "purpose/container-management",
    "integration/claude",
    "tech/compose",
  ]
---

# Docker MCP

#status/active #category/containerization #integration/docker #purpose/container-management #integration/claude #tech/compose

## Description

A powerful Model Context Protocol (MCP) server for Docker operations, enabling seamless container and compose stack management through Claude AI.

## Features

- Docker container management
- Docker Compose stack operations
- Container health monitoring
- Resource usage tracking
- Network configuration
- Volume management
- Image handling
- Service scaling
- Log management
- AI-assisted container operations

## Installation

```bash
npm install @quantgeekdev/docker-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "docker": {
      "command": "npx",
      "args": ["@quantgeekdev/docker-mcp"],
      "env": {
        "DOCKER_HOST": "unix:///var/run/docker.sock",
        "COMPOSE_PROJECT_NAME": "my-project",
        "CLAUDE_API_KEY": "your-claude-api-key"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Docker Engine
- Docker Compose
- Claude API access
- Docker socket access

## Related Servers

- [Docker MCP Server](https://github.com/ckreiling/mcp-server-docker) - Python-based Docker management
