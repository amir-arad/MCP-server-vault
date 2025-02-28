---
type: server
repo_url: https://github.com/dillip285/mcp-dev-server
name: Development Tools MCP Server
owner: dillip285
stars: 0
last_updated: 2024-12-15
status: active
official: false
verified: false
sources: ["inbox/batch_009.md"]
tags:
  [
    "status/active",
    "category/development",
    "integration/docker",
    "integration/git",
    "purpose/project-management",
    "purpose/automation",
  ]
---

# Development Tools MCP Server

#status/active #category/development #integration/docker #integration/git #purpose/project-management #purpose/automation

## Description

Integrates with Docker, Git, and development tools to enable software project management, code analysis, and automated workflows across languages and frameworks.

## Features

- Docker integration
- Git operations
- Project management
- Code analysis
- Workflow automation
- Build processes
- Deployment support
- Version control
- Environment management
- Tool orchestration

## Installation

```bash
npm install @dillip285/mcp-dev-server
```

## Usage

```javascript
{
  "mcpServers": {
    "dev-tools": {
      "command": "npx",
      "args": ["@dillip285/mcp-dev-server"],
      "env": {
        "DOCKER_HOST": "unix:///var/run/docker.sock",
        "GIT_PATH": "/usr/bin/git",
        "WORKSPACE_ROOT": "./workspace",
        "AUTO_BUILD": "true",
        "LOG_LEVEL": "info"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Docker Engine
- Git
- Build tools
- Code analyzers
- Process manager

## Related Servers

- modelcontextprotocol-docker-server
- modelcontextprotocol-git-server
- modelcontextprotocol-development-server
