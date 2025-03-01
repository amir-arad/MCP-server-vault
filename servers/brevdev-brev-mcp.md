--- 
type: server
repo_url: https://github.com/brevdev/brev-mcp
name: Brev MCP Server
owner: brevdev
stars: 3
last_updated: 2025-03-01
status: active
official: false
verified: true
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/machine-learning",
    "purpose/model-deployment",
    "purpose/cloud-computing",
  ]
---

# Brev MCP Server

#status/active #category/machine-learning #purpose/model-deployment #purpose/cloud-computing

## Description

Run, build, train, and deploy ML models on the cloud.

## Features

- ML model deployment
- Cloud training
- Model building
- Deployment management
- Resource optimization
- Performance monitoring
- Scaling automation
- Version control

## Installation

```bash
npm install @brevdev/brev-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "brev": {
      "command": "npx",
      "args": ["@brevdev/brev-mcp"],
      "env": {
        "BREV_API_KEY": "your-api-key",
        "CLOUD_PROVIDER": "aws",
        "INSTANCE_TYPE": "ml.t3.medium",
        "AUTO_SCALING": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Cloud provider account
- ML frameworks
- API credentials

## Related Servers

- None currently listed