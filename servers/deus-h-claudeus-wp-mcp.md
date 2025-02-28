---
type: server
repo_url: https://github.com/deus-h/claudeus-wp-mcp
name: Claudeus WordPress MCP Server
owner: deus-h
stars: 3
last_updated: 2025-02-15
status: active
official: false
verified: false
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/cms",
    "integration/wordpress",
    "purpose/content-management",
    "tech/rest-api",
    "category/ai",
  ]
---

# Claudeus WordPress MCP Server

#status/active #category/cms #integration/wordpress #purpose/content-management #tech/rest-api #category/ai

## Description

A server enabling seamless interaction between AI models and WordPress sites with secure, standardized communication using the WordPress REST API for comprehensive site management.

## Features

- WordPress integration
- Content management
- Post creation/editing
- Media handling
- User management
- Comment moderation
- Plugin interaction
- Theme customization
- Security controls
- API standardization

## Installation

```bash
npm install @deus-h/claudeus-wp-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "claudeus-wp": {
      "command": "npx",
      "args": ["@deus-h/claudeus-wp-mcp"],
      "env": {
        "WP_URL": "https://your-wordpress-site.com",
        "WP_USERNAME": "your-username",
        "WP_APP_PASSWORD": "your-app-password",
        "API_VERSION": "v2",
        "VERIFY_SSL": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- WordPress site
- REST API access
- Authentication tokens
- Media processor
- Content parser

## Related Servers

- modelcontextprotocol-wordpress-server
- aborroy-alfresco-mcp-poc
- akira-papa-akirapapa-mcp-notion-server
