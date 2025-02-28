---
type: server
repo_url: https://github.com/whataboutyou-ai/eunomia-MCP-server
name: Eunomia MCP Server
owner: whataboutyou-ai
stars: 5
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_011.md"]
tags:
  [
    "status/active",
    "category/governance",
    "purpose/data-governance",
    "purpose/access-control",
    "purpose/pii-detection",
    "tech/framework",
  ]
---

# Eunomia MCP Server

#status/active #category/governance #purpose/data-governance #purpose/access-control #purpose/pii-detection #tech/framework

## Description

Extension of the Eunomia framework that connects Eunomia instruments with MCP servers, providing a simple way to orchestrate data governance policies (like PII detection or user access control) and seamlessly integrate them with external services.

## Features

- Data governance integration
- PII detection
- User access control
- Policy orchestration
- External service integration
- Policy enforcement
- Compliance monitoring
- Audit logging
- Data classification
- Security controls

## Installation

```bash
npm install @whataboutyou-ai/eunomia-mcp-server
```

## Usage

```javascript
{
  "mcpServers": {
    "eunomia": {
      "command": "npx",
      "args": ["@whataboutyou-ai/eunomia-mcp-server"],
      "env": {
        "POLICY_DIR": "./policies",
        "LOG_LEVEL": "info",
        "PII_DETECTION_MODE": "strict",
        "AUDIT_ENABLED": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Eunomia framework
- Policy engine
- Storage system
- Audit logging system

## Related Servers

- None currently listed
