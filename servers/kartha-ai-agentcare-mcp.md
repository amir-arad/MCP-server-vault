---
type: server
repo_url: https://github.com/Kartha-AI/agentcare-mcp
name: AgentCare MCP Server
owner: Kartha-AI
stars: 2
last_updated: 2025-02-19
status: active
official: false
verified: false
sources: ["inbox/batch_001.md"]
tags: ["status/active", "category/healthcare", "integration/fhir", "integration/cerner", "integration/epic", "purpose/healthcare"]
---

# AgentCare MCP Server

#status/active #category/healthcare #integration/fhir #integration/cerner #integration/epic #purpose/healthcare

## Description

An MCP server that provides healthcare tools for interacting with FHIR data and medical resources on EMRs like Cerner and Epic.

## Features

- FHIR data integration
- Cerner EMR support
- Epic EMR support
- Medical resource access
- Healthcare data processing
- Secure data handling
- EMR system compatibility

## Installation

```bash
npm install @kartha-ai/agentcare-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "agentcare": {
      "command": "npx",
      "args": ["@kartha-ai/agentcare-mcp"],
      "env": {
        "FHIR_BASE_URL": "https://your-fhir-server/fhir",
        "EMR_TYPE": "epic",  // or "cerner"
        "EMR_API_KEY": "your-api-key",
        "SECURE_MODE": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- FHIR server access
- EMR system credentials (Epic or Cerner)
- HIPAA compliance setup

## Related Servers

- None currently listed