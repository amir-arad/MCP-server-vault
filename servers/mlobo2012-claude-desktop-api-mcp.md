---
type: server
repo_url: https://github.com/mlobo2012/Claude_Desktop_API_USE_VIA_MCP
name: Claude Desktop API MCP Server
owner: mlobo2012
stars: 2
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/ai",
    "integration/claude",
    "purpose/api-access",
    "purpose/conversation-management",
    "tech/typescript",
  ]
---

# Claude Desktop API MCP Server

#status/active #category/ai #integration/claude #purpose/api-access #purpose/conversation-management #tech/typescript

## Description

Integrates Claude API features, enabling direct API access, extended context windows, and advanced conversation management. Helpful to bypass standard daily limits of Claude.ai.

## Features

- Direct Claude API integration via MCP
- Conversation history tracking and management
- System prompt support
- Seamless switching between Professional Plan and API usage
- Easy configuration with Claude Desktop

## Usage

To use this server in an MCP client such as Claude Desktop:

1.  **Clone the Repository**

    # Using VS Code:

    # 1. Press Cmd + Shift + P

    # 2. Type "Git: Clone"

    # 3. Paste: https://github.com/mlobo2012/Claude\_Desktop\_API\_USE\_VIA\_MCP.git

    # Or using terminal:

    git clone https://github.com/mlobo2012/Claude\_Desktop\_API\_USE\_VIA\_MCP.git
    cd Claude_Desktop_API_USE_VIA_MCP

2.  **Install Dependencies**

    ```bash
    pip install -r requirements.txt
    ```

3.  **Configure Environment**

    # Copy environment template

    cp .env.example .env

    # Edit .env and add your API key

    ANTHROPIC_API_KEY=your_api_key_here

4.  **Configure Claude Desktop**

    - macOS: Navigate to `~/Library/Application Support/Claude/`

      # Using Finder:

      # 1. Press Cmd + Shift + G

      # 2. Enter: ~/Library/Application Support/Claude/

    - Windows: Navigate to `%APPDATA%\Claude\`
    - Create or edit `claude_desktop_config.json`
    - Copy contents from `config/claude_desktop_config.json`
    - Update paths and API keys

## Dependencies

- Node.js >= 16
- Claude API key
- TypeScript runtime
- WebSocket support
- Storage backend
- Rate limiter
