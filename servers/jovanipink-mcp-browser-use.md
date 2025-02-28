---
type: server
repo_url: https://github.com/JovaniPink/mcp-browser-use
name: Browser Use MCP Server
owner: JovaniPink
stars: 9
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/automation",
    "purpose/browser-control",
    "category/ai",
    "purpose/web-interaction",
  ]
---

# Browser Use MCP Server

#status/active #category/automation #purpose/browser-control #category/ai #purpose/web-interaction

## Description

Enables AI agents to interact with web browsers using natural language, featuring automated browsing, form filling, vision-based element detection, and structured JSON responses for systematic browser control. The server is built on Anthropic's [Model Context Protocol (MCP)](https://modelcontextprotocol.io/introduction) and provides a seamless integration with the [browser-use](https://github.com/browser-use/browser-use) library.

## Features

1.  **Browser Control**

- Automated browser interactions via natural language
- Navigation, form filling, clicking, and scrolling capabilities
- Tab management and screenshot functionality
- Cookie and state management

2.  **Agent System**

- Custom agent implementation in custom_agent.py
- Vision-based element detection
- Structured JSON responses for actions
- Message history management and summarization

3.  **Configuration**

- Environment-based configuration for API keys and settings
- Chrome browser settings (debugging port, persistence)
- Model provider selection and parameters

## Dependencies

This project relies on the following Python packages:

- pydantic >=2.10.5
- fastapi >=0.115.6
- uvicorn >=0.22.0
- fastmcp >=0.4.1
- python-dotenv >=1.0.1
- langchain >=0.3.14
- langchain-openai >=0.2.14
- langchain-ollama >=0.2.2
- openai >=1.59.5
- browser-use ==0.1.19
- instructor >=1.7.2
- pyperclip >=1.9.0

## Usage

To install Browser Use for Claude Desktop automatically via [Smithery](https://smithery.ai/server/@JovaniPink/mcp-browser-use):

```bash
npx -y @smithery/cli install @JovaniPink/mcp-browser-use --client claude
```

Development Configuration

```json
"mcpServers": {
  "mcp_server_browser_use": {
    "command": "uvx",
    "args": [
      "mcp-server-browser-use"
    ],
    "env": {
      "OPENAI_ENDPOINT": "https://api.openai.com/v1",
      "OPENAI_API_KEY": "",
      "ANTHROPIC_API_KEY": "",
      "GOOGLE_API_KEY": "",
      "AZURE_OPENAI_ENDPOINT": "",
      "AZURE_OPENAI_API_KEY": "",
      // "DEEPSEEK_ENDPOINT": "https://api.deepseek.com",
      // "DEEPSEEK_API_KEY": "",
      // Set to false to disable anonymized telemetry
      "ANONYMIZED_TELEMETRY": "false",
      // Chrome settings
      "CHROME_PATH": "",
      "CHROME_USER_DATA": "",
      "CHROME_DEBUGGING_PORT": "9222",
      "CHROME_DEBUGGING_HOST": "localhost",
      // Set to true to keep browser open between AI tasks
      "CHROME_PERSISTENT_SESSION": "false",
      // Model settings
      "MCP_MODEL_PROVIDER": "anthropic",
      "MCP_MODEL_NAME": "claude-3-5-sonnet-20241022",
      "MCP_TEMPERATURE": "0.3",
      "MCP_MAX_STEPS": "30",
      "MCP_USE_VISION": "true",
      "MCP_MAX_ACTIONS_PER_STEP": "5",
      "MCP_TOOL_CALL_IN_CONTENT": "true"
    }
  }
}
```

## Related Servers

- adamdude828/mcp-browser-use
- Saik0s/mcp-browser-use
- hrmeetsingh/mcp-browser-automation
