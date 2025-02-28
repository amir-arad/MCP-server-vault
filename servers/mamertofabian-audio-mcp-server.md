---
type: server
repo_url: https://github.com/mamertofabian/audio-mcp-server
name: Audio MCP Server
owner: mamertofabian
stars: 1
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_003.md"]
tags:
  [
    "status/active",
    "category/audio",
    "tech/play-sound",
    "purpose/sound-playback",
  ]
---

# Audio MCP Server

#status/active #category/audio #tech/play-sound #purpose/sound-playback

## Description

Integrates with the play-sound library to enable cross-platform audio playback for voice notifications, sound effects, and audio cues.

## Features

- Cross-platform audio playback
- Voice notifications
- Sound effects
- Audio cues
- Format support
- Volume control
- Playback management
- Event handling

## Installation

```bash
npm install @mamertofabian/audio-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "audio": {
      "command": "npx",
      "args": ["@mamertofabian/audio-mcp"],
      "env": {
        "AUDIO_PATH": "./sounds",
        "DEFAULT_VOLUME": "1.0",
        "ALLOWED_FORMATS": ".mp3,.wav,.ogg",
        "MAX_DURATION": "30"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- play-sound library
- Audio output device
- Audio codecs

## Related Servers

- None currently listed
