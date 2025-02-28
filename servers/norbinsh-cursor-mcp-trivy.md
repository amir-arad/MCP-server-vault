---
type: server
repo_url: https://github.com/norbinsh/cursor-mcp-trivy
name: Cursor Trivy MCP Server
owner: norbinsh
stars: 2
last_updated: 2025-02-18
status: active
official: false
verified: false
sources: ["inbox/batch_008.md"]
tags:
  [
    "status/active",
    "category/security",
    "integration/trivy",
    "purpose/vulnerability-scanning",
    "purpose/remediation",
    "category/devops",
  ]
---

# Cursor Trivy MCP Server

#status/active #category/security #integration/trivy #purpose/vulnerability-scanning #purpose/remediation #category/devops

## Description

Integrates with Trivy to provide vulnerability scanning and automated remediation for projects across multiple programming languages and package managers.

## Features

- Vulnerability scanning
- Automated remediation
- Multi-language support
- Package management
- Security reporting
- Risk assessment
- Fix suggestions
- Scan scheduling
- Result tracking
- Policy enforcement

## Installation

```bash
npm install @norbinsh/cursor-mcp-trivy
```

## Usage

```javascript
{
  "mcpServers": {
    "cursor-trivy": {
      "command": "npx",
      "args": ["@norbinsh/cursor-mcp-trivy"],
      "env": {
        "TRIVY_PATH": "/usr/local/bin/trivy",
        "SCAN_INTERVAL": "86400",
        "SEVERITY_THRESHOLD": "HIGH",
        "AUTO_REMEDIATE": "false",
        "REPORT_PATH": "./security-reports"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Trivy scanner
- Package managers
- Security database
- Report generator
- Fix applier

## Related Servers

- nahmanmate-better-auth-mcp-server
- buga-luga/cursor-mcp
- modelcontextprotocol-security-server
