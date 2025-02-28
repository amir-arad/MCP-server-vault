---
type: server
repo_url: https://github.com/mamertofabian/elevenlabs-mcp-server
name: ElevenLabs MCP Server
owner: mamertofabian
stars: 11
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_010.md"]
tags:
  [
    "status/active",
    "category/audio",
    "integration/elevenlabs",
    "purpose/text-to-speech",
    "tech/api",
    "purpose/voice-synthesis",
  ]
---

# ElevenLabs MCP Server

#status/active #category/audio #integration/elevenlabs #purpose/text-to-speech #tech/api #purpose/voice-synthesis

## Description

A Model Context Protocol (MCP) server that integrates with ElevenLabs text-to-speech API, featuring both a server component and a sample web-based MCP Client (SvelteKit) for managing voice generation tasks.

## Features

- Generate audio from text using ElevenLabs API
- Support for multiple voices and script parts
- SQLite database for persistent history storage
- Sample SvelteKit MCP Client for:
  - Simple text-to-speech conversion
  - Multi-part script management
  - Voice history tracking and playback
  - Audio file downloads
- Text-to-speech conversion
- Voice selection
- Speech customization
- Audio format options
- Voice cloning
- Batch processing
- Real-time synthesis
- Voice style control
- Audio file management
- API rate limiting

## Installation

### Installing via Smithery

To install ElevenLabs MCP Server for Claude Desktop automatically via [Smithery](https://smithery.ai/server/elevenlabs-mcp-server):

```bash
npx -y @smithery/cli install elevenlabs-mcp-server --client claude
```

### Using uvx (recommended)

When using [`uvx`](https://docs.astral.sh/uv/guides/tools/), no specific installation is needed.

Add the following configuration to your MCP settings file (e.g., `cline_mcp_settings.json` for Claude Desktop):

```json
{
  "mcpServers": {
    "elevenlabs": {
      "command": "uvx",
      "args": ["elevenlabs-mcp-server"],
      "env": {
        "ELEVENLABS_API_KEY": "your-api-key",
        "ELEVENLABS_VOICE_ID": "your-voice-id",
        "ELEVENLABS_MODEL_ID": "eleven_flash_v2",
        "ELEVENLABS_STABILITY": "0.5",
        "ELEVENLABS_SIMILARITY_BOOST": "0.75",
        "ELEVENLABS_STYLE": "0.1",
        "ELEVENLABS_OUTPUT_DIR": "output"
      }
    }
  }
}
```

### Development Installation

1.  Clone this repository
2.  Install dependencies:

    ```bash
    uv venv
    ```

3.  Copy `.env.example` to `.env` and fill in your ElevenLabs credentials

## Using the Sample SvelteKit MCP Client

1.  Navigate to the web UI directory:

    ```bash
    cd clients/web-ui
    ```

2.  Install dependencies:

    ```bash
    pnpm install
    ```

3.  Copy `.env.example` to `.env` and configure as needed
4.  Run the web UI:

    ```bash
    pnpm dev
    ```

5.  Open [http://localhost:5174](http://localhost:5174) in your browser

### Available Tools

- `generate_audio_simple`: Generate audio from plain text using default voice settings
- `generate_audio_script`: Generate audio from a structured script with multiple voices and actors
- `delete_job`: Delete a job by its ID
- `get_audio_file`: Get the audio file by its ID
- `list_voices`: List all available voices
- `get_voiceover_history`: Get voiceover job history. Optionally specify a job ID for a specific job.

### Available Resources

- `voiceover://history/{job_id}`: Get the audio file by its ID
- `voiceover://voices`: List all available voices
