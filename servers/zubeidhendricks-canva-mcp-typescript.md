---
type: server
repo_url: https://github.com/ZubeidHendricks/canva-mcp-typescript
name: Canva TypeScript MCP Server
owner: ZubeidHendricks
stars: 0
last_updated: 2025-02-17
status: active
official: false
verified: false
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/design",
    "integration/canva",
    "tech/typescript",
    "purpose/content-creation",
  ]
---

# Canva TypeScript MCP Server

#status/active #category/design #integration/canva #tech/typescript #purpose/content-creation

## Description

Integrates with Canva's API to enable automated generation and scheduling of viral content from spreadsheet data for efficient social media marketing.

## Features

- Canva API integration
- Content automation
- Spreadsheet data import
- Social media scheduling
- Design generation
- Template management
- Content optimization
- Performance tracking

## Installation

```bash
npm install @zubeidhendricks/canva-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "canva": {
      "command": "npx",
      "args": ["@zubeidhendricks/canva-mcp"],
      "env": {
        "CANVA_API_KEY": "your-api-key",
        "SPREADSHEET_URL": "your-sheet-url",
        "TEMPLATE_ID": "your-template-id",
        "SCHEDULE_INTERVAL": "daily"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- TypeScript >= 4.5
- Canva account
- API access

## Related Servers

- None currently listed
