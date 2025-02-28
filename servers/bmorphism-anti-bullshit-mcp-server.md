---
type: server
repo_url: https://github.com/bmorphism/anti-bullshit-mcp-server
name: Anti Bullshit MCP Server
owner: bmorphism
stars: 11
last_updated: 2025-02-05
status: active
official: false
verified: false
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/verification", "purpose/fact-checking", "category/ai"]
---

# Anti Bullshit MCP Server

#status/active #category/verification #purpose/fact-checking #category/ai

## Description

Enables analysis of claims, validation of sources, and detection of manipulation using multiple epistemological frameworks to ensure credible and ethical information.

## Features

- Claim analysis
- Source validation
- Manipulation detection
- Epistemological frameworks
- Credibility assessment
- Ethical information verification
- Bias detection
- Citation checking

## Installation

```bash
npm install @bmorphism/anti-bullshit-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "anti-bullshit": {
      "command": "npx",
      "args": ["@bmorphism/anti-bullshit-mcp"],
      "env": {
        "VERIFICATION_LEVEL": "strict",
        "SOURCE_CHECK_DEPTH": "3",
        "FRAMEWORKS": "scientific,journalistic,academic",
        "CONFIDENCE_THRESHOLD": "0.85"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Fact-checking APIs
- Source databases
- NLP models

## Related Servers

- None currently listed