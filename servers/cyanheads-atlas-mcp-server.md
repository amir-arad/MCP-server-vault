---
type: server
repo_url: https://github.com/cyanheads/atlas-mcp-server
name: ATLAS MCP Server
owner: cyanheads
stars: 88
last_updated: 2025-03-01
status: active
official: false
verified: true
sources: ["inbox/batch_002.md"]
tags:
  [
    "status/active",
    "category/task-management",
    "category/ai",
    "purpose/workflow-automation",
  ]
---

# ATLAS MCP Server

#status/active #category/task-management #category/ai #purpose/workflow-automation

## Description

ATLAS (Adaptive Task & Logic Automation System) is a Model Context Protocol server that provides hierarchical task management capabilities to Large Language Models. This tool provides LLMs with the structure and context needed to manage complex tasks and dependencies.

## Features

- Hierarchical task management
- Dependency tracking
- Task automation
- Context management
- LLM integration
- Workflow optimization
- Progress monitoring
- Resource allocation

## Installation

```bash
npm install atlas-mcp-server
```

## Usage

```javascript
{
  "mcpServers": {
    "atlas": {
      "command": "npx",
      "args": ["@cyanheads/atlas-mcp"],
      "env": {
        "TASK_STORAGE": "./tasks",
        "MAX_DEPTH": "5",
        "AUTO_CLEANUP": "true",
        "CONTEXT_TTL": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Storage system
- LLM integration
- Task scheduler

## Related Servers

- None currently listed
