---
type: server
repo_url: https://github.com/stevennevins/architect-mcp-server
name: Architect MCP Server Template
owner: stevennevins
stars: 5
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/development", "tech/typescript", "purpose/architecture", "category/template", "integration/llm-cli"]
---

# Architect MCP Server Template

#status/active #category/development #tech/typescript #purpose/architecture #category/template #integration/llm-cli

## Description

A template for creating Model Context Protocol (MCP) servers in TypeScript, offering features like container-based dependency injection, a service-based architecture, and integration with the LLM CLI for architectural design feedback through natural language. This template provides a structured foundation for building MCP servers with built-in testing tools and debugging capabilities.

## Features

- TypeScript-based MCP server template
- Integration with LLM CLI for architectural design feedback
- Conversation context management across multiple interactions
- Built-in TestClient for local testing
- MCP Inspector for visual debugging
- Dependency injection system
- Service-based architecture
- Hot reload development environment
- Comprehensive testing framework
- Local testing with Cursor integration

## Installation

```bash
# Clone the repository
git clone https://github.com/stevennevins/architect-mcp-server.git
cd architect-mcp-server

# Install dependencies
npm install

# Build the project
npm run build

# Link for local testing
npm run link
```

## Usage

```javascript
{
  "mcpServers": {
    "architect-template": {
      "command": "npx",
      "args": ["architect-mcp-server"],
      "env": {
        "LLM_MODEL": "gpt-4",
        "LOG_LEVEL": "info"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- TypeScript >= 4.5
- LLM CLI (installable via `brew install llm`)
- MCP Inspector for debugging (optional)

## Related Servers

- squirrelogic/mcp-architect - Similar architecture-focused MCP server
- stevennevins/mcp-server-template - Base template used by this project
- modelcontextprotocol/servers - Official MCP server implementations