---
type: server
repo_url: https://github.com/yangkyeongmo/mcp-server-apache-airflow
name: Apache Airflow MCP Server
owner: yangkyeongmo
stars: 1
last_updated: 2025-02-18
status: active
official: false
verified: false
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/workflow", "integration/airflow", "purpose/orchestration"]
---

# Apache Airflow MCP Server

#status/active #category/workflow #integration/airflow #purpose/orchestration

## Description

Provides a standardized way for MCP clients to interact with Apache Airflow's REST API, supporting operations like DAG management and monitoring Airflow system health.

## Features

- DAG management
- System health monitoring
- REST API integration
- Workflow orchestration
- Task scheduling
- Execution tracking
- Error handling
- Performance monitoring

## Installation

```bash
npm install @yangkyeongmo/mcp-server-apache-airflow
```

## Usage

```javascript
{
  "mcpServers": {
    "airflow": {
      "command": "npx",
      "args": ["@yangkyeongmo/mcp-server-apache-airflow"],
      "env": {
        "AIRFLOW_API_URL": "http://localhost:8080",
        "AIRFLOW_USERNAME": "admin",
        "AIRFLOW_PASSWORD": "admin",
        "REFRESH_INTERVAL": "30"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Apache Airflow instance
- REST API access
- Authentication credentials

## Related Servers

- None currently listed