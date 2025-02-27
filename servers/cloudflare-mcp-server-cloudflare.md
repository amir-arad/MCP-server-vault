---
repo_url: https://github.com/cloudflare/mcp-server-cloudflare
owner: cloudflare
name: mcp-server-cloudflare
stars: 277
last_updated: 2025-02-21
status: active
official: true
verified: true
sources:
  - inbox
  - awesome-mcp-servers-wong2
  - mcpservers-org
  - opentools
  - smithery-ai
tags:
  - status/active
  - status/official
  - category/cloud
  - integration/cloudflare
  - tech/typescript
  - purpose/infrastructure
---

# Cloudflare MCP Server

#status/active #status/official #category/cloud #integration/cloudflare #tech/typescript #purpose/infrastructure

## Description

The Cloudflare MCP server lets you use Claude Desktop, or any MCP Client, to use natural language to accomplish tasks on your Cloudflare account. Interact with Cloudflare's developer platform including Workers, KV, R2, D1, and other services.

## Features

- Deploy and configure Cloudflare resources
- Interact with Cloudflare Workers
- Manage KV, R2, and D1 data stores
- Control DNS settings
- Configure security settings
- View analytics and logs

## Installation

```bash
npm install -g @cloudflare/mcp-server
npx @cloudflare/mcp-server
```

## Authentication

The server uses Cloudflare API tokens for authentication. You'll need to create an API token with appropriate permissions in your Cloudflare dashboard.

## Dependencies

- Node.js v16+
- Cloudflare account with API access

## Related Servers

- [Cloudflare Github Backup MCP](https://github.com/DynamicEndpoints/cloudflare-github-backup-mcp)
