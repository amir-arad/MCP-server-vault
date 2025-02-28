---
type: server
repo_url: https://github.com/metoro-io/metoro-mcp-server
name: Metoro
owner: metoro-io
stars: 0
last_updated: 2025-02-28
status: active
official: true
verified: true
sources: ["inbox"]
tags: ["status/active", "status/official", "category/monitoring"]
---

# Metoro

#status/active #status/official #category/monitoring

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

## Usage

1.  Install the [Claude Desktop App](https://claude.ai/download).
2.  Make sure you have [Golang](https://golang.org/dl/) installed. `brew install go` for mac or `sudo apt-get install golang` for ubuntu.
3.  Clone the repository: `git clone https://github.com/metoro-io/metoro-mcp-server.git`
4.  Navigate to the repository directory: `cd metoro-mcp-server`
5.  Build the server executable: `go build -o metoro-mcp-server`

### If you already have a Metoro Account:

Copy your auth token from your Metoro account in [Settings](https://us-east.metoro.io/settings) -> Users Settings. Create a file in `~/Library/Application Support/Claude/claude_desktop_config.json` with the following contents:

```json
{
  "mcpServers": {
    "metoro-mcp-server": {
      "command": "<your path to Metoro MCP server go executable>/metoro-mcp-server",
      "args": [],
      "env": {
        "METORO_AUTH_TOKEN": "<your auth token>",
        "METORO_API_URL": "https://us-east.metoro.io"
      }
    }
  }
}
```

### If you don't have a Metoro Account:

No worries, you can still play around using the [Live Demo Cluster](https://demo.us-east.metoro.io/). The included token is a demo token, publicly available for anyone to use. Create a file in `~/Library/Application Support/Claude/claude_desktop_config.json` with the following contents:

```json
{
  "mcpServers": {
    "metoro-mcp-server": {
      "command": "<your path to Metoro MCP server go executable>/metoro-mcp-server",
      "args": [],
      "env": {
        "METORO_AUTH_TOKEN": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJjdXN0b21lcklkIjoiOThlZDU1M2QtYzY4ZC00MDRhLWFhZjItNDM2ODllNWJiMGUzIiwiZW1haWwiOiJ0ZXN0QGNocmlzYmF0dGFyYmVlLmNvbSIsImV4cCI6MTgyMTI0NzIzN30.7G6alDpcZh_OThYj293Jce5rjeOBqAhOlANR_Fl5auw",
        "METORO_API_URL": "https://demo.us-east.metoro.io"
      }
    }
  }
}
```

4.  Once you are done editing `claude_desktop_config.json` save the file and restart Claude Desktop app.
5.  You should now see the Metoro MCP Server in the dropdown list of MCP Servers in the Claude Desktop App. You are ready to start using Metoro MCP Server with Claude Desktop App!

## Dependencies

- Node.js >= 14.x
- Metoro account
- Metoro API key
- Kubernetes cluster
