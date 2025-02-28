---
type: server
repo_url: https://github.com/Bigsy/Clojars-MCP-Server
name: Clojars MCP Server
owner: Bigsy
stars: 2
last_updated: 2025-02-18
status: active
official: false
verified: false
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/package-management",
    "tech/clojure",
    "purpose/dependencies",
    "integration/clojars",
    "purpose/library-management",
  ]
---

# Clojars MCP Server

#status/active #category/package-management #tech/clojure #purpose/dependencies #integration/clojars #purpose/library-management

## Description

Provides up to date dependency information of Clojure libraries. This MCP server enables access to Clojars repository data for managing and tracking Clojure package dependencies.

## Features

- Dependency tracking
- Version information
- Library search
- Update notifications
- Compatibility checking
- Artifact resolution
- Metadata access
- Release tracking
- Security alerts
- Analytics support

## Installation

```bash
npm install @bigsy/clojars-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "clojars": {
      "command": "npx",
      "args": ["@bigsy/clojars-mcp"],
      "env": {
        "CLOJARS_MIRROR": "https://clojars.org",
        "UPDATE_INTERVAL": "3600",
        "CACHE_TTL": "86400",
        "MAX_VERSIONS": "10",
        "NOTIFY_UPDATES": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Clojars API access
- Cache system
- Version parser
- Update notifier
- Metadata parser

## Related Servers

- hugoduncan/mcp-clj
- bmorphism-babashka-mcp-server
- modelcontextprotocol-package-server
