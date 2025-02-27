---
repo_url: https://github.com/axiomhq/mcp-server-axiom
owner: axiomhq
name: mcp-server-axiom
stars: 10
last_updated: 2025-02-20
status: active
official: true
verified: false
sources:
  - inbox
tags:
  - status/active
  - status/official
  - category/database
  - category/analytics
  - tech/go
  - purpose/data-analysis
  - integration/axiom
---

# Axiom

#status/active #status/official #category/database #category/analytics #tech/go #purpose/data-analysis #integration/axiom

## Description

A Model Context Protocol server implementation for Axiom that enables AI agents to query and analyze logs, traces, and all other event data in natural language using Axiom Processing Language (APL).

## Features

- Execute APL queries against Axiom datasets
- List available Axiom datasets
- Rate limiting control for API requests
- Flexible configuration options (config file, command line flags, environment variables)
- Seamless integration with Claude desktop app

## Installation

### From Releases:

Download the latest built binary from the [releases page](https://github.com/axiomhq/axiom-mcp/releases).

### From Source:

```bash
go install github.com/axiomhq/axiom-mcp@latest
```

## Configuration

Configure using one of these methods:

### Config File Example (config.txt):

```
token xaat-your-token
url https://api.axiom.co
query-rate 1
query-burst 1
datasets-rate 1
datasets-burst 1
```

### Command Line Flags:

```bash
axiom-mcp \
  -token xaat-your-token \
  -url https://api.axiom.co \
  -query-rate 1 \
  -query-burst 1 \
  -datasets-rate 1 \
  -datasets-burst 1
```

### Environment Variables:

```bash
export AXIOM_TOKEN=xaat-your-token
export AXIOM_URL=https://api.axiom.co
export AXIOM_ORG_ID=your-org-id
export AXIOM_QUERY_RATE=1
export AXIOM_QUERY_BURST=1
export AXIOM_DATASETS_RATE=1
export AXIOM_DATASETS_BURST=1
```

## Usage with Claude

1. Create a config file:

```bash
echo "token xaat-your-token" > config.txt
```

2. Configure the Claude app to use the MCP server:

```json
{
  "mcpServers": {
    "axiom": {
      "command": "/path/to/your/axiom-mcp-binary",
      "args": ["--config", "/path/to/your/config.txt"],
      "env": {
        "AXIOM_TOKEN": "xaat-your-token",
        "AXIOM_URL": "https://api.axiom.co",
        "AXIOM_ORG_ID": "your-org-id"
      }
    }
  }
}
```

## Dependencies

- Go compiler (if building from source)
- Axiom account with API token

## Related Servers

- [Grafana](https://github.com/grafana/mcp-grafana)
- [Tinybird](https://github.com/tinybirdco/mcp-tinybird)
- [Postgres](https://github.com/modelcontextprotocol/servers/tree/main/src/postgres)
