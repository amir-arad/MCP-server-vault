---
type: server
repo_url: https://github.com/kimtth/mcp-aoai-web-browsing
name: AOAI Web Browsing MCP Server
owner: kimtth
stars: 6
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_002.md"]
tags:
  [
    "status/active",
    "category/web-browsing",
    "integration/azure",
    "integration/openai",
    "purpose/web-interaction",
  ]
---

# AOAI Web Browsing MCP Server

#status/active #category/web-browsing #integration/azure #integration/openai #purpose/web-interaction

## Description

A minimal server/client application implementation utilizing the Model Context Protocol (MCP) and Azure OpenAI.

## Features

- Azure OpenAI integration
- Web browsing capabilities
- Client-server architecture
- MCP protocol support
- Web page interaction
- Content extraction
- Navigation control
- Session management
- The MCP server is built with `FastMCP`.
- `Playwright` is used for web browser automation.
- The MCP response about tools is converted to the OpenAI function calling format.

## Installation

```bash
npm install @kimtth/mcp-aoai-web-browsing
```

## Usage

1.  Rename `.env.template` to `.env`, then fill in the values in `.env` for Azure OpenAI:

```
AZURE_OPEN_AI_ENDPOINT=
AZURE_OPEN_AI_API_KEY=
AZURE_OPEN_AI_DEPLOYMENT_MODEL=
AZURE_OPEN_AI_API_VERSION=
```

2.  Install `uv` for python library management

```bash
pip install uv
uv sync
```

3.  Execute `python chatgui.py`

- The sample screen shows the client launching a browser to navigate to the URL.

```javascript
{
  "mcpServers": {
    "aoai-web": {
      "command": "npx",
      "args": ["@kimtth/mcp-aoai-web-browsing"],
      "env": {
        "AZURE_OPENAI_KEY": "your-azure-openai-key",
        "AZURE_OPENAI_ENDPOINT": "your-azure-endpoint",
        "MODEL_DEPLOYMENT": "gpt-4",
        "MAX_TOKENS": "4000"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Azure OpenAI subscription
- Web browser automation
- MCP client library

## Related Servers

- None currently listed
