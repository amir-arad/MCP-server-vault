---
type: server
repo_url: https://github.com/grafana/mcp-grafana
name: Grafana
owner: grafana
stars: 50
last_updated: 2025-02-28
status: active
official: true
verified: true
sources: ["inbox"]
tags:
  [
    "status/active",
    "status/official",
    "category/monitoring",
    "category/analytics",
    "tech/python",
  ]
---

# Grafana

#status/active #status/official #category/monitoring #category/analytics

## Description

Search dashboards, investigate incidents and query datasources in your Grafana instance. This MCP server enables seamless interaction with Grafana's monitoring and analytics capabilities.

## Features

- Dashboard search and management
- Incident investigation tools
- Data source querying
- Metrics visualization
- Alert management
- Real-time monitoring
- Custom dashboard creation
- Cross-datasource analytics

## Installation

```bash
npm install @grafana/mcp-server
```

## Usage

```javascript
import { GrafanaServer } from "@grafana/mcp-server";

const server = new GrafanaServer({
  url: "https://your-grafana-instance.com",
  apiKey: "your-grafana-api-key",
});

// Search dashboards
const dashboards = await server.searchDashboards({
  query: "Production Metrics",
  folder: "Operations",
});

// Query a datasource
const metrics = await server.queryDatasource({
  datasourceName: "Prometheus",
  query: "rate(http_requests_total[5m])",
  timeRange: {
    from: "now-1h",
    to: "now",
  },
});
```

## Dependencies

- Node.js >= 14.x
- Grafana instance
- Grafana API key

## Related Servers

- None currently listed
