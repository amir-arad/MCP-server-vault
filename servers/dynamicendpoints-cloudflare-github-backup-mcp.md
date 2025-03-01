--- 
type: server
repo_url: https://github.com/DynamicEndpoints/cloudflare-github-backup-mcp
name: Cloudflare GitHub Backup MCP Server
owner: DynamicEndpoints
stars: 0
last_updated: 2025-03-01
status: active
official: false
verified: true
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/backup",
    "integration/cloudflare",
    "integration/github",
    "purpose/backup",
    "purpose/disaster-recovery",
    "tech/javascript",
  ]
---

# Cloudflare GitHub Backup MCP Server

#status/active #category/backup #integration/cloudflare #integration/github #purpose/backup #purpose/disaster-recovery

## Description

Automates backing up Cloudflare configurations to GitHub repositories, enabling version control and disaster recovery for DNS, Workers, and security settings.

## Features

- Configuration backup
- GitHub integration
- Version control
- Automated scheduling
- DNS record backup
- Worker backup
- Security settings
- Change tracking
- Restore capability
- Diff generation

## Installation

```bash
npm install @dynamicendpoints/cloudflare-github-backup-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "cf-backup": {
      "command": "npx",
      "args": ["@dynamicendpoints/cloudflare-github-backup-mcp"],
      "env": {
        "CF_API_TOKEN": "your-cloudflare-token",
        "GITHUB_TOKEN": "your-github-token",
        "REPO_NAME": "your-backup-repo",
        "BACKUP_INTERVAL": "86400",
        "BACKUP_PATH": "./backups"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Cloudflare API access
- GitHub API access
- Version control system
- Backup manager
- Diff generator