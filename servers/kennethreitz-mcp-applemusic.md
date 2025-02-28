---
type: server
repo_url: https://github.com/kennethreitz/mcp-applemusic
name: Apple Music MCP Server
owner: kennethreitz
stars: 21
last_updated: 2025-02-21
status: active
official: false
verified: false
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/media", "integration/apple", "tech/applescript", "purpose/music-control"]
---

# Apple Music MCP Server

#status/active #category/media #integration/apple #tech/applescript #purpose/music-control

## Description

Facilitates controlling Apple Music on macOS via AppleScript through MCP commands, allowing users to manage playback, search for tracks, and create playlists.

## Features

- Apple Music control
- Playback management
- Track search
- Playlist creation
- Volume control
- Queue management
- Library browsing
- Metadata access

## Installation

```bash
npm install @kennethreitz/mcp-applemusic
```

## Usage

```javascript
{
  "mcpServers": {
    "apple-music": {
      "command": "npx",
      "args": ["@kennethreitz/mcp-applemusic"],
      "env": {
        "DEFAULT_PLAYLIST": "Library",
        "VOLUME_STEP": "10",
        "ALLOW_REMOTE": "true",
        "METADATA_CACHE_TTL": "300"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- macOS
- Apple Music app
- AppleScript permissions

## Related Servers

- Dhravya/apple-mcp
- joshrutkowski/applescript-mcp