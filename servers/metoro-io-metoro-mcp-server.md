---
type: server
repo_url: https://github.com/metoro-io/metoro-mcp-server
name: Metoro
owner: metoro-io
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
tags: ["status/active", "status/official", "category/monitoring"]
---

#status/active #status/official #category/monitoring

# Metoro

## Description

Query and interact with kubernetes environments monitored by Metoro. This MCP server provides comprehensive monitoring and management capabilities for Kubernetes clusters through the Metoro platform.

## Features

- Kubernetes cluster monitoring
- Real-time metrics collection
- Resource utilization tracking
- Pod and container insights
- Performance analytics
- Alert management
- Cluster health monitoring
- Custom metric queries
- Historical data analysis
- Multi-cluster support

## Installation

```bash
npm install @metoro/mcp-server
```

## Usage

```javascript
import { MetoroServer } from "@metoro/mcp-server";

const server = new MetoroServer({
  apiKey: "your-metoro-api-key",
  clusterId: "your-cluster-id",
});

// Get cluster metrics
const metrics = await server.getMetrics({
  timeRange: {
    from: "now-1h",
    to: "now",
  },
  metrics: ["cpu_usage", "memory_usage", "pod_count"],
});

// Query pod status
const pods = await server.queryPods({
  namespace: "production",
  labelSelector: "app=frontend",
  status: "Running",
});

// Set up alerts
await server.createAlert({
  name: "High CPU Usage",
  condition: "cpu_usage > 80%",
  duration: "5m",
  severity: "critical",
  notifications: [
    {
      type: "slack",
      channel: "#alerts",
    },
  ],
});
```

## Dependencies

- Node.js >= 14.x
- Metoro account
- Metoro API key
- Kubernetes cluster

## Related Servers

- None currently listed
