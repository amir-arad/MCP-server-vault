---
type: server
repo_url: https://github.com/berlinbra/binary-reader-mcp
name: Binary Reader MCP Server
owner: berlinbra
stars: 0
last_updated: 2025-01-31
status: active
official: false
verified: false
sources: ["inbox/batch_003.md"]
tags: ["status/active", "category/development", "purpose/file-analysis", "tech/unreal-engine", "purpose/forensics"]
---

# Binary Reader MCP Server

#status/active #category/development #purpose/file-analysis #tech/unreal-engine #purpose/forensics

## Description

Analyzes Unreal Engine asset files and generic binary structures, enabling metadata extraction and file format inspection for game development and digital forensics.

## Features

- Unreal Engine asset analysis
- Binary structure parsing
- Metadata extraction
- File format inspection
- Game development support
- Digital forensics tools
- Structure validation
- Format documentation

## Installation

```bash
npm install @berlinbra/binary-reader-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "binary-reader": {
      "command": "npx",
      "args": ["@berlinbra/binary-reader-mcp"],
      "env": {
        "ASSET_PATH": "./assets",
        "UE_VERSION": "5.1",
        "METADATA_FORMAT": "json",
        "ANALYSIS_DEPTH": "full"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Unreal Engine knowledge
- Binary analysis tools
- File system access

## Related Servers

- None currently listed