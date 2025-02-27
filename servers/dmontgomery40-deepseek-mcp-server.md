---
repo_url: https://github.com/DMontgomery40/deepseek-mcp-server
owner: DMontgomery40
name: deepseek-mcp-server
stars: 57
last_updated: 2025-02-20
status: active
official: false
verified: false
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
  - tech/typescript
  - purpose/reasoning
---

#status/active #status/community #category/llm #integration/deepseek #tech/typescript #purpose/reasoning

# DeepSeek MCP Server

## Description

The DeepSeek MCP Server is a Model Context Protocol implementation that integrates DeepSeek's advanced language models with MCP-compatible applications. It offers features like chat completion, custom model selection, and parameter control for enhancing language-based interactions.

## Features

- Integration with DeepSeek's language models
- Support for DeepSeek R1 reasoning engine
- Chat completion API
- Custom parameter configuration
- Multi-model support

## Installation

```bash
# Clone the repository
git clone https://github.com/DMontgomery40/deepseek-mcp-server.git
cd deepseek-mcp-server

# Install dependencies
npm install

# Configure your API key
echo "DEEPSEEK_API_KEY=your_api_key" > .env

# Start the server
npm start
```

## Authentication

The server requires a DeepSeek API key which should be stored in the environment variables or a .env file.

## Dependencies

- Node.js v16+
- DeepSeek API access

## Related Servers

- [Deepseek Claude MCP Server](https://github.com/HarshJ23/deepseek-claude-MCP-server)
- [Deepseek Thinking Claude 3.5 Sonnet Cline MCP](https://github.com/newideas99/Deepseek-Thinking-Claude-3.5-Sonnet-CLINE-MCP)
- [Deepseek R1](https://github.com/66julienmartin/MCP-server-Deepseek_R1)
