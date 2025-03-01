---
type: server
repo_url: https://github.com/hideya/mcp-client-langchain-py
name: LangChain Python Client MCP Server
owner: hideya
stars: 4
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/ai",
    "tech/python",
    "integration/langchain",
    "integration/openai",
    "integration/anthropic",
    "integration/groq",
    "tech/javascript",
  ]
---

# LangChain Python Client MCP Server

#status/active #category/ai #tech/python #integration/langchain #integration/openai #integration/anthropic #integration/groq

## Description

This server facilitates the invocation of AI models from providers like Anthropic, OpenAI, and Groq, enabling users to manage and configure large language model interactions seamlessly.

## Features

- Multi-provider support
- Model management
- API integration
- Response streaming
- Token management
- Error handling
- Rate limiting
- Model switching
- Context management
- Chain execution

## Installation

```bash
npm install @hideya/mcp-client-langchain-py
```

## Usage

```javascript
{
  "mcpServers": {
    "langchain-client": {
      "command": "npx",
      "args": ["@hideya/mcp-client-langchain-py"],
      "env": {
        "OPENAI_API_KEY": "your-openai-key",
        "ANTHROPIC_API_KEY": "your-anthropic-key",
        "GROQ_API_KEY": "your-groq-key",
        "DEFAULT_MODEL": "gpt-4",
        "MAX_TOKENS": "4096"
      }
    }
  }
}
```

## Dependencies

- Python >= 3.8
- LangChain
- OpenAI SDK
- Anthropic SDK
- Groq SDK
- Token counter

## Related Servers

- pyroprompts-any-chat-completions-mcp
- dmontgomery40-deepseek-mcp-server
- kivo360-anthropic-mcp-code-analyzer
