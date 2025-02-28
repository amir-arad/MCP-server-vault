---
type: server
repo_url: https://github.com/kennethreitz/mcp-applemusic
name: Apple Music MCP Server
owner: kennethreitz
stars: 21
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_002.md"]
tags:
  [
    "status/active",
    "category/media",
    "integration/apple",
    "tech/applescript",
    "purpose/music-control",
  ]
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

First, ensure you have uv installed:

```bash
$ brew install uv
```

Then, with **Claude Desktop**, add the following to `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "iTunesControlServer": {
      "command": "uvx",
      "args": ["-n", "mcp-applemusic"]
    }
  }
}
```

## Available Commands

The following commands are available through the MCP server:

```
itunes_play()         # Start playback
itunes_pause()        # Pause playback
itunes_next()         # Skip to next track
itunes_previous()     # Go to previous track
itunes_search(query)  # Search library for tracks
itunes_play_song(song)  # Play specific song
itunes_create_playlist(name, songs)  # Create new playlist
itunes_library()      # Get library statistics
```

## Usage

Start the server:

```bash
python server.py
```

Example interactions:

```python
# Search for a song
results = itunes_search("Hey Jude")

# Create a new playlist
itunes_create_playlist("Beatles Favorites", ["Yesterday", "Hey Jude", "Let It Be"])

# Play a specific song
itunes_play_song("Hey Jude")
```

## Dependencies

- Node.js >= 14
- macOS
- Apple Music app
- AppleScript permissions

## Related Servers

- Dhravya/apple-mcp
- joshrutkowski/applescript-mcp
