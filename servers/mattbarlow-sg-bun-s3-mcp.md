---
type: server
repo_url: https://github.com/mattbarlow-sg/bun-s3-mcp
name: Bun S3 MCP Server
owner: mattbarlow-sg
stars: 0
last_updated: 2025-01-16
status: active
official: false
verified: false
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/storage",
    "integration/s3",
    "tech/bun",
    "purpose/code-management",
  ]
---

# Bun S3 MCP Server

#status/active #category/storage #integration/s3 #tech/bun #purpose/code-management

## Description

Integrates with S3 to provide efficient code snippet management and retrieval.

## Features

- S3 integration
- Code snippet storage
- Snippet retrieval
- Efficient management
- Version control
- Search functionality
- Tag organization
- Access control

## Installation

```bash
npm install @mattbarlow-sg/bun-s3-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "bun-s3": {
      "command": "npx",
      "args": ["@mattbarlow-sg/bun-s3-mcp"],
      "env": {
        "AWS_ACCESS_KEY_ID": "your-access-key",
        "AWS_SECRET_ACCESS_KEY": "your-secret-key",
        "S3_BUCKET": "your-bucket",
        "SNIPPET_PREFIX": "code/"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Bun runtime
- AWS account
- S3 bucket

## Related Servers

- None currently listed
