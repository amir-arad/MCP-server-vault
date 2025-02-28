--- 
type: server
repo_url: https://github.com/ZilongXue/claude-post
name: ClaudePost MCP Server
owner: ZilongXue
stars: 22
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/communication",
    "integration/gmail",
    "purpose/email-management",
    "tech/typescript",
    "category/ai",
  ]
---

# ClaudePost MCP Server

#status/active #category/communication #integration/gmail #purpose/email-management #tech/typescript #category/ai

## Description

A Model Context Protocol (MCP) server that provides a seamless email management interface through Claude. This integration allows you to handle emails directly through natural language conversations with Claude, supporting features like searching, reading, and sending emails securely.

## Features

- Email search functionality
- Email reading
- Email composition
- Secure authentication
- Attachment handling
- Label management
- Thread organization
- Draft management
- Contact integration
- Filter creation

## Installation

1.  Install uv:
    
    ```bash
    # MacOS/Linux
    curl -LsSf https://astral.sh/uv/install.sh | sh
    
    # Remember to restart your terminal after installation
    ```
    
2.  Clone and set up the project:
    
    ```bash
    # Clone the repository
    git clone https://github.com/ZilongXue/claude-post.git
    cd claude-post
    
    # Create and activate virtual environment
    uv venv
    source .venv/bin/activate  # On Windows: .venv\\Scripts\\activate
    
    # Install dependencies
    uv pip install -e .
    ```
    
3.  Create a `.env` file in the project root:
    
    ```
    EMAIL_ADDRESS=your.email@gmail.com
    EMAIL_PASSWORD=your-app-specific-password
    IMAP_SERVER=imap.gmail.com
    SMTP_SERVER=smtp.gmail.com
    SMTP_PORT=587
    ```
    
4.  Configure Claude Desktop:
    
    First, make sure you have Claude for Desktop installed. You can install the latest version [here](https://claude.ai/download). If you already have Claude for Desktop, make sure it's updated to the latest version.
    
    Open your Claude Desktop configuration file:
    
    ```
    # MacOS
    ~/Library/Application Support/Claude/claude_desktop_config.json
    
    # Create the file if it doesn't exist
    mkdir -p ~/Library/Application\\ Support/Claude
    touch ~/Library/Application\\ Support/Claude/claude_desktop_config.json
    ```
    
    Add the following configuration:
    
    ```json
    {
     "mcpServers": {
       "email": {
         "command": "/Users/username/.local/bin/uv",
         "args": [
           "--directory",
           "/path/to/claude-post/src/email_client",
           "run",
           "email-client"
         ]
       }
     }
    }
    ```
    
    Replace `/Users/username` and `/path/to/claude-post` with your actual paths.
    
    After updating the configuration, restart Claude Desktop for the changes to take effect.

## Usage

```javascript
{
  "mcpServers": {
    "claude-post": {
      "command": "npx",
      "args": ["@zilongxue/claude-post"],
      "env": {
        "GMAIL_CLIENT_ID": "your-client-id",
        "GMAIL_CLIENT_SECRET": "your-client-secret",
        "OAUTH_REFRESH_TOKEN": "your-refresh-token",
        "MAX_RESULTS": "100",
        "CACHE_DURATION": "3600"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Gmail API access
- OAuth 2.0 credentials
- Email parser
- MIME handler
- Cache system

## Related Servers

- apicolet-brevo-mcp
- r3-yamauchi-mcp-server-blastengine-mailer
- modelcontextprotocol-gmail-server