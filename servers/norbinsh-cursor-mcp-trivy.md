---
type: server
repo_url: https://github.com/norbinsh/cursor-mcp-trivy
name: Cursor Trivy MCP Server
owner: norbinsh
stars: 2
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_008.md"]
tags:
  [
    "status/active",
    "category/security",
    "integration/trivy",
    "purpose/vulnerability-scanning",
    "purpose/remediation",
    "category/devops",
    "tech/python",
    "tech/automation",
    "integration/cursor",
    "purpose/security"
  ]
---

# Cursor Trivy MCP Server

#status/active #category/security #integration/trivy #purpose/vulnerability-scanning #purpose/remediation #category/devops #tech/python #tech/automation #integration/cursor #purpose/security

## Description

A Python-based MCP server that provides automated security scanning capabilities through integration with Trivy. The server enables automated vulnerability scanning and remediation for projects across multiple programming languages and package managers, offering comprehensive security analysis through a standardized interface.

## Features

- Automated vulnerability scanning
- Multi-package manager support
- Automated dependency updates
- Security report generation
- Risk assessment tools
- Fix recommendations
- Scheduled scanning
- Result tracking system
- Policy enforcement
- Python/Node.js/Ruby/Go support
- Real-time scanning
- Dependency analysis
- Version management
- Security compliance
- Integration capabilities

## Installation

```bash
# Create and activate virtual environment
python -m venv .venv
source .venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Install Trivy (macOS)
brew install trivy

# Start server
python server.py --transport sse --port 54321
```

## Usage

```javascript
// Configuration
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

// Cursor IDE Integration
http://127.0.0.1:54321/sse

// Available Tools
scan_project:
  - workspace: Directory path to scan

fix_vulnerability:
  - workspace: Directory to modify
  - pkg_name: Package to update
  - target_version: Version to update to
```

## Dependencies

- Python >= 3.12
- Trivy scanner
- Package managers
- Security database
- Report generator
- Fix applier
- SSE transport
- Cursor IDE
- MCP SDK
- Automation tools

## Related Servers

- nahmanmate-better-auth-mcp-server
- buga-luga/cursor-mcp
- modelcontextprotocol-security-server
- aquasecurity/trivy-server