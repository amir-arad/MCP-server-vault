--- 
type: server
repo_url: https://github.com/daipendency/daipendency-mcp
name: Daipendency Documentation MCP Server
owner: daipendency
stars: 35
last_updated: 2025-03-01
status: active
official: true
verified: true
sources: ["inbox/batch_008.md"]
tags:
  [
    "status/active",
    "status/official",
    "category/documentation",
    "tech/rust",
    "purpose/dependency-docs",
    "purpose/api-docs",
  ]
---

# Daipendency Documentation MCP Server

#status/active #status/official #category/documentation #tech/rust #purpose/dependency-docs #purpose/api-docs

## Description

Get the narrative and API documentation for the exact version of any of your dependencies. Only Rust is supported at the moment, providing precise documentation access for Rust crates.

## Features

- Version-specific docs
- API documentation
- Narrative content
- Rust crate support
- Documentation search
- Version matching
- Content caching
- Example code
- Type information
- Offline access

## Installation

```bash
npm install @daipendency/daipendency-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "daipendency": {
      "command": "npx",
      "args": ["@daipendency/daipendency-mcp"],
      "env": {
        "CARGO_HOME": "~/.cargo",
        "DOCS_CACHE": "./doc-cache",
        "CACHE_TTL": "86400",
        "MAX_VERSIONS": "5",
        "OFFLINE_MODE": "false"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Rust toolchain
- Cargo package manager
- Documentation parser
- Cache system
- Search indexer