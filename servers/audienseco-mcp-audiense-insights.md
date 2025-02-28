---
type: server
repo_url: https://github.com/AudienseCo/mcp-audiense-insights
name: Audiense Insights MCP Server
owner: AudienseCo
stars: 1
last_updated: 2025-02-17
status: active
official: false
verified: false
sources: ["inbox/batch_003.md"]
tags: ["status/active", "category/marketing", "integration/audiense", "purpose/analytics"]
---

# Audiense Insights MCP Server

#status/active #category/marketing #integration/audiense #purpose/analytics

## Description

Enables interaction with Audiense Insights accounts via the Model Context Protocol, facilitating the extraction and analysis of marketing insights and audience data including demographics, behavior, and influencer engagement.

## Features

- Marketing insights extraction
- Audience data analysis
- Demographic profiling
- Behavioral analysis
- Influencer engagement tracking
- Data visualization
- Report generation
- Trend analysis

## Installation

```bash
npm install @audienseco/mcp-insights
```

## Usage

```javascript
{
  "mcpServers": {
    "audiense-insights": {
      "command": "npx",
      "args": ["@audienseco/mcp-insights"],
      "env": {
        "AUDIENSE_API_KEY": "your-api-key",
        "ACCOUNT_ID": "your-account-id",
        "DATA_RETENTION": "30",
        "MAX_RESULTS": "1000"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Audiense account
- API credentials
- Data access permissions

## Related Servers

- None currently listed