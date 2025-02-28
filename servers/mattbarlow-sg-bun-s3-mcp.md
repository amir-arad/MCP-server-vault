---
type: server
repo_url: https://github.com/mattbarlow-sg/bun-s3-mcp
name: Bun S3 MCP Server
owner: mattbarlow-sg
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
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

This is an MCP service that uses Bun's [s3 bindings](https://bun.sh/docs/api/s3). The service works with Claude Desktop to save and load code snippets to S3 as markdown files. Integrates with S3 to provide efficient code snippet management and retrieval.

## Features

- Use the bun runtime directly for MCP which eliminates transpilation.
- Use bun s3 bindings for fast S3 API operations.
- Shows how to configure preloading for mocking in Bun tests.
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
