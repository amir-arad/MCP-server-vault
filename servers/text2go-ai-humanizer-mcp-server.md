---
type: server
repo_url: https://github.com/Text2Go/ai-humanizer-mcp-server
name: AI Humanizer MCP Server
owner: Text2Go
stars: 6
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_001.md"]
tags:
  [
    "status/active",
    "category/content-processing",
    "category/ai",
    "purpose/text-enhancement",
  ]
---

To install AI Humanizer MCP Server for Claude Desktop automatically via [Smithery](https://smithery.ai/server/@Text2Go/ai-humanizer-mcp-server):

```bash
npx -y @smithery/cli install @Text2Go/ai-humanizer-mcp-server --client claude
```

# AI Humanizer MCP Server

#status/active #category/content-processing #category/ai #purpose/text-enhancement

## Description

Helps refine AI-generated content to sound more natural and human-like. Built with advanced AI detection and text enhancement capabilities.

## Features

- AI content detection
- Natural language enhancement
- Text refinement
- Style customization
- Tone adjustment
- Context preservation
- Readability improvement
- Voice consistency

## Installation

```bash
npm install @text2go/ai-humanizer-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "ai-humanizer": {
      "command": "npx",
      "args": ["@text2go/ai-humanizer-mcp"],
      "env": {
        "MODEL_PATH": "./models",
        "MAX_TEXT_LENGTH": "5000",
        "STYLE_PRESET": "casual",
        "ENHANCEMENT_LEVEL": "balanced"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- AI detection models
- Text processing libraries
- NLP resources

## Related Servers

- None currently listed
