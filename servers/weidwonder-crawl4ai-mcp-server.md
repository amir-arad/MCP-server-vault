---
type: server
repo_url: https://github.com/weidwonder/crawl4ai-mcp-server
name: Crawl4AI MCP Server
owner: weidwonder
stars: 17
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_007.md"]
tags:
  [
    "status/active",
    "category/web-scraping",
    "category/ai",
    "purpose/information-retrieval",
    "purpose/search",
    "tech/llm",
    "tech/python",
    "tech/fastmcp",
    "integration/duckduckgo",
    "integration/google"
  ]
---

# Crawl4AI MCP Server

#status/active #category/web-scraping #category/ai #purpose/information-retrieval #purpose/search #tech/llm #tech/python #tech/fastmcp #integration/duckduckgo #integration/google

## Description

A Python-based MCP server that provides intelligent information retrieval capabilities optimized for LLMs (Large Language Models). The server offers robust search functionality through multiple search engines (DuckDuckGo, Google) and LLM-optimized web content understanding, utilizing intelligent content extraction to efficiently gather and process internet information into formats best suited for LLM processing.

## Features

- Multi-engine search support (DuckDuckGo, Google)
- LLM-optimized content extraction
- Intelligent noise filtering
- Multiple output formats
- Citation support
- High-performance async design
- Smart content recognition
- Token efficiency optimization
- URL reference preservation
- Customizable search parameters
- Flexible output formatting
- FastMCP implementation

## Installation

```bash
# Method 1: Standard Installation
python -m venv crawl4ai_env
source crawl4ai_env/bin/activate  # Linux/Mac
# or
.\crawl4ai_env\Scripts\activate  # Windows

pip install -r requirements.txt
playwright install

# Method 2: Claude Desktop Client via Smithery
npx -y @smithery/cli install @weidwonder/crawl4ai-mcp-server --client claude
```

## Usage

```python
# Search Example
{
  "query": "python programming",
  "num_results": 5,
  "engine": "all"  # or "duckduckgo", "google"
}

# Content Extraction Example
{
  "url": "https://example.com",
  "format": "markdown_with_citations"  # or "fit_markdown", "raw_markdown", etc.
}
```

## Dependencies

- Python >= 3.9
- FastMCP framework
- Playwright browser
- DuckDuckGo API
- Google Custom Search API (optional)
- Content extraction engine
- Async runtime
- Token processor
- Format converter
- Citation manager

## Related Servers

- crawl4ai/crawl4ai (technology provider)
- modelcontextprotocol-web-scraping-server
- mendableai-firecrawl-mcp-server
- oxylabs-oxylabs-mcp