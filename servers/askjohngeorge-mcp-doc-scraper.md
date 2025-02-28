---
type: server
repo_url: https://github.com/askjohngeorge/mcp-doc-scraper
name: Doc Scraper MCP Server
owner: askjohngeorge
stars: 2
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_010.md"]
tags:
  [
    "status/active",
    "category/documentation",
    "integration/jina",
    "purpose/web-scraping",
    "purpose/content-conversion",
    "tech/markdown",
  ]
---

# Doc Scraper MCP Server

#status/active #category/documentation #integration/jina #purpose/web-scraping #purpose/content-conversion #tech/markdown

## Description

Converts web documentation to clean markdown using Jina.ai's API, enabling easy transformation of online docs for content migration or offline use.

## Features

- Web documentation scraping
- Markdown conversion
- Jina.ai API integration
- Content cleaning and formatting
- Batch processing
- Link preservation
- Image handling
- Code block formatting
- Table conversion
- Metadata extraction

## Installation

```bash
pip install mcp-doc-scraper
```

## Usage

```javascript
{
  "mcpServers": {
    "doc-scraper": {
      "command": "python",
      "args": ["-m", "mcp_doc_scraper"],
      "env": {
        "JINA_API_KEY": "your-jina-api-key",
        "MAX_CONCURRENT_REQUESTS": "5",
        "OUTPUT_DIR": "./docs"
      }
    }
  }
}
```

## Dependencies

- Python >= 3.8
- Jina.ai API access
- BeautifulSoup4
- requests
- markdown2
- html2text

## Related Servers

- None currently listed
