---
type: server
repo_url: https://github.com/twolven/mcp-codesavant
name: CodeSavant MCP Server
owner: twolven
stars: 5
last_updated: 2025-02-06
status: active
official: false
verified: false
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/development",
    "purpose/code-manipulation",
    "purpose/version-control",
    "purpose/code-execution",
    "tech/multi-language",
  ]
---

# CodeSavant MCP Server

#status/active #category/development #purpose/code-manipulation #purpose/version-control #purpose/code-execution #tech/multi-language

## Description

Provides code manipulation, execution, and version control capabilities. It allows AI assistants to read, write, and execute code while maintaining a history of changes.

## Features

- Code manipulation
- Code execution
- Version control
- Change tracking
- History management
- Language support
- Execution sandbox
- Diff generation
- Rollback support
- Security controls

## Installation

```bash
npm install @twolven/mcp-codesavant
```

## Usage

```javascript
{
  "mcpServers": {
    "codesavant": {
      "command": "npx",
      "args": ["@twolven/mcp-codesavant"],
      "env": {
        "WORKSPACE_PATH": "./workspace",
        "VCS_TYPE": "git",
        "SANDBOX_ENABLED": "true",
        "MAX_FILE_SIZE": "1mb",
        "SUPPORTED_LANGUAGES": "python,javascript,java"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Git
- Language runtimes
- Sandbox environment
- Diff tools
- Version control system

## Related Servers

- automata-labs-team-code-sandbox-mcp
- seanivore/mcp-code-analyzer
- modelcontextprotocol-git-server
