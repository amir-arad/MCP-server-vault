---
type: server
repo_url: https://github.com/modelcontextprotocol/servers/tree/main/src/everything
name: Everything MCP Server
owner: modelcontextprotocol
stars: 9794
last_updated: 2025-02-21
status: active
official: true
verified: true
sources: ["inbox/batch_011.md"]
tags: ["status/active", "status/official", "status/verified", "category/reference", "purpose/testing", "purpose/development"]
---

# Everything MCP Server

#status/active #status/official #status/verified #category/reference #purpose/testing #purpose/development

## Description

Reference / test server with prompts, resources, and tools, serving as a comprehensive example implementation and testing ground for MCP functionality.

## Features

- Reference implementation
- Test resources
- Tool examples
- Prompt templates
- Resource management
- Testing utilities
- Documentation examples
- Development aids
- Integration patterns
- Best practices

## Installation

```bash
npm install @modelcontextprotocol/everything
```

## Usage

```javascript
{
  "mcpServers": {
    "everything": {
      "command": "npx",
      "args": ["@modelcontextprotocol/everything"],
      "env": {
        "TEST_MODE": "true",
        "LOG_LEVEL": "debug",
        "RESOURCE_DIR": "./resources",
        "PROMPT_DIR": "./prompts"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- MCP SDK
- Testing frameworks
- Resource files
- Documentation tools

## Related Servers

- None currently listed