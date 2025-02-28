---
type: server
repo_url: https://github.com/keturiosakys/bluesky-context-server
name: Bluesky Context Server
owner: keturiosakys
stars: 10
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/social-media",
    "integration/bluesky",
    "purpose/query",
    "category/context",
  ]
---

# Bluesky Context Server

#status/active #category/social-media #integration/bluesky #purpose/query #category/context

## Description

A simple MCP server that allows Claude Desktop to query Bluesky instances.

## Features

- Bluesky instance querying
- Claude Desktop integration
- Data retrieval
- Context analysis
- Feed monitoring
- User lookup
- Content search
- Real-time updates

## Usage

### Installing via Smithery

To install Bluesky Context Server for Claude Desktop automatically via [Smithery](https://smithery.ai/server/@laulauland/bluesky-context-server):

```bash
npx -y @smithery/cli install @laulauland/bluesky-context-server --client claude
```

### Installing manually

1.  Place the code somewhere on your computer.
2.  Configure your Claude Desktop app to use the MCP server.

```json
// ~/Library/Application Support/Claude/config.json
{
  "mcpServers": {
    "bluesky": {
      "command": "/Users/laurynas-fp/.bun/bin/bun",
      "args": ["<path_to_this_directory>/bluesky-context-server/index.ts"],
      "env": {
        "BLUESKY_APP_KEY": "",
        "BLUESKY_IDENTIFIER": ""
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Bluesky account
- Claude Desktop
- API access

## Related Servers

- morinokami/mcp-server-bluesky
- laulauland/bluesky-context-server
- berlinbra/BlueSky-MCP
