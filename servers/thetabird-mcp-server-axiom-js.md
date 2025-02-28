---
type: server
repo_url: https://github.com/ThetaBird/mcp-server-axiom-js
name: Axiom JS MCP Server
owner: ThetaBird
stars: 1
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_003.md"]
tags:
  [
    "status/active",
    "category/analytics",
    "integration/axiom",
    "tech/javascript",
    "purpose/data-analysis",
  ]
---

```bash
npx -y @smithery/cli install @ThetaBird/mcp-server-axiom-js --client claude
```

```bash
npx -y @smithery/cli install @ThetaBird/mcp-server-axiom-js --client claude
```

# Axiom JS MCP Server

#status/active #category/analytics #integration/axiom #tech/javascript #purpose/data-analysis

## Description

An npx-compatible port of @Axiom's mcp-server-axiom.

## Features

- NPX compatibility
- Axiom integration
- Data analysis
- Query execution
- JavaScript implementation
- Result formatting
- Error handling
- Configuration management

## Installation

```bash
npm install @thetabird/axiom-mcp-js
```

## Usage

```javascript
{
  "mcpServers": {
    "axiom-js": {
      "command": "npx",
      "args": ["@thetabird/axiom-mcp-js"],
      "env": {
        "AXIOM_API_TOKEN": "your-api-token",
        "AXIOM_ORG_ID": "your-org-id",
        "DATASET_NAME": "your-dataset",
        "CACHE_TTL": "300"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Axiom account
- API credentials
- Dataset permissions

## Related Servers

- axiomhq/mcp-server-axiom
