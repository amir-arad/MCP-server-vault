---
type: server
repo_url: https://github.com/squirrelogic/mcp-architect
name: Architect MCP Server
owner: squirrelogic
stars: 12
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_002.md"]
tags:
  [
    "status/active",
    "category/architecture",
    "purpose/design",
    "category/ai",
    "tech/cloud",
    "tech/nodejs",
  ]
---

# Architect MCP Server

#status/active #category/architecture #purpose/design #category/ai #tech/cloud

## Description

Facilitates comprehensive architectural design and evaluation through specialized agents, rich resources, and powerful tools covering diverse architectural domains, including cloud, AI, and blockchain.

## Features

- Architectural design assistance
- Specialized agents
- Resource management
- Domain expertise
- Cloud architecture
- AI system design
- Blockchain architecture
- Design evaluation

## Installation

```bash
npm install @squirrelogic/mcp-architect
```

## Usage

```javascript
{
  "mcpServers": {
    "architect": {
      "command": "npx",
      "args": ["@squirrelogic/mcp-architect"],
      "env": {
        "DOMAINS": "cloud,ai,blockchain",
        "EVALUATION_DEPTH": "comprehensive",
        "RESOURCE_PATH": "./resources",
        "AGENT_CONFIG": "./agents.json"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Domain-specific tools
- Resource libraries
- Agent frameworks

## Related Servers

- stevennevins/architect-mcp-server
