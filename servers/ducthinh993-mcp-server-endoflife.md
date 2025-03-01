--- 
type: server
repo_url: https://github.com/ducthinh993/mcp-server-endoflife
name: End of Life MCP Server
owner: ducthinh993
stars: 1
last_updated: 2025-03-01
status: active
official: false
verified: true
sources: ["inbox/batch_010.md"]
tags: ["status/active", "category/software-lifecycle", "integration/endoflife-date", "purpose/version-tracking", "purpose/security-status", "category/ai"]
---

# End of Life MCP Server

#status/active #category/software-lifecycle #integration/endoflife-date #purpose/version-tracking #purpose/security-status #category/ai

## Description

Enables AI assistants to check software end-of-life dates and support status using the endoflife.date API, providing accurate information on software lifecycle, security status, and upgrade recommendations in real-time.

## Features

- Software lifecycle tracking
- End-of-life date checking
- Support status monitoring
- Security status tracking
- Upgrade recommendations
- Version comparison
- Real-time updates
- API integration
- Data caching
- Notification system

## Installation

```bash
npm install @ducthinh993/mcp-server-endoflife
```

## Usage

```javascript
{
  "mcpServers": {
    "endoflife": {
      "command": "npx",
      "args": ["@ducthinh993/mcp-server-endoflife"],
      "env": {
        "ENDOFLIFE_API_KEY": "your-api-key",
        "CACHE_DURATION": "86400",
        "NOTIFICATION_THRESHOLD": "90",
        "CHECK_INTERVAL": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- endoflife.date API access
- Cache storage
- Network connectivity
- Notification system

## Related Servers

- None currently listed