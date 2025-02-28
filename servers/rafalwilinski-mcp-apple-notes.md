---
type: server
repo_url: https://github.com/RafalWilinski/mcp-apple-notes
name: Apple Notes MCP Server
owner: RafalWilinski
stars: 119
last_updated: 2025-02-21
status: active
official: false
verified: false
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/productivity", "integration/apple", "purpose/note-management", "tech/macos"]
---

# Apple Notes MCP Server

#status/active #category/productivity #integration/apple #purpose/note-management #tech/macos

## Description

Enables semantic search and RAG (Retrieval Augmented Generation) over your Apple Notes.

## Features

- Semantic search
- RAG capabilities
- Notes indexing
- Content retrieval
- Natural language queries
- Vector embeddings
- Context-aware search
- Real-time updates

## Installation

```bash
npm install @rafalwilinski/mcp-apple-notes
```

## Usage

```javascript
{
  "mcpServers": {
    "apple-notes": {
      "command": "npx",
      "args": ["@rafalwilinski/mcp-apple-notes"],
      "env": {
        "NOTES_DB_PATH": "~/Library/Group Containers/group.com.apple.notes/NoteStore.sqlite",
        "EMBEDDING_MODEL": "all-mpnet-base-v2",
        "INDEX_UPDATE_INTERVAL": "300",
        "MAX_RESULTS": "10"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- macOS
- Apple Notes app
- Vector database (optional)

## Related Servers

- Dhravya/apple-mcp
- sirmews/apple-notes-mcp
- turlockmike/apple-notifier-mcp