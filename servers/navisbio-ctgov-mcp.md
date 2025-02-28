---
type: server
repo_url: https://github.com/navisbio/ctgov_MCP
name: Clinical Trials Database MCP Server
owner: navisbio
stars: 3
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_008.md"]
tags:
  [
    "status/active",
    "category/healthcare",
    "integration/aact",
    "purpose/clinical-trials",
    "purpose/research",
    "category/database",
    "tech/python",
    "tech/postgresql",
    "purpose/data-analysis",
    "purpose/insights"
  ]
---

# Clinical Trials Database MCP Server

#status/active #category/healthcare #integration/aact #purpose/clinical-trials #purpose/research #category/database #tech/python #tech/postgresql #purpose/data-analysis #purpose/insights

## Description

A Python-based MCP server that provides access to the AACT (Aggregate Analysis of ClinicalTrials.gov) database. The server enables comprehensive analysis of clinical trial data, tracking development trends, and automatically generating analysis memos that capture insights about therapeutic landscapes. It offers tools for querying trial data, analyzing patterns, and extracting valuable research insights.

## Features

- Clinical trial data querying
- Therapeutic landscape analysis
- Research pattern tracking
- Insight generation
- Data extraction
- Query optimization
- Result filtering
- Statistical analysis
- Data visualization
- Export functionality
- Schema exploration
- Memo generation
- Pattern recognition
- Trend analysis

## Installation

```bash
# Option 1: Using published package
uvx mcp-server-aact

# Option 2: Running from source
git clone https://github.com/navisbio/ctgov_MCP.git
cd ctgov_MCP
uv run mcp-server-aact
```

## Usage

```python
# Configuration
{
  "mcpServers": {
    "clinical-trials": {
      "command": "uvx",
      "args": ["mcp-server-aact"],
      "env": {
        "DB_USER": "your-username",
        "DB_PASSWORD": "your-password",
        "CACHE_TTL": "3600"
      }
    }
  }
}

# Example Analysis Query
{
  "prompt": "indication-landscape",
  "arguments": {
    "topic": "multiple sclerosis"
  }
}
```

## Dependencies

- Python >= 3.9
- AACT database access
- PostgreSQL client
- Query builder
- Data analyzer
- Export handler
- Cache manager
- Insight generator
- Pattern analyzer
- Statistical tools

## Related Servers

- modelcontextprotocol-healthcare-server
- kartha-ai-agentcare-mcp
- modelcontextprotocol-research-server
- OpenDataMCP/OpenDataMCP