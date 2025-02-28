---
type: server
repo_url: https://github.com/compiledwithproblems/file-context-mcp
name: File Context MCP Server
owner: compiledwithproblems
stars: 1
last_updated: 2025-02-07
status: active
official: false
verified: false
sources: ["inbox/batch_012.md"]
tags: ["status/active", "category/llm", "purpose/context-management", "purpose/file-querying", "tech/multi-model", "purpose/file-analysis"]
---

# File Context MCP Server

#status/active #category/llm #purpose/context-management #purpose/file-querying #tech/multi-model #purpose/file-analysis

## Description

This server provides an API to query Large Language Models using context from local files, supporting various models and file types for context-aware responses.

## Features

- LLM integration
- File context management
- Multi-model support
- File type handling
- Context-aware queries
- Response generation
- File analysis
- Context optimization
- Model selection
- Query processing

## Installation

```bash
npm install @compiledwithproblems/file-context-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "file-context": {
      "command": "npx",
      "args": ["@compiledwithproblems/file-context-mcp"],
      "env": {
        "DEFAULT_MODEL": "gpt-4",
        "MAX_CONTEXT_LENGTH": "8000",
        "ALLOWED_FILE_TYPES": "txt,md,json,yaml",
        "CACHE_ENABLED": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- LLM API access
- File system access
- Text processing libraries
- Cache system

## Related Servers

- [File Context Server](https://github.com/bsmi021/mcp-file-context-server) - Alternative file context implementation