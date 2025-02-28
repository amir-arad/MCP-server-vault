---
type: server
repo_url: https://github.com/ExactDoug/mcp-fetch
name: Fetch MCP Server
owner: ExactDoug
stars: 1
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_011.md"]
tags:
  [
    "status/active",
    "category/web",
    "purpose/content-retrieval",
    "purpose/html-conversion",
    "tech/markdown",
    "category/llm",
    "tech/python"
  ]
---

# Fetch MCP Server

#status/active #category/web #purpose/content-retrieval #purpose/html-conversion #tech/markdown #category/llm #tech/python

## Description

A Python-based MCP server that provides web content fetching capabilities, optimized for LLMs. The server retrieves and processes content from web pages, converting HTML to markdown for easier consumption by language models, with support for content truncation and pagination.

## Features

- Web content retrieval
- HTML to Markdown conversion
- Content truncation
- Pagination support
- LLM optimization
- Content cleaning
- Link processing
- Image handling
- Error management
- Cache control
- Start index support
- UV installation support
- PIP installation support

## Installation

```bash
# Using uv (recommended)
uvx pip install mcp-server-fetch

# Using PIP
pip install mcp-server-fetch
```

## Usage

```javascript
{
  "mcpServers": {
    "fetch": {
      "command": "uvx",
      "args": ["mcp-server-fetch"],
      "env": {
        "MAX_CONTENT_LENGTH": "50000",
        "PAGE_SIZE": "1000",
        "CACHE_TTL": "3600",
        "CLEAN_HTML": "true"
      }
    }
  }
}

// Available Tools
fetch:
  - url: URL to fetch
  - max_length: Max characters to return
  - start_index: Character index to start from
  - raw: Get raw content (boolean)
```

## Dependencies

- Python 3.7+
- uv or PIP
- HTML parser
- Markdown converter
- Cache system
- Network connectivity

## Related Servers

- zcaceres/fetch-mcp
- modelcontextprotocol/fetch-server