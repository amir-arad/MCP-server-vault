---
type: server
repo_url: https://github.com/turlockmike/chess-mcp
name: Chess Analysis MCP Server
owner: turlockmike
stars: 2
last_updated: 2025-02-08
status: active
official: false
verified: false
sources: ["inbox/batch_005.md"]
tags:
[
"status/active",
"category/games",
"integration/stockfish",
"purpose/analysis",
"tech/chess",
]

---

# Chess Analysis MCP Server

#status/active #category/games #integration/stockfish #purpose/analysis #tech/chess

## Description

Helps you analyze chess positions and get professional evaluations using Stockfish. This MCP server provides deep chess position analysis and strategic insights powered by the Stockfish chess engine.

## Features

- Position evaluation
- Move analysis
- Best move suggestions
- Line calculation
- Opening book access
- Endgame tablebases
- Game analysis
- PGN parsing
- FEN support
- Stockfish integration

## Installation

```bash
npm install @turlockmike/chess-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "chess": {
      "command": "npx",
      "args": ["@turlockmike/chess-mcp"],
      "env": {
        "STOCKFISH_PATH": "/usr/local/bin/stockfish",
        "ANALYSIS_DEPTH": "20",
        "MULTI_PV": "3",
        "HASH_SIZE": "128",
        "THREADS": "4"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Stockfish chess engine
- Chess.js library
- PGN parser
- Opening book database
- Endgame tablebases (optional)

## Related Servers

- None currently listed
