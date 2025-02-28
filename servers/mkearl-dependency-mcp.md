---
type: server
repo_url: https://github.com/mkearl/dependency-mcp
name: Dependency Management MCP Server
owner: mkearl
stars: 5
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_009.md"]
tags:
  [
    "status/active",
    "category/development",
    "purpose/dependency-management",
    "purpose/analysis",
    "tech/caching",
    "purpose/tracking",
  ]
---

# Dependency Management MCP Server

#status/active #category/development #purpose/dependency-management #purpose/analysis #tech/caching #purpose/tracking

## Description

A Model Context Protocol (MCP) server that analyzes codebases to generate dependency graphs and architectural insights. This server helps understand code structure, dependencies, and architectural patterns across multiple programming languages, offering caching and flexible configuration for efficient tracking across complex software ecosystems.

## Features

- **Multi-Language Support**: Analyzes dependencies in TypeScript, JavaScript, C#, Python, and more
- **Dependency Graph Generation**: Creates detailed dependency graphs in JSON or DOT format
- **Architectural Analysis**: Infers architectural layers and validates against rules
- **File Metadata**: Extracts imports, exports, and other metadata from source files
- **Scoring System**: Evaluates codebase against architectural rules and patterns
- Dependency tracking
- Analysis tools
- Cache management
- Configuration options
- Version control
- Update checking
- Conflict detection
- Security scanning
- Report generation
- Ecosystem support

## Commands

- `analyze_dependencies`: Analyzes dependencies in a codebase and generates a dependency graph.
- `get_dependency_graph`: Gets the dependency graph for a codebase in JSON or DOT format.
- `get_file_metadata`: Gets detailed metadata about a specific file.
- `get_architectural_score`: Scores the codebase against architectural rules and patterns.

## Installation

```bash
npm install @mkearl/dependency-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "dependency-mgmt": {
      "command": "npx",
      "args": ["@mkearl/dependency-mcp"],
      "env": {
        "CACHE_PATH": "./dep-cache",
        "CACHE_TTL": "86400",
        "SCAN_INTERVAL": "3600",
        "ECOSYSTEMS": "npm,pip,maven",
        "SECURITY_CHECK": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Package managers
- Cache system
- Analysis tools
- Security scanner
- Report generator
