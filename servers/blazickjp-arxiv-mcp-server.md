---
type: server
repo_url: https://github.com/blazickjp/arxiv-mcp-server
name: ArXiv MCP Server
owner: blazickjp
stars: 70
last_updated: 2025-02-19
status: active
official: false
verified: false
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/academic", "integration/arxiv", "purpose/research", "category/search"]
---

# ArXiv MCP Server

#status/active #category/academic #integration/arxiv #purpose/research #category/search

## Description

The ArXiv MCP Server bridges the gap between AI models and academic research by providing a sophisticated interface to arXiv's extensive research repository. This server enables AI assistants to perform precise paper searches and access full paper content, enhancing their ability to engage with scientific literature.

## Features

- Precise paper search
- Full content access
- Metadata extraction
- Citation parsing
- Category filtering
- Author search
- Abstract analysis
- PDF processing

## Installation

```bash
npm install @blazickjp/arxiv-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "arxiv": {
      "command": "npx",
      "args": ["@blazickjp/arxiv-mcp"],
      "env": {
        "MAX_RESULTS": "100",
        "CACHE_TTL": "3600",
        "PDF_STORAGE": "./pdfs",
        "DEFAULT_CATEGORIES": "cs.AI,cs.LG,cs.CL"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- PDF processing tools
- Storage space for PDFs
- Internet connection

## Related Servers

- None currently listed