---
type: server
repo_url: https://github.com/tatn/mcp-server-fetch-python
name: Fetch Python MCP Server
owner: tatn
stars: 3
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_012.md"]
tags:
  [
    "status/active",
    "category/web",
    "tech/python",
    "purpose/content-fetching",
    "purpose/format-conversion",
    "tech/transformation",
  ]
---

# Fetch Python MCP Server

#status/active #category/web #tech/python #purpose/content-fetching #purpose/format-conversion #tech/transformation

## Description

An MCP server for fetching and transforming web content into various formats, providing flexible content retrieval and conversion capabilities.

## Features

- Web content fetching
- Format transformation
- Multiple format support
- Content validation
- Error handling
- Response formatting
- Cache management
- Format detection
- Content cleaning
- Rate limiting

## Installation

```bash
pip install mcp-server-fetch-python
```

## Usage

```javascript
{
  "mcpServers": {
    "fetch-python": {
      "command": "python",
      "args": ["-m", "mcp_server_fetch_python"],
      "env": {
        "DEFAULT_FORMAT": "markdown",
        "CACHE_TTL": "3600",
        "MAX_RETRIES": "3",
        "TIMEOUT": "30"
      }
    }
  }
}
```

## Dependencies

- Python >= 3.7
- Requests library
- BeautifulSoup4
- Format converters
- Cache system

## Related Servers

- [Fetch](https://github.com/modelcontextprotocol/servers/tree/main/src/fetch) - Official fetch implementation
- [Fetch Typescript](https://github.com/tatn/mcp-server-fetch-typescript) - TypeScript version
