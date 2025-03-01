--- 
type: server
repo_url: https://github.com/davidvc/code-mcp
name: Code Graph Analysis MCP Server
owner: davidvc
stars: 4
last_updated: 2025-03-01
status: active
official: false
verified: true
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/development",
    "integration/neo4j",
    "purpose/code-analysis",
    "tech/graph-database",
    "purpose/structural-analysis",
  ]
---

# Code Graph Analysis MCP Server

#status/active #category/development #integration/neo4j #purpose/code-analysis #tech/graph-database #purpose/structural-analysis

## Description

Integrates code analysis using a Neo4j graph database to enable structural insights, quality metrics, and natural language querying of codebases.

## Features

- Graph-based analysis
- Code structure mapping
- Quality metrics
- Natural language queries
- Dependency tracking
- Pattern detection
- Impact analysis
- Relationship mapping
- Metric collection
- Visual insights

## Installation

```bash
npm install @davidvc/code-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "code-graph": {
      "command": "npx",
      "args": ["@davidvc/code-mcp"],
      "env": {
        "NEO4J_URI": "bolt://localhost:7687",
        "NEO4J_USER": "neo4j",
        "NEO4J_PASSWORD": "your-password",
        "PROJECT_PATH": "./",
        "SCAN_INTERVAL": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Neo4j database
- Graph algorithms
- Code parser
- Query engine
- Visualization tools

## Related Servers

- davidvc/code-knowledge-mcptool
- seanivore/mcp-code-analyzer
- neo4j-contrib-mcp-neo4j