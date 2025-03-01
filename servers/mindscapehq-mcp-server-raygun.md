--- 
type: server
repo_url: https://github.com/MindscapeHQ/mcp-server-raygun
name: Raygun
owner: MindscapeHQ
stars: 3
last_updated: 2025-02-28
status: active
official: true
verified: true
sources: ["inbox"]
tags: ["status/active", "status/official", "category/monitoring"]
---

#status/active #status/official #category/monitoring

# Raygun

## Description

Interact with your crash reporting and real using monitoring data on your Raygun account. This MCP server provides comprehensive access to Raygun's API features through the Model Context Protocol.

## Features

- Crash reporting integration
- Real-time monitoring
- Error tracking
- Performance metrics
- User session tracking
- Issue management
- Deployment tracking
- Alert configuration
- Custom grouping rules
- Detailed error analysis

## Installation

```bash
npm install @raygun/mcp-server
```

## Usage

```javascript
import { RaygunServer } from "@raygun/mcp-server";

const server = new RaygunServer({
  apiKey: "your-raygun-api-key",
  applicationId: "your-app-id",
});

// Get crash reports
const crashes = await server.getCrashes({
  timeRange: {
    from: "now-24h",
    to: "now",
  },
  filters: {
    status: "active",
    severity: ["error", "critical"],
  },
});

// Analyze performance metrics
const performance = await server.getPerformanceMetrics({
  timeframe: "1h",
  metrics: ["page_load_time", "server_response_time", "database_queries"],
  groupBy: "endpoint",
});

// Track deployment
await server.trackDeployment({
  version: "1.2.3",
  timestamp: new Date().toISOString(),
  metadata: {
    commitHash: "abc123",
    environment: "production",
    deployer: "CI/CD",
  },
});

// Configure alerts
await server.createAlert({
  name: "High Error Rate",
  condition: {
    metric: "error_rate",
    operator: ">",
    threshold: 5,
    timeWindow: "5m",
  },
  notifications: [
    {
      type: "email",
      recipients: ["team@example.com"],
    },
    {
      type: "slack",
      channel: "#alerts",
    },
  ],
});
```

## Dependencies

- Node.js >= 14.x
- Raygun account
- Raygun API key
- Application ID in Raygun

## Related Servers

- None currently listed