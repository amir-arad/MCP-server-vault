---
type: server
repo_url: https://github.com/macrat/mcp-ayd-server
name: Ayd MCP Server
owner: macrat
stars: 0
last_updated: 2024-12-16
status: active
official: false
verified: false
sources: ["inbox/batch_003.md"]
tags: ["status/active", "category/monitoring", "purpose/service-monitoring", "purpose/incident-response"]
---

# Ayd MCP Server

#status/active #category/monitoring #purpose/service-monitoring #purpose/incident-response

## Description

Integrates with Ayd to enable service monitoring, status checks, and log retrieval for enhanced operational visibility and incident response.

## Features

- Service monitoring
- Status checks
- Log retrieval
- Operational visibility
- Incident response
- Alert management
- Performance tracking
- Health reporting

## Installation

```bash
npm install @macrat/mcp-ayd
```

## Usage

```javascript
{
  "mcpServers": {
    "ayd": {
      "command": "npx",
      "args": ["@macrat/mcp-ayd"],
      "env": {
        "AYD_ENDPOINT": "http://localhost:9000",
        "CHECK_INTERVAL": "60",
        "LOG_RETENTION": "7d",
        "ALERT_THRESHOLD": "3"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Ayd instance
- Service endpoints
- Log storage

## Related Servers

- None currently listed