---
type: server
repo_url: https://github.com/weidwonder/crawl4ai-mcp-server
name: Crawl4AI MCP Server
owner: weidwonder
stars: 9
last_updated: 2025-02-19
status: active
official: false
verified: false
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/web-scraping",
    "category/ai",
    "purpose/information-retrieval",
    "purpose/search",
    "tech/llm",
  ]
---

# Crawl4AI MCP Server

#status/active #category/web-scraping #category/ai #purpose/information-retrieval #purpose/search #tech/llm

## Description

Crawl4AI MCP Server is an intelligent information retrieval server offering robust search capabilities and LLM-optimized web content understanding, utilizing multi-engine search and intelligent content extraction to efficiently gather and comprehend internet information.

## Features

- Intelligent crawling
- Content extraction
- LLM optimization
- Multi-engine search
- Content understanding
- Search capabilities
- Data processing
- Content analysis
- Result ranking
- Information synthesis

## Installation

```bash
npm install @weidwonder/crawl4ai-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "crawl4ai": {
      "command": "npx",
      "args": ["@weidwonder/crawl4ai-mcp"],
      "env": {
        "LLM_API_KEY": "your-llm-key",
        "CRAWL_DEPTH": "3",
        "MAX_PAGES": "1000",
        "EXTRACTION_QUALITY": "high",
        "CONCURRENT_REQUESTS": "5"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- LLM API access
- Web crawler
- Content extractor
- Search engine
- Analysis engine

## Related Servers

- modelcontextprotocol-web-scraping-server
- mendableai-firecrawl-mcp-server
- oxylabs-oxylabs-mcp
