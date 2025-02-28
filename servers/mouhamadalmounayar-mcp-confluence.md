---
type: server
repo_url: https://github.com/mouhamadalmounayar/mcp-confluence
name: Confluence Slash Commands MCP Server
owner: mouhamadalmounayar
stars: 9
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
    "purpose/slash-commands",
    "integration/zed",
    "purpose/context",
    "tech/typescript",
    "tech/nodejs"
  ]
---

# Confluence Slash Commands MCP Server

#status/active #category/productivity #integration/confluence #purpose/slash-commands #integration/zed #purpose/context #tech/typescript #tech/nodejs

## Description

A model context server that provides prompts that can be used as slash commands for clients like Zed Editor, in order to add page contents as context to the AI assistant. The server enables seamless integration between Confluence pages and AI tools through slash commands.

## Features

- Slash commands for Confluence integration
- Context integration with AI assistants
- Confluence page and blog post access
- Page content retrieval and formatting
- Command suggestions and auto-completion
- Context management and caching
- Editor integration (Zed)
- Content formatting and parsing
- Search capabilities
- Permission handling and authentication

## Installation

```bash
npm install @mouhamadalmounayar/mcp-confluence
```

## Usage

```javascript
{
  "mcpServers": {
    "confluence-commands": {
      "command": "npx",
      "args": ["@mouhamadalmounayar/mcp-confluence"],
      "env": {
        "CONFLUENCE_URL": "your-confluence-url",
        "CONFLUENCE_TOKEN": "your-api-token",
        "SPACE_KEY": "your-space",
        "COMMAND_PREFIX": "/",
        "CACHE_TTL": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Confluence API access token
- Command parser
- Context manager
- Content formatter
- Permission handler

## Related Servers

- aaronsb/confluence-cloud-mcp
- zereight/confluence-mcp
- ks-gen-ai/confluence-mcp-server