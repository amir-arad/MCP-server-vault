--- 
type: server
repo_url: https://github.com/davidteren/claude-server
name: Claude Context Manager MCP Server
owner: davidteren
stars: 0
last_updated: 2025-03-01
status: active
official: false
verified: true
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/ai",
    "integration/claude",
    "purpose/context-management",
    "purpose/knowledge-organization",
    "tech/typescript",
  ]
---

# Claude Context Manager MCP Server

#status/active #category/ai #integration/claude #purpose/context-management #purpose/knowledge-organization #tech/typescript

## Description

Enhances Claude's capabilities with context management across sessions, knowledge organization through hierarchical project contexts, and continuous conversation threads stored in a well-structured directory.

## Features

- Context persistence
- Session management
- Hierarchical organization
- Project contexts
- Thread continuity
- Knowledge indexing
- Context switching
- History tracking
- Search capabilities
- Export functionality

## Installation

The server is automatically configured in your Claude desktop app's MCP settings. All contexts are stored in `~/.claude/` for better organization:

## Usage

```javascript
{
  "mcpServers": {
    "claude-context": {
      "command": "npx",
      "args": ["@davidteren/claude-server"],
      "env": {
        "STORAGE_PATH": "./contexts",
        "MAX_CONTEXTS": "100",
        "HIERARCHY_DEPTH": "5",
        "INDEX_INTERVAL": "3600",
        "BACKUP_ENABLED": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Claude API access
- Storage system
- Search indexer
- Context manager
- Backup system

## Related Servers

- modelcontextprotocol-memory-server
- claudekeep/mcp-server
- vetlefo-claude-chunks