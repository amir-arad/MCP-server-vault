---
type: server
repo_url: https://github.com/RafalWilinski/aws-mcp
name: AWS MCP Server
owner: RafalWilinski
stars: 95
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_003.md"]
tags:
  [
    "status/active",
    "category/cloud",
    "integration/aws",
    "purpose/cloud-management",
    "category/ai",
  ]
---

# AWS MCP Server

#status/active #category/cloud #integration/aws #purpose/cloud-management #category/ai

## Description

A Model Context Protocol (MCP) server that enables AI assistants like Claude to interact with your AWS environment. This allows for natural language querying and management of your AWS resources during conversations. Think of better Amazon Q alternative.

## Features

- Natural language AWS interaction
- Resource management
- Service querying
- Cost monitoring
- Security analysis
- Performance tracking
- Infrastructure management
- Configuration control

## Installation

```bash
npm install @rafalwilinski/aws-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "aws": {
      "command": "npx",
      "args": ["@rafalwilinski/aws-mcp"],
      "env": {
        "AWS_ACCESS_KEY_ID": "your-access-key",
        "AWS_SECRET_ACCESS_KEY": "your-secret-key",
        "AWS_REGION": "us-east-1",
        "LANGUAGE_MODEL": "gpt-4"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- AWS account
- IAM credentials
- Language model access

## Related Servers

- modelcontextprotocol/aws-kb-retrieval-server
- rishikavikondala/mcp-server-aws
- baryhuang/mcp-server-aws-resources-python
