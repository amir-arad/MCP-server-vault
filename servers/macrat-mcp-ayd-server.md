---
type: server
repo_url: https://github.com/macrat/mcp-ayd-server
name: Ayd MCP Server
owner: macrat
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_003.md"]
tags:
  [
    "status/active",
    "category/monitoring",
    "purpose/service-monitoring",
    "purpose/incident-response",
  ]
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

## Usage

1.  Download the latest binary from [release page](https://github.com/macrat/mcp-ayd-server/releases).
2.  Setup your client's configuration file.

    For example, if you use Claude Desktop:

```json
{
  "mcpServers": {
    "ayd": {
      "command": "C:\\path\\to\\mcp-ayd-server.exe",
      "args": ["http://127.0.0.1:9000"]
    }
  }
}
```

3.  Run the client app.
4.  Ask assistant like "What's the latest status of Ayd?"

## Dependencies

- Node.js >= 14
- Ayd instance
- Service endpoints
- Log storage

## Related Servers

- None currently listed
