---
type: server
repo_url: https://github.com/mendableai/firecrawl-mcp-server
name: Firecrawl
owner: mendableai
stars: 0
last_updated: 2025-02-28
status: active
official: true
verified: true
sources: ["inbox"]
tags: ["status/active", "status/official", "category/web-scraping"]
---

# Firecrawl

## Description

Extract web data with [Firecrawl](https://firecrawl.dev). This MCP server provides powerful web scraping and data extraction capabilities, allowing you to efficiently collect and process web content.

## Features

- Scrape, crawl, search, extract and batch scrape support
- Web scraping with JS rendering
- URL discovery and crawling
- Web search with content extraction
- Automatic retries with exponential backoff
- Efficient batch processing with built-in rate limiting
- Credit usage monitoring for cloud API
- Comprehensive logging system
- Support for cloud and self-hosted FireCrawl instances
- Mobile/Desktop viewport support
- Smart content filtering with tag inclusion/exclusion
- Advanced web scraping capabilities
- Automated data extraction
- Support for dynamic websites
- Rate limiting and proxy management
- Custom extraction rules
- Structured data output
- Browser-based rendering support

## Installation

### Running with npx

```bash
env FIRECRAWL_API_KEY=fc-YOUR_API_KEY npx -y firecrawl-mcp
```

### Manual Installation

```bash
npm install -g firecrawl-mcp
```

### Running on Cursor

Configuring Cursor 🖥️ Note: Requires Cursor version 0.45.6+

To configure FireCrawl MCP in Cursor:

1.  Open Cursor Settings
2.  Go to Features > MCP Servers
3.  Click "+ Add New MCP Server"
4.  Enter the following:
    - Name: "firecrawl-mcp" (or your preferred name)
    - Type: "command"
    - Command: `env FIRECRAWL_API_KEY=your-api-key npx -y firecrawl-mcp`

> If you are using Windows and are running into issues, try `cmd /c "set FIRECRAWL_API_KEY=your-api-key && npx -y firecrawl-mcp"`

Replace `your-api-key` with your FireCrawl API key.

After adding, refresh the MCP server list to see the new tools. The Composer Agent will automatically use FireCrawl MCP when appropriate, but you can explicitly request it by describing your web scraping needs. Access the Composer via Command+L (Mac), select "Agent" next to the submit button, and enter your query.

### Running on Windsurf

Add this to your `./codeium/windsurf/model_config.json`:

```json
{
  "mcpServers": {
    "mcp-server-firecrawl": {
      "command": "npx",
      "args": ["-y", "firecrawl-mcp"],
      "env": {
        "FIRECRAWL_API_KEY": "YOUR_API_KEY_HERE"
      }
    }
  }
}
```

## Configuration

### Environment Variables

#### Required for Cloud API

- `FIRECRAWL_API_KEY`: Your FireCrawl API key
  - Required when using cloud API (default)
  - Optional when using self-hosted instance with `FIRECRAWL_API_URL`
- `FIRECRAWL_API_URL` (Optional): Custom API endpoint for self-hosted instances
  - Example: `https://firecrawl.your-domain.com`
  - If not provided, the cloud API will be used (requires API key)

#### Optional Configuration

##### Retry Configuration

- `FIRECRAWL_RETRY_MAX_ATTEMPTS`: Maximum number of retry attempts (default: 3)
- `FIRECRAWL_RETRY_INITIAL_DELAY`: Initial delay in milliseconds before first retry (default: 1000)
- `FIRECRAWL_RETRY_MAX_DELAY`: Maximum delay in milliseconds between retries (default: 10000)
- `FIRECRAWL_RETRY_BACKOFF_FACTOR`: Exponential backoff multiplier (default: 2)

##### Credit Usage Monitoring

- `FIRECRAWL_CREDIT_WARNING_THRESHOLD`: Credit usage warning threshold (default: 1000)
- `FIRECRAWL_CREDIT_CRITICAL_THRESHOLD`: Credit usage critical threshold (default: 100)
