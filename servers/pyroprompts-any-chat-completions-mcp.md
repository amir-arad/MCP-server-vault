---
type: server
repo_url: https://github.com/pyroprompts/any-chat-completions-mcp
name: Any Chat Completions MCP Server
owner: pyroprompts
stars: 68
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/llm", "integration/openai", "integration/perplexity", "integration/groq", "integration/xai", "tech/typescript", "tech/javascript"]
---

# Any Chat Completions MCP Server

#status/active #category/llm #integration/openai #integration/perplexity #integration/groq #integration/xai #tech/typescript #tech/javascript

## Description

A TypeScript-based MCP server that enables Claude to integrate with any OpenAI SDK compatible chat completion API. This server allows Claude to communicate with various AI providers including OpenAI, Perplexity, Groq, xAI, PyroPrompts and more through a unified interface.

## Features

- OpenAI SDK compatibility for seamless integration
- Support for multiple AI providers (OpenAI, Perplexity, Groq, xAI, PyroPrompts)
- Configurable provider settings (API keys, base URLs, models)
- Ability to run multiple providers simultaneously
- Chat completion API relay
- Response streaming support
- Error handling and debugging tools
- Simple configuration through environment variables

## Installation

```bash
# Clone the repository
git clone https://github.com/pyroprompts/any-chat-completions-mcp.git
cd any-chat-completions-mcp

# Install dependencies
npm install

# Build the server
npm run build
```

## Usage

```javascript
{
  "mcpServers": {
    "chat-openai": {
      "command": "node",
      "args": [
        "/path/to/any-chat-completions-mcp/build/index.js"
      ],
      "env": {
        "AI_CHAT_KEY": "your-openai-key",
        "AI_CHAT_NAME": "OpenAI",
        "AI_CHAT_MODEL": "gpt-4o",
        "AI_CHAT_BASE_URL": "https://api.openai.com/v1"
      }
    },
    "chat-perplexity": {
      "command": "node",
      "args": [
        "/path/to/any-chat-completions-mcp/build/index.js"
      ],
      "env": {
        "AI_CHAT_KEY": "your-perplexity-key",
        "AI_CHAT_NAME": "Perplexity",
        "AI_CHAT_MODEL": "llama-3.1-sonar-small-128k-online",
        "AI_CHAT_BASE_URL": "https://api.perplexity.ai"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- TypeScript
- API keys for the providers you want to use
- OpenAI SDK compatible APIs

## Related Servers

- [OpenAI MCP Server](https://github.com/modelcontextprotocol/servers/tree/main/src/openai-server) - Official OpenAI integration
- [Groq MCP Server](https://github.com/modelcontextprotocol/servers/tree/main/src/groq-server) - Official Groq integration
- [Any Chat Completions API](https://github.com/pyroprompts/any-chat-completions-api) - Related project by PyroPrompts