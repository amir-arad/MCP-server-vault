--- 
type: server
repo_url: https://github.com/axiomhq/mcp-server-axiom
name: Axiom MCP Server
owner: axiomhq
stars: 14
last_updated: 2025-03-01
status: active
official: true
verified: true
sources: ["inbox/batch_003.md"]
tags: ["status/active", "status/official", "category/analytics", "integration/axiom", "purpose/data-analysis"]
---

# Axiom MCP Server

#status/active #status/official #category/analytics #integration/axiom #purpose/data-analysis

## Description

A Model Context Protocol server implementation for Axiom that enables AI agents to query your data using Axiom Processing Language (APL).

## Features

- APL query support
- Data analysis
- AI agent integration
- Query optimization
- Result formatting
- Data visualization
- Performance monitoring
- Access control

## Installation

```bash
npm install @axiomhq/mcp-server-axiom
```

## Usage

```javascript
{
  "mcpServers": {
    "axiom": {
      "command": "npx",
      "args": ["@axiomhq/mcp-server-axiom"],
      "env": {
        "AXIOM_TOKEN": "your-api-token",
        "AXIOM_ORG_ID": "your-org-id",
        "DEFAULT_DATASET": "your-dataset",
        "QUERY_TIMEOUT": "30"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Axiom account
- API token
- Dataset access

## Related Servers

- ThetaBird/mcp-server-axiom-js