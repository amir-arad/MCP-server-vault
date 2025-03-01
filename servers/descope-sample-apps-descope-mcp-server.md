--- 
type: server
repo_url: https://github.com/descope-sample-apps/descope-mcp-server
name: Descope Management MCP Server
owner: descope-sample-apps
stars: 2
last_updated: 2025-03-01
status: active
official: true
verified: true
sources: ["inbox/batch_009.md"]
tags:
  [
    "status/active",
    "status/official",
    "category/management",
    "integration/descope",
    "purpose/user-management",
    "purpose/auditing",
  ]
---

# Descope Management MCP Server

#status/active #status/official #category/management #integration/descope #purpose/user-management #purpose/auditing

## Description

Interact with Descope's Management APIs to manage users, audit, and more. This server provides comprehensive access to Descope's user management and auditing capabilities.

## Features

- User management
- Audit logging
- Access control
- Role management
- Permission handling
- Activity tracking
- Report generation
- Security controls
- API integration
- Event monitoring

## Installation

```bash
npm install @descope-sample-apps/descope-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "descope": {
      "command": "npx",
      "args": ["@descope-sample-apps/descope-mcp"],
      "env": {
        "DESCOPE_PROJECT_ID": "your-project-id",
        "DESCOPE_API_KEY": "your-api-key",
        "AUDIT_ENABLED": "true",
        "LOG_LEVEL": "info",
        "RETENTION_DAYS": "30"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Descope account
- API credentials
- Audit logger
- User manager
- Report generator

## Related Servers

- modelcontextprotocol-management-server
- nahmanmate-better-auth-mcp-server
- modelcontextprotocol-audit-server