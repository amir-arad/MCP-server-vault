---
type: server
repo_url: https://github.com/kimtth/mcp-aoai-web-browsing
name: AOAI Web Browsing MCP Server
owner: kimtth
stars: 6
last_updated: 2025-01-27
status: active
official: false
verified: false
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/web-browsing", "integration/azure", "integration/openai", "purpose/web-interaction"]
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

## Installation

```bash
npm install @kimtth/mcp-aoai-web-browsing
```

## Usage

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