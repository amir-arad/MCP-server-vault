--- 
type: server
repo_url: https://github.com/ztobs/cline-browser-use-mcp
name: Cline Browser Automation MCP Server
owner: ztobs
stars: 12
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/automation",
    "tech/python",
    "purpose/browser-automation",
    "purpose/web-scraping",
    "tech/selenium",
  ]
---

# Cline Browser Automation MCP Server

#status/active #category/automation #tech/python #purpose/browser-automation #purpose/web-scraping #tech/selenium

## Description

Enables browser automation using Python scripts, offering operations like taking webpage screenshots, retrieving HTML content, and executing JavaScript. This MCP server provides comprehensive browser control capabilities.

## Features

- Screenshot capture
- HTML extraction
- JavaScript execution
- Browser automation
- Element interaction
- Page navigation
- Cookie management
- Form handling
- Network monitoring
- Error recovery

## Installation

### Installing via Smithery

To install Browser Use Server for Claude Desktop automatically via [Smithery](https://smithery.ai/server/@ztobs/cline-browser-use-mcp):

```bash
npx -y @smithery/cli install @ztobs/cline-browser-use-mcp --client claude
```

1.  Clone this repository
2.  Install dependencies:

```bash
npm install
```

3.  Build the server:

```bash
npm run build
```

## MCP Configuration

Add the following configuration to your Cline MCP settings:

```json
"browser-use": {
  "command": "node",
  "args": [
    "/home/YOUR_HOME/Documents/Cline/MCP/browser-use-server/build/index.js"
  ],
  "env": {
    // Required: Set at least one API key
    "GLHF_API_KEY": "your_api_key",
    "GROQ_API_KEY": "your_api_key",
    "OPENAI_API_KEY": "your_api_key",
    "OPENROUTER_API_KEY": "your_api_key",
    "GITHUB_API_KEY": "your_api_key",
    "DEEPSEEK_API_KEY": "your_api_key",
    "GEMINI_API_KEY": "your_api_key",
    "OLLAMA_API_KEY": "your_api_key",
    // Optional: Configuration overrides
    "MODEL": "your_preferred_model",
    "BASE_URL": "your_custom_url",
    "USE_VISION": "false"
  },
  "disabled": false,
  "autoApprove": []
}
```

Replace:

*   `YOUR_HOME` with your actual home directory name
*   `your_api_key` with your actual API keys

## Usage

Here are some example tasks you can accomplish using the browser-use server with Cline:

### Modifying Web Page Elements during Development

To change the color of a heading on a page that requires authentication:

```
Change the colour of the headline with the text "Alle Foren im Überblick." to deep blue on https://localhost:3000/foren/ page

To check/see the page, use browser-use MCP server to:
Open https://localhost:3000/auth,
Login with ztobs:Password123,
Navigate to https://localhost:3000/foren/,
Accept cookies if required

hint: execute all browser actions in one command with multiple comma-separated steps
```

This task demonstrates:

*   Multi-step browser automation using comma-separated steps
*   Authentication handling
*   Cookie acceptance
*   DOM manipulation
*   CSS styling changes

The server will execute these steps sequentially, handling any required interactions along the way.

## Dependencies

- Python >= 3.8
- Selenium WebDriver
- Chrome/Firefox browser
- Screenshot library
- HTML parser
- JavaScript executor

## Related Servers

- modelcontextprotocol-puppeteer-server
- hrmeetsingh-mcp-browser-automation
- browserbase-mcp-server-browserbase