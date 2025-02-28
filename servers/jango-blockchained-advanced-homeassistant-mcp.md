---
type: server
repo_url: https://github.com/jango-blockchained/advanced-homeassistant-mcp
name: Advanced Home Assistant MCP Server
owner: jango-blockchained
stars: 3
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_001.md"]
tags: ["status/active", "category/home-automation", "integration/home-assistant", "purpose/device-control", "tech/typescript", "tech/bun", "feature/speech-recognition"]
---

# Advanced Home Assistant MCP Server

#status/active #category/home-automation #integration/home-assistant #purpose/device-control #tech/typescript #tech/bun #feature/speech-recognition

## Description

A comprehensive MCP server for Home Assistant integration, providing intelligent device control and monitoring capabilities with context-aware organization. Built with Bun for maximum performance, this server offers flexible interfaces for device management and automation, with optional speech recognition features.

## Features

- Smart Device Control:
  - Lights: Brightness, color, RGB control
  - Climate: Temperature, HVAC, humidity management
  - Covers: Position and tilt control
  - Switches: On/off functionality
  - Sensors: State monitoring
- Intelligent Organization:
  - Context-aware grouping
  - Smart device categorization
- Robust Architecture:
  - Error handling
  - State validation
  - Real-time updates
- WebSocket/Server-Sent Events (SSE) for state updates
- JWT-based authentication
- Optional Speech Features:
  - Wake word detection ("hey jarvis", "ok google", "alexa")
  - Speech-to-text using fast-whisper
  - Multiple language support
  - GPU acceleration support

## Installation

```bash
# Clone the repository
git clone https://github.com/jango-blockchained/advanced-homeassistant-mcp.git
cd advanced-homeassistant-mcp

# Set up the environment
chmod +x scripts/setup-env.sh
./scripts/setup-env.sh

# Build and launch with Docker
./docker-build.sh
docker compose up -d

# With speech features
./docker-build.sh --speech
docker compose -f docker-compose.yml -f docker-compose.speech.yml up -d
```

## Usage

```javascript
{
  "mcpServers": {
    "homeassistant-mcp": {
      "command": "bun",
      "args": ["run", "start"],
      "env": {
        "HASS_URL": "http://your-homeassistant:8123",
        "HASS_TOKEN": "your-long-lived-access-token",
        "REFRESH_INTERVAL": "5000",
        "ENABLE_SPEECH_FEATURES": "false"
      }
    }
  }
}
```

## Dependencies

- Bun runtime (v1.0.26+)
- Home Assistant instance
- Docker (optional, recommended for deployment)
- Node.js 18+ (optional, for speech features)
- NVIDIA GPU with CUDA support (optional, for faster speech processing)

## Related Servers

- [Home Assistant Companion](https://github.com/modelcontextprotocol/servers/tree/main/src/home-assistant) - Official MCP server for Home Assistant
- [Smart Home Hub](https://github.com/example/smart-home-hub-mcp) - Generic smart home integration server