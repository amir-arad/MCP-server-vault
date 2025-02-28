---
type: server
repo_url: https://github.com/Automata-Labs-team/code-sandbox-mcp
name: Code Sandbox MCP Server
owner: Automata-Labs-team
stars: 17
last_updated: 2025-02-20
status: active
official: false
verified: false
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/security",
    "tech/docker",
    "purpose/sandbox",
    "purpose/code-execution",
    "tech/containerization",
  ]
---

# Code Sandbox MCP Server

#status/active #category/security #tech/docker #purpose/sandbox #purpose/code-execution #tech/containerization

## Description

An MCP server to create secure code sandbox environment for executing code within Docker containers. This server provides isolated and controlled environments for safe code execution.

## Features

- Secure sandboxing
- Docker integration
- Resource limiting
- Environment isolation
- Code execution
- Output capture
- Security policies
- Container management
- Cleanup automation
- Access control

## Installation

```bash
npm install @automata-labs/code-sandbox-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "code-sandbox": {
      "command": "npx",
      "args": ["@automata-labs/code-sandbox-mcp"],
      "env": {
        "DOCKER_HOST": "unix:///var/run/docker.sock",
        "MAX_MEMORY": "512m",
        "CPU_LIMIT": "1.0",
        "TIMEOUT": "30",
        "NETWORK_ACCESS": "none"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Docker Engine
- Container runtime
- Security modules
- Resource monitor
- Network isolator

## Related Servers

- modelcontextprotocol-docker-server
- toowiredd/chatgpt-mcp-server
- wonderwhy-er-claudecomputercommander
