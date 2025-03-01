--- 
type: server
repo_url: https://github.com/dandeliongold/mcp-decent-sampler-drums
name: DecentSampler Drums MCP Server
owner: dandeliongold
stars: 0
last_updated: 2025-03-01
status: active
official: false
verified: true
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

A Model Context Protocol server for generating DecentSampler drum kit configurations.

This TypeScript-based MCP server provides tools for working with DecentSampler drum kit presets, including WAV file analysis and XML generation.

[![Decent-Sampler Drums Server MCP server](https://camo.githubusercontent.com/22ea5f5e36f183feb216a0eb33874804ca31a8fbb21ca9c27c92c09f92802082/68747470733a2f2f676c616d612e61692f6d63702f736572766572732f706879706b757177636e2f6261646765)](https://glama.ai/mcp/servers/phypkuqwcn)

**Warning:** Creating complex presets may end up exceeding Claude Desktop's maximum message length. We are still working on streamlining this tool to work around this limitation. If you are creating simple presets without a lot of mics or other variations, the xml file should be small enough for Claude to write to a file.

## Features

- [WAV file analysis and validation](/dandeliongold/mcp-decent-sampler-drums/blob/master/docs/tools.md#analyze_wav_samples)
- [Global pitch and envelope controls](/dandeliongold/mcp-decent-sampler-drums/blob/master/docs/tools.md#configure_drum_controls)
- [Multi-mic routing with MIDI controls](/dandeliongold/mcp-decent-sampler-drums/blob/master/docs/tools.md#configure_mic_routing)
- [Round robin sample playback](/dandeliongold/mcp-decent-sampler-drums/blob/master/docs/tools.md#configure_round_robin)
- [Flexible velocity layer handling](/dandeliongold/mcp-decent-sampler-drums/blob/master/docs/schemas.md#generate_drum_groups)
- [Muting group support](/dandeliongold/mcp-decent-sampler-drums/blob/master/docs/schemas.md#generate_drum_groups)
- [Auxiliary output routing](/dandeliongold/mcp-decent-sampler-drums/blob/master/docs/tools.md#configure_mic_routing)

## Documentation

- [How do I use these tools?](/dandeliongold/mcp-decent-sampler-drums/blob/master/docs/workflows.md) - Step-by-step workflows with real examples
- [Tools Documentation](/dandeliongold/mcp-decent-sampler-drums/blob/master/docs/tools.md) - Detailed information about each available tool
- [Input Schemas](/dandeliongold/mcp-decent-sampler-drums/blob/master/docs/schemas.md) - TypeScript interfaces and parameter descriptions

## Installation

### Prerequisites

- Node.js (v14 or higher)
- npm (usually comes with Node.js)
- Claude Desktop app (for use with Claude)

### Setup

1.  Install dependencies:

npm install

2.  Build the server:

npm run build

3.  Add to your Claude Desktop config:

**Windows:** `%APPDATA%/Claude/claude_desktop_config.json` **MacOS:** `~/Library/Application Support/Claude/claude_desktop_config.json`

```json
{
  "mcpServers": {
    "decent-sampler-drums": {
      "command": "npx",
      "args": [
        "-y",
        "@dandeliongold/mcp-decent-sampler-drums"
      ],
      "env": {}
    }
  }
}
```

## Usage Guidelines

When using this MCP server to generate simple presets, you should always reference the `simple_preset_guidelines` prompt.

For more complex presets (including sections such as buses, effects, etc.), reference the `advanced_preset_guidelines` prompt. Note that creating complex presets with a large number of samples can still be unstable and may exceed Claude Desktop's maximum message length.

## About Decent Sampler

Decent Sampler is a FREE sampling plugin that allows you to play samples in the Decent Sampler format.

### Useful Links

- [Download Decent Sampler Plugin](https://www.decentsamples.com/product/decent-sampler-plugin/)
- [Decent Sampler Developer Resources](https://www.decentsamples.com/decent-sampler-developer-resources/)

### Sample Sources

The goal of this MCP server is to make it easier to set up your own presets, whether you're playing your kitchen utensils into your phone, or recording a full kit in a studio. To create your own drum kits, you'll also need samples.

If you don't already have samples ready to go, here are some resources to get started:

#### Free and Low-Cost Sample Resources

-   **99sounds.org**
    
    *   [Drum Samples Collection](https://99sounds.org/drum-samples/) - Various drum kits and percussion samples
    *   [Dub & Reggae Sounds](https://99sounds.org/dub-reggae-sounds/) - Specialized collection of reggae drum sounds
-   **Archive.org:** [Sample Pack Collection](https://archive.org/search?query=subject%3A%22Sample+Pack%22+drums&sort=-downloads) - Community-contributed drum samples, sorted by popularity. Includes some cool stuff like vintage drum machines and CMI Fairlight samples.
    
-   **Sample Pack Nation:** [Oberheim DMX/DX Drumkits](https://samplepacknation.bandcamp.com/album/oberheim-dmx-dx-drumkits-50-sounds) - Classic drum machine sounds (Under 10 USD/EUR)