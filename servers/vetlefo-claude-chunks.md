---
type: server
repo_url: https://github.com/vetlefo/claude-chunks
name: Claude Chunks MCP Server
owner: vetlefo
stars: 7
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/ai",
    "integration/claude",
    "purpose/document-processing",
    "purpose/summarization",
    "tech/typescript",
  ]
---

To install Claude Chunks MCP Server for Claude Desktop automatically via [Smithery](https://smithery.ai/server/@vetlefo/claude-chunks):

```bash
npx -y @smithery/cli install @vetlefo/claude-chunks --client claude
```

# Claude Chunks MCP Server

#status/active #category/ai #integration/claude #purpose/document-processing #purpose/summarization #tech/typescript

## Description

An MCP server that intelligently chunks large documents for Claude, enabling efficient context-aware processing and summary generation for enhanced document comprehension.

## Features

- Smart document chunking
- Context preservation
- Summary generation
- Token optimization
- Chunk overlap management
- Metadata handling
- Processing pipeline
- Progress tracking
- Error recovery
- Format support

## Installation

```bash
npm install @vetlefo/claude-chunks
```

## Usage

```javascript
{
  "mcpServers": {
    "claude-chunks": {
      "command": "npx",
      "args": ["@vetlefo/claude-chunks"],
      "env": {
        "MAX_CHUNK_SIZE": "8000",
        "OVERLAP_SIZE": "500",
        "MIN_CHUNK_SIZE": "1000",
        "PRESERVE_HEADERS": "true",
        "OUTPUT_FORMAT": "markdown"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Claude API access
- Text processing libraries
- Document parser
- Token counter
- Format converter

## Related Servers

- modelcontextprotocol-memory-server
- shin-t-o-mcp-access
- chatmcp/mcp-server-chatsum
