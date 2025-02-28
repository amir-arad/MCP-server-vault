---
type: server
repo_url: https://github.com/dandeliongold/mcp-decent-sampler-drums
name: DecentSampler Drums MCP Server
owner: dandeliongold
stars: 0
last_updated: 2025-02-17
status: active
official: false
verified: false
sources: ["inbox/batch_008.md"]
tags:
  [
    "status/active",
    "category/audio",
    "integration/decent-sampler",
    "purpose/drum-kits",
    "tech/wav",
    "tech/xml",
  ]
---

# DecentSampler Drums MCP Server

#status/active #category/audio #integration/decent-sampler #purpose/drum-kits #tech/wav #tech/xml

## Description

Facilitates the creation of DecentSampler drum kit configurations, supporting WAV file analysis and XML generation to ensure accurate sample lengths and well-structured presets.

## Features

- Drum kit configuration
- WAV file analysis
- XML generation
- Sample length detection
- Preset structuring
- Audio processing
- Configuration validation
- Metadata handling
- Batch processing
- Template support

## Installation

```bash
npm install @dandeliongold/decent-sampler-drums-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "decent-sampler": {
      "command": "npx",
      "args": ["@dandeliongold/decent-sampler-drums-mcp"],
      "env": {
        "SAMPLES_PATH": "./drum-samples",
        "OUTPUT_PATH": "./presets",
        "DEFAULT_FORMAT": "24bit",
        "AUTO_NORMALIZE": "true",
        "TEMPLATE_PATH": "./templates"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- WAV file analyzer
- XML generator
- Audio processor
- Template engine
- Validation tools

## Related Servers

- modelcontextprotocol-audio-server
- mamertofabian-audio-mcp-server
- modelcontextprotocol-music-server
