---
type: server
repo_url: https://github.com/bsmi021/mcp-file-context-server
name: File Context MCP Server
owner: bsmi021
stars: 1
last_updated: 2025-01-30
status: active
official: false
verified: false
sources: ["inbox/batch_012.md"]
tags: ["status/active", "category/development", "purpose/file-access", "purpose/code-analysis", "purpose/quality-assessment", "purpose/navigation"]
---

# File Context MCP Server

#status/active #category/development #purpose/file-access #purpose/code-analysis #purpose/quality-assessment #purpose/navigation

## Description

Provides advanced file system access and code analysis capabilities, enabling efficient reading, searching, and analysis of large codebases for automated quality assessment and intelligent navigation.

## Features

- File system access
- Code analysis
- Quality assessment
- Intelligent navigation
- Search capabilities
- Pattern detection
- Metrics collection
- Code structure analysis
- Documentation parsing
- Performance monitoring

## Installation

```bash
npm install @bsmi021/mcp-file-context-server
```

## Usage

```javascript
{
  "mcpServers": {
    "file-context": {
      "command": "npx",
      "args": ["@bsmi021/mcp-file-context-server"],
      "env": {
        "ROOT_DIR": "./src",
        "IGNORE_PATTERNS": "node_modules,dist,build",
        "MAX_FILE_SIZE": "10485760",
        "ANALYSIS_DEPTH": "3"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Code analysis tools
- File system access
- Search indexing
- Metrics collector

## Related Servers

- [File Context MCP](https://github.com/compiledwithproblems/file-context-mcp) - LLM-based file context analysis