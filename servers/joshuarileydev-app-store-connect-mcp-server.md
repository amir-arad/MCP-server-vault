---
type: server
repo_url: https://github.com/JoshuaRileyDev/app-store-connect-mcp-server
name: App Store Connect MCP Server
owner: JoshuaRileyDev
stars: 8
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_002.md"]
tags: ["status/active", "category/development", "integration/apple", "purpose/app-management", "tech/typescript", "integration/app-store-connect", "category/mobile"]
---

# App Store Connect MCP Server

#status/active #category/development #integration/apple #purpose/app-management #tech/typescript #integration/app-store-connect #category/mobile

## Description

A Model Context Protocol (MCP) server for interacting with the App Store Connect API. This server provides comprehensive tools for iOS developers to manage their applications, beta testing programs, bundle IDs, devices, and user permissions directly through Claude, streamlining the app development and release workflow.

## Features

- App Management:
  - List all apps in App Store Connect
  - Get detailed app information
  - View app metadata and relationships
- Beta Testing:
  - List beta groups and testers
  - Add/remove testers from groups
  - Manage beta test configurations
- Bundle ID Management:
  - List registered bundle IDs
  - Create new bundle IDs
  - Get bundle ID details
  - Enable/disable capabilities
- Device Management:
  - List registered devices
  - Filter by device type, platform, status
  - View device details
- User Management:
  - List team members
  - View user roles and permissions
  - Filter users by role and access

## Installation

```bash
npm install @joshuarileydev/app-store-connect-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "app-store-connect": {
      "command": "npx",
      "args": [
        "-y",
        "@joshuarileydev/app-store-connect-mcp"
      ],
      "env": {
        "APP_STORE_CONNECT_KEY_ID": "YOUR_KEY_ID",
        "APP_STORE_CONNECT_ISSUER_ID": "YOUR_ISSUER_ID",
        "APP_STORE_CONNECT_P8_PATH": "/path/to/your/auth-key.p8"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- TypeScript
- App Store Connect API key (generated from App Store Connect portal)
- Apple Developer account with appropriate permissions
- JWT authentication via .p8 private key file

## Related Servers

- dhravya-apple-mcp - General Apple services integration
- joshrutkowski-applescript-mcp - AppleScript automation for macOS
- kennethreitz-mcp-applemusic - Apple Music API integration
- modelcontextprotocol/github-server - Similar integration pattern for GitHub