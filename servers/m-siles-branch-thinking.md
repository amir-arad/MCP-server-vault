---
type: server
repo_url: https://github.com/m-siles/branch-thinking
name: Branch Thinking MCP Server
owner: m-siles
stars: 12
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/productivity",
    "purpose/thought-organization",
    "purpose/decision-making",
  ]
---

# Branch Thinking MCP Server

#status/active #category/productivity #purpose/thought-organization #purpose/decision-making

## Description

A server that facilitates branch-based navigation of thoughts, enabling users to manage multiple thought branches, generate insights, and track branch priorities through a structured thinking process. This is based on the `sequential-thinking` tool available here: [https://github.com/modelcontextprotocol/servers/tree/main/src/sequentialthinking](https://github.com/modelcontextprotocol/servers/tree/main/src/sequentialthinking)

## Features

- **Branch Management**: Create and navigate between different lines of thought
- **Cross References**: Link related thoughts across branches with typed relationships
- **Insights**: Automatically generate insights from key points in thoughts
- **Priority Tracking**: Track branch priorities based on confidence and connections
- Branch-based navigation
- Thought management
- Insight generation
- Priority tracking
- Structured thinking
- Branch organization
- Decision support
- Progress tracking

## Commands

- `list`: Show all branches with their current status
- `focus [branchId]`: Switch focus to a specific branch
- `history [branchId?]`: Show the history of thoughts in a branch

## Installation

Place this project in your custom MCP tool directory.

```bash
npm install
npm run build
```

Add to your `claude_desktop_config.json`:

```json
"branch-thinking": {
  "command": "node",
  "args": [    "/your-custom-mcp-dir-here/branch-thinking/dist/index.js"
  ]
}
```

## Dependencies

- Node.js >= 14
- Storage system
- Backup system
- Graph database (optional)

## Tips

Claude often will not use tools unless explicitly prompted to do so.

If you want to use this tool without being prompted, add to either your Claude Profile Settings (or a system prompt) something like so:

_If I ask you to "think step by step," "think before you respond," or "use chain of thought," that means use the branch-thinking tool. Don't hesitate to use the branch-thinking tool on your own if you think your response would benefit from multiple steps._
