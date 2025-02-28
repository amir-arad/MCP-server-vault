---
type: server
repo_url: https://github.com/Sunwood-ai-labs/documind-mcp-server
name: Documind MCP Server
owner: Sunwood-ai-labs
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_010.md"]
tags:
  [
    "status/active",
    "category/documentation",
    "category/ai",
    "purpose/project-analysis",
    "purpose/workflow-guidance",
    "tech/filesystem",
  ]
---

# Documind MCP Server

#status/active #category/documentation #category/ai #purpose/project-analysis #purpose/workflow-guidance #tech/filesystem

## Description

Parses through README documentation/project files on your local filesystem to guide development workflows. Provides intelligent analysis and insights from project documentation.

## Features

- README file parsing
- Project file analysis
- Development workflow guidance
- Documentation indexing
- Content organization
- Search capabilities
- Context-aware suggestions
- Project structure analysis
- Dependency tracking
- Documentation quality checks

## Installation

```bash
npm install @sunwood-ai-labs/documind-mcp-server
```

## Usage

```javascript
{
  "mcpServers": {
    "documind": {
      "command": "npx",
      "args": ["@sunwood-ai-labs/documind-mcp-server"],
      "env": {
        "PROJECT_ROOT": "./",
        "SCAN_DEPTH": "3",
        "IGNORE_PATTERNS": "node_modules,dist,build"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- File system access
- Search indexing engine
- Natural language processing libraries
- Project analysis tools

## Related Servers

- None currently listed
