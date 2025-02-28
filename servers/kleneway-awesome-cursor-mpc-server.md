---
type: server
repo_url: https://github.com/kleneway/awesome-cursor-mpc-server
name: Awesome Cursor MPC Server
owner: kleneway
stars: 174
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_003.md"]
tags:
  [
    "status/active",
    "category/development",
    "integration/cursor",
    "purpose/code-assistance",
    "category/ai",
  ]
---

# Awesome Cursor MPC Server

#status/active #category/development #integration/cursor #purpose/code-assistance #category/ai

## Description

An AI-powered development toolkit for Cursor providing intelligent coding assistance through advanced reasoning, UI screenshot analysis, and code review tools. Note that this is mostly a tutorial demo, and not a production-ready tool.

## Features

### 🎨 Code Architect

Call advanced reasoning LLMs to generate plans and instructions for coding agents.

### 📸 Screenshot Buddy

Take UI design screenshots and use them with the composer agent.

### 🔍 Code Review

Use git diffs to trigger code reviews.

- Intelligent coding assistance
- Advanced reasoning
- UI screenshot analysis
- Code review tools
- Automated suggestions
- Context awareness
- Pattern recognition
- Performance optimization

## Installation

First, you'll need to set up your environment variables. Create a file at `src/env/keys.ts`:

```typescript
export const OPENAI_API_KEY = "your_key_here";
// Add any other keys you need
```

> ⚠️ **Security Note**: Storing API keys directly in source code is not recommended for production environments. This is only for local development and learning purposes. You can set the env var inline in the Cursor MCP interface as well.

```bash
npm install
# or
yarn install
```

## Usage

This project is designed to be used as an MCP server in Cursor. Here's how to set it up:

1.  Open Cursor
2.  Go to `Cursor Settings > Features > MCP`
3.  Click `+ Add New MCP Server`
4.  Fill out the form:
    - **Name**: AI Development Assistant
    - **Type**: stdio
    - **Command**: `node /path/to/your/project/dist/index.js`

> 📘 **Pro Tip**: You might need to use the full path to your project's built index.js file.

After adding the server, you should see your tools listed under "Available Tools". If not, try clicking the refresh button in the top right corner of the MCP server section.

For more details about MCP setup, check out the [Cursor MCP Documentation](https://docs.cursor.com/advanced/model-context-protocol).

## Dependencies

- Node.js >= 16
- Cursor editor
- AI model access
- Screenshot capabilities
