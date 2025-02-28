---
type: server
repo_url: https://github.com/ckreiling/mcp-server-docker
name: Docker MCP Server
owner: ckreiling
stars: 50
last_updated: 2025-02-19
status: active
official: false
verified: false
sources: ["inbox/batch_010.md"]
tags: ["status/active", "category/containerization", "integration/docker", "tech/python", "purpose/container-management", "tech/sdk"]
---

# Docker MCP Server

#status/active #category/containerization #integration/docker #tech/python #purpose/container-management #tech/sdk

## Description

Manage Docker containers, bridged by the Docker SDK for Python. Provides comprehensive container management capabilities through a Model Context Protocol interface.

## Features

- Container lifecycle management
- Image management
- Volume management
- Network configuration
- Container health monitoring
- Resource usage tracking
- Log access and management
- Environment configuration
- Port mapping
- Docker compose integration

## Installation

```bash
pip install mcp-server-docker
```

## Usage

```javascript
{
  "mcpServers": {
    "docker": {
      "command": "python",
      "args": ["-m", "mcp_server_docker"],
      "env": {
        "DOCKER_HOST": "unix:///var/run/docker.sock",
        "DOCKER_API_VERSION": "1.41",
        "MAX_CONTAINERS": "50"
      }
    }
  }
}
```

## Dependencies

- Python >= 3.7
- Docker Engine
- Docker SDK for Python
- Docker Compose (optional)
- Docker socket access

## Related Servers

- None currently listed