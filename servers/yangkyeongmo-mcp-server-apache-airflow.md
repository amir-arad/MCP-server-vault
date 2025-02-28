--- 
type: server
repo_url: https://github.com/yangkyeongmo/mcp-server-apache-airflow
name: Apache Airflow MCP Server
owner: yangkyeongmo
stars: 1
last_updated: 2025-02-28
status: active
official: false
verified: true
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

Set the following environment variables:

```
AIRFLOW_HOST=<your-airflow-host>
AIRFLOW_USERNAME=<your-airflow-username>
AIRFLOW_PASSWORD=<your-airflow-password>
```

Add to your `claude_desktop_config.json`:

```json
{
 "mcpServers": {
 "mcp-server-apache-airflow": {
 "command": "uvx",
 "args": ["mcp-server-apache-airflow"],
 "env": {
 "AIRFLOW_HOST": "https://your-airflow-host",
 "AIRFLOW_USERNAME": "your-username",
 "AIRFLOW_PASSWORD": "your-password"
 }
 }
 }
}
```

Alternative configuration using `uv`:

```json
{
 "mcpServers": {
 "mcp-server-apache-airflow": {
 "command": "uv",
 "args": [
 "--directory",
 "/path/to/mcp-server-apache-airflow",
 "run",
 "mcp-server-apache-airflow"
 ],
 "env": {
 "AIRFLOW_HOST": "https://your-airflow-host",
 "AIRFLOW_USERNAME": "your-username",
 "AIRFLOW_PASSWORD": "your-password"
 }
 }
 }
}
```

Replace `/path/to/mcp-server-apache-airflow` with the actual path where you've cloned the repository.

### Manual Execution

You can also run the server manually:

```bash
python src/server.py
```

Options:

*   `--port`: Port to listen on for SSE (default: 8000)
*   `--transport`: Transport type (stdio/sse, default: stdio)

## Dependencies

- Node.js >= 14
- Apache Airflow instance
- REST API access
- Authentication credentials

## Related Servers

- None currently listed