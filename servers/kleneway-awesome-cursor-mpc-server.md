---
type: server
repo_url: https://github.com/kleneway/awesome-cursor-mpc-server
name: Awesome Cursor MPC Server
owner: kleneway
stars: 174
last_updated: 2025-02-21
status: active
official: false
verified: false
sources: ["inbox/batch_003.md"]
tags: ["status/active", "category/development", "integration/cursor", "purpose/code-assistance", "category/ai"]
---

# Awesome Cursor MPC Server

#status/active #category/development #integration/cursor #purpose/code-assistance #category/ai

## Description

An AI-powered development toolkit for Cursor providing intelligent coding assistance through advanced reasoning, UI screenshot analysis, and code review tools.

## Features

- Intelligent coding assistance
- Advanced reasoning
- UI screenshot analysis
- Code review tools
- Automated suggestions
- Context awareness
- Pattern recognition
- Performance optimization

## Installation

```bash
npm install @kleneway/awesome-cursor-mpc
```

## Usage

```javascript
{
  "mcpServers": {
    "cursor": {
      "command": "npx",
      "args": ["@kleneway/awesome-cursor-mpc"],
      "env": {
        "AI_MODEL": "gpt-4",
        "SCREENSHOT_PATH": "./screenshots",
        "CODE_CONTEXT_DEPTH": "3",
        "ANALYSIS_TIMEOUT": "30000"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Cursor editor
- AI model access
- Screenshot capabilities

## Related Servers

- None currently listed