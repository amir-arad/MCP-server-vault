---
type: server
repo_url: https://github.com/Toowiredd/chatgpt-mcp-server
name: ChatGPT Docker Management MCP Server
owner: Toowiredd
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/devops",
    "integration/docker",
    "category/ai",
    "tech/gpt",
    "purpose/container-management",
  ]
---

To install ChatGPT Docker Management MCP Server for Claude Desktop automatically via [Smithery](https://smithery.ai/server/@Toowiredd/chatgpt-mcp-server):

```bash
npx -y @smithery/cli install @Toowiredd/chatgpt-mcp-server --client claude
```

# ChatGPT Docker Management MCP Server

#status/active #category/devops #integration/docker #category/ai #tech/gpt #purpose/container-management

## Description

A Model Context Protocol server that enables Docker container management through natural language interactions using a custom GPT interface. This server bridges the gap between natural language commands and Docker operations.

## Features

- Natural language Docker control
- Container lifecycle management
- Image management
- Volume handling
- Network configuration
- Resource monitoring
- Log analysis
- Health checks
- Environment management
- Security policy enforcement

## Installation

```bash
npm install @toowiredd/chatgpt-mcp-server
```

## Usage

```javascript
{
  "mcpServers": {
    "docker-gpt": {
      "command": "npx",
      "args": ["@toowiredd/chatgpt-mcp-server"],
      "env": {
        "OPENAI_API_KEY": "your-openai-api-key",
        "DOCKER_HOST": "unix:///var/run/docker.sock",
        "MAX_CONTAINERS": "10",
        "SECURITY_LEVEL": "high"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Docker Engine
- OpenAI API key
- Docker SDK
- GPT model access
- Security policies

## Related Servers

- modelcontextprotocol-docker-server
- pyroprompts-any-chat-completions-mcp
