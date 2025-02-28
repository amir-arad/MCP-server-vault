---
type: server
repo_url: https://github.com/Lakphy/deep-reasoning-mcp
name: Deep Reasoning MCP Server
owner: Lakphy
stars: 4
last_updated: 2025-02-18
status: active
official: false
verified: false
sources: ["inbox/batch_008.md"]
tags:
  [
    "status/active",
    "category/ai",
    "integration/openrouter",
    "purpose/reasoning",
    "purpose/analysis",
    "tech/sdk",
  ]
---

# Deep Reasoning MCP Server

#status/active #category/ai #integration/openrouter #purpose/reasoning #purpose/analysis #tech/sdk

## Description

Integrates with OpenRouter's AI SDK to enable deep reasoning capabilities for complex analysis and inference tasks. This server provides advanced reasoning capabilities for sophisticated problem-solving.

## Features

- Deep reasoning
- Complex analysis
- Inference tasks
- Chain reasoning
- Logic processing
- Pattern recognition
- Decision making
- Explanation generation
- Context handling
- Result validation

## Installation

```bash
npm install @lakphy/deep-reasoning-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "deep-reasoning": {
      "command": "npx",
      "args": ["@lakphy/deep-reasoning-mcp"],
      "env": {
        "OPENROUTER_API_KEY": "your-api-key",
        "MAX_DEPTH": "10",
        "TIMEOUT": "60000",
        "MODEL": "gpt-4",
        "CONFIDENCE_THRESHOLD": "0.8"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- OpenRouter SDK
- AI models
- Reasoning engine
- Analysis tools
- Validation system

## Related Servers

- modelcontextprotocol-reasoning-server
- kivo360-anthropic-mcp-code-analyzer
- bmorphism-anti-bullshit-mcp-server
