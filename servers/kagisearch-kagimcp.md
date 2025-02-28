---
type: server
repo_url: https://github.com/kagisearch/kagimcp
name: Kagi Search
owner: kagisearch
stars: 0
last_updated: 2025-02-28
status: active
official: true
verified: true
sources: ["inbox"]
tags: ["status/active", "status/official", "category/search"]
---

# Kagi Search

#status/active #status/official #category/search

## Description

Search the web using Kagi's search API. This MCP server provides access to Kagi's powerful search capabilities, offering high-quality, privacy-focused web search results.

## Features

- Advanced web search capabilities
- Privacy-focused search results
- Customizable search parameters
- Rich search result metadata
- Fast response times
- Content filtering options
- Domain-specific searches
- Result ranking optimization

## Setup Instructions

> Before anything, ensure you have access to the search API. It is currently in closed beta and available upon request. Please reach out to [support@kagi.com](mailto:support@kagi.com) for an invite.

Install uv first.

MacOS/Linux:

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

Windows:

```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

## Setup with Claude Desktop

```json
{
  "mcpServers": {
    "kagi": {
      "command": "uvx",
      "args": ["kagimcp"],
      "env": {
        "KAGI_API_KEY": "YOUR_API_KEY_HERE"
      }
    }
  }
}
```

## Installing via Smithery

Alternatively, you can install Kagi for Claude Desktop automatically via [Smithery](https://smithery.ai/server/kagimcp):

```bash
npx -y @smithery/cli install kagimcp --client claude
```

## Ask Claude a question requiring search

e.g. "Who was time's 2024 person of the year?"

## Debugging

Run:

```bash
npx @modelcontextprotocol/inspector uvx kagimcp
```

## Dependencies

- Node.js >= 14.x
- Kagi API key
- Active Kagi subscription

## Related Servers

- None currently listed
