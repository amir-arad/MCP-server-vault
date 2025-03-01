---
type: server
repo_url: https://github.com/cpage-pivotal/app-advisor-mcp
name: App Advisor MCP Server
owner: cpage-pivotal
stars: 2
last_updated: 2025-03-01
status: active
official: false
verified: true
sources: ["inbox/batch_002.md"]
tags:
  [
    "status/active",
    "category/development",
    "integration/spring",
    "integration/cloud-foundry",
    "purpose/optimization",
  ]
---

# App Advisor MCP Server

#status/active #category/development #integration/spring #integration/cloud-foundry #purpose/optimization

## Description

Integrates with Spring Application Advisor to provide insights and recommendations for optimizing Spring applications in Cloud Foundry environments.

## Features

- Spring application analysis
- Performance optimization
- Cloud Foundry integration
- Application insights
- Recommendation engine
- Resource monitoring
- Configuration analysis
- Best practices validation

## Installation

```bash
npm install @cpage-pivotal/app-advisor-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "app-advisor": {
      "command": "npx",
      "args": ["@cpage-pivotal/app-advisor-mcp"],
      "env": {
        "CF_API_URL": "https://api.cf.example.com",
        "CF_USERNAME": "your-username",
        "CF_PASSWORD": "your-password",
        "SPRING_PROFILE": "cloud"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Cloud Foundry environment
- Spring Framework
- Application Advisor access

## Related Servers

- None currently listed
