---
type: server
repo_url: https://github.com/rishikavikondala/mcp-server-aws
name: AWS MCP Server
owner: rishikavikondala
stars: 40
last_updated: 2025-02-19
status: active
official: false
verified: false
sources: ["inbox/batch_003.md"]
tags: ["status/active", "category/cloud", "integration/aws", "integration/s3", "integration/dynamodb"]
---

# AWS MCP Server

#status/active #category/cloud #integration/aws #integration/s3 #integration/dynamodb

## Description

Manage AWS S3 and DynamoDB resources.

## Features

- S3 bucket management
- DynamoDB operations
- Resource monitoring
- Access control
- Data manipulation
- Backup management
- Cost optimization
- Performance tracking

## Installation

```bash
npm install @rishikavikondala/mcp-server-aws
```

## Usage

```javascript
{
  "mcpServers": {
    "aws": {
      "command": "npx",
      "args": ["@rishikavikondala/mcp-server-aws"],
      "env": {
        "AWS_ACCESS_KEY_ID": "your-access-key",
        "AWS_SECRET_ACCESS_KEY": "your-secret-key",
        "AWS_REGION": "us-east-1",
        "DEFAULT_BUCKET": "your-bucket-name"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- AWS account
- IAM credentials
- AWS SDK

## Related Servers

- modelcontextprotocol/aws-kb-retrieval-server
- RafalWilinski/aws-mcp
- baryhuang/mcp-server-aws-resources-python