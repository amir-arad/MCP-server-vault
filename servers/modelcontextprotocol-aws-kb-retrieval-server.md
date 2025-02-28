---
type: server
repo_url: https://github.com/modelcontextprotocol/servers/tree/main/src/aws-kb-retrieval-server
name: AWS KB Retrieval Server
owner: modelcontextprotocol
stars: 9794
last_updated: 2025-02-21
status: active
official: true
verified: false
sources: ["inbox/batch_003.md"]
tags: ["status/active", "status/official", "category/knowledge-base", "integration/aws", "integration/bedrock"]
---

# AWS KB Retrieval Server

#status/active #status/official #category/knowledge-base #integration/aws #integration/bedrock

## Description

Retrieval from AWS Knowledge Base using Bedrock Agent Runtime.

## Features

- Knowledge base retrieval
- Bedrock agent integration
- Runtime management
- Query processing
- Content indexing
- Search optimization
- Response formatting
- Context handling

## Installation

```bash
npm install @modelcontextprotocol/aws-kb-retrieval-server
```

## Usage

```javascript
{
  "mcpServers": {
    "aws-kb": {
      "command": "npx",
      "args": ["@modelcontextprotocol/aws-kb-retrieval-server"],
      "env": {
        "AWS_ACCESS_KEY_ID": "your-access-key",
        "AWS_SECRET_ACCESS_KEY": "your-secret-key",
        "AWS_REGION": "us-east-1",
        "BEDROCK_AGENT_ID": "your-agent-id"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- AWS account
- Bedrock access
- Knowledge base setup

## Related Servers

- RafalWilinski/aws-mcp
- rishikavikondala/mcp-server-aws
- baryhuang/mcp-server-aws-resources-python