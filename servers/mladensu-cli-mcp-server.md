---
type: server
repo_url: https://github.com/MladenSU/cli-mcp-server
name: CLI MCP Server
owner: MladenSU
stars: 29
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/system",
    "purpose/cli",
    "purpose/security",
    "tech/typescript",
    "category/automation",
  ]
---

# CLI MCP Server

#status/active #category/system #purpose/cli #purpose/security #tech/typescript #category/automation

## Description

Command line interface with secure execution and customizable security policies. This MCP server provides a secure environment for executing CLI commands with configurable permissions and restrictions.

## Features

- Secure command execution
- Security policy management
- Command whitelisting
- Permission controls
- Output sanitization
- Environment isolation
- Audit logging
- Resource limits
- Error handling
- Policy templates

## Installation

```bash
npm install @mladensu/cli-mcp-server
```

## Usage

```javascript
{
  "mcpServers": {
    "cli": {
      "command": "npx",
      "args": ["@mladensu/cli-mcp-server"],
      "env": {
        "POLICY_PATH": "./security-policies.json",
        "ALLOWED_COMMANDS": "git,npm,node",
        "MAX_EXECUTION_TIME": "30",
        "LOG_LEVEL": "info",
        "SANDBOX_MODE": "strict"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Security policy engine
- Command executor
- Audit logger
- Sandbox environment
- Policy validator

## Related Servers

- modelcontextprotocol-terminal-server
- wonderwhy-er-claudecomputercommander
- andre-jesus-claude-mcp
