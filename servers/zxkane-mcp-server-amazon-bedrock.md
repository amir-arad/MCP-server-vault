---
type: server
repo_url: https://github.com/zxkane/mcp-server-amazon-bedrock
name: Amazon Bedrock MCP Server
owner: zxkane
stars: 12
last_updated: 2025-01-26
status: active
official: false
verified: false
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/ai", "integration/aws", "integration/bedrock", "purpose/image-generation"]
---

# Amazon Bedrock MCP Server

#status/active #category/ai #integration/aws #integration/bedrock #purpose/image-generation

## Description

Provides access to Amazon Bedrock's Nova Canvas model for AI image generation.

## Features

- Amazon Bedrock integration
- Nova Canvas model access
- AI image generation
- AWS authentication
- Image customization
- Batch processing
- Result management
- AWS service integration

## Installation

```bash
npm install @zxkane/mcp-server-amazon-bedrock
```

## Usage

```javascript
{
  "mcpServers": {
    "amazon-bedrock": {
      "command": "npx",
      "args": ["@zxkane/mcp-server-amazon-bedrock"],
      "env": {
        "AWS_ACCESS_KEY_ID": "your-access-key",
        "AWS_SECRET_ACCESS_KEY": "your-secret-key",
        "AWS_REGION": "us-east-1",
        "MODEL_ID": "nova-canvas-1"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- AWS credentials
- Amazon Bedrock access
- AWS SDK

## Related Servers

- None currently listed