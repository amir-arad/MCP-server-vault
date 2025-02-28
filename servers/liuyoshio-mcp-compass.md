---
type: server
repo_url: https://github.com/liuyoshio/mcp-compass
name: MCP Compass Server
owner: liuyoshio
stars: 11
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/discovery",
    "purpose/recommendation",
    "purpose/search",
    "category/ai",
    "purpose/understanding",
  ]
---

# MCP Compass Server

#status/active #category/discovery #purpose/recommendation #purpose/search #category/ai #purpose/understanding

## Description

MCP Compass is a discovery & recommendation service that assists AI assistants in finding and understanding Model Context Protocol servers through natural language queries.

## Features

- 🔍 **Smart Search**: Find MCP services using natural language queries
- 📚 **Rich Metadata**: Get detailed information about each service
- 🔄 **Real-time Updates**: Always up-to-date with the latest MCP services
- Server discovery
- Recommendation engine
- Natural language queries
- Server understanding
- Capability matching
- Usage suggestions
- Documentation access
- Relevance ranking
- Server comparison
- Integration guidance

## Usage

### Installation

For Claude Desktop, edit your `claude_desktop_config.json` file:

#### MacOS/Linux

```bash
code ~/Library/Application\ Support/Claude/claude_desktop_config.json
```

#### Windows

```powershell
code $env:AppData\\Claude\\claude_desktop_config.json
```

1.  **As an MCP Service**:

    Add to your AI assistant's MCP configuration to enable service discovery capabilities.

```json
{
  "mcpServers": {
    "mcp-compass": {
      "command": "npx",
      "args": ["-y", "@liuyoshio/mcp-compass"]
    }
  }
}
```

or

```json
{
  "mcpServers": {
    "mcp-compass": {
      "command": "node",
      "args": ["/path/to/repo/build/index.js"]
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Vector database
- Search engine
- NLP processor
- Recommendation system
- Documentation parser

## Related Servers

- chatmcp/mcp-server-collector
- modelcontextprotocol-discovery-server
- modelcontextprotocol-registry-server
