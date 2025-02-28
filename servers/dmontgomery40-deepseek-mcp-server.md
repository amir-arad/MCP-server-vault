---
type: server
repo_url: https://github.com/DMontgomery40/deepseek-mcp-server
name: DeepSeek MCP Server
owner: DMontgomery40
stars: 70
last_updated: 2025-02-28
status: active
official: false
verified: true
sources:
  - inbox
  - awesome-mcp-servers-wong2
  - mcpservers-org
  - opentools
tags:
  - status/active
  - status/community
  - category/llm
  - integration/deepseek
  - tech/javascript
  - purpose/reasoning
---

#status/active #status/community #category/llm #integration/deepseek #tech/javascript #purpose/reasoning

# DeepSeek MCP Server

## Description

A Model Context Protocol (MCP) server for the DeepSeek API, allowing seamless integration of DeepSeek's powerful language models with MCP-compatible applications like Claude Desktop. The server provides access to DeepSeek's advanced models including R1 (reasoner) and V3 (chat) with customizable parameters and multi-turn conversation support.

## Features

- Integration with DeepSeek's language models (R1 and V3)
- Automatic model fallback if primary model is unavailable
- Custom model selection and configuration
- Temperature control (0.0 - 2.0)
- Max tokens limit adjustment
- Top P sampling (0.0 - 1.0)
- Presence and frequency penalty settings
- Multi-turn conversation support with context preservation
- Resource discovery for available models and configurations

## Installation

```bash
# Install via npm
npm install -g deepseek-mcp-server

# Or install via Smithery
npx -y @smithery/cli install @dmontgomery40/deepseek-mcp-server --client claude
```

## Usage

```javascript
{
  "mcpServers": {
    "deepseek": {
      "command": "npx",
      "args": ["-y", "deepseek-mcp-server"],
      "env": {
        "DEEPSEEK_API_KEY": "your-api-key"
      }
    }
  }
}
```

## Dependencies

- Node.js
- DeepSeek API key
- Internet connection

## Related Servers

- [Deepseek Claude MCP Server](https://github.com/HarshJ23/deepseek-claude-MCP-server) - Alternative implementation
- [Deepseek Thinking Claude 3.5 Sonnet Cline MCP](https://github.com/newideas99/Deepseek-Thinking-Claude-3.5-Sonnet-CLINE-MCP) - Enhanced version
- [Deepseek R1](https://github.com/66julienmartin/MCP-server-Deepseek_R1) - R1 model focused implementation