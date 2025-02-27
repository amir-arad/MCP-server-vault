---
type: server
repo_url: https://github.com/esignaturescom/mcp-server-esignatures
name: eSignatures
owner: esignaturescom
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
tags: ["status/active", "status/official", "category/utility"]
---

#status/active #status/official #category/utility

# eSignatures

## Description

Contract and template management MCP server for drafting, reviewing, and sending binding contracts. Integrates with [eSignatures](https://esignatures.com) platform for comprehensive digital contract management.

## Features

- Contract drafting and management
- Template-based document creation
- Document review workflow
- Digital signature integration
- Contract status tracking
- Template management
- Secure document handling

## Installation

```bash
npm install @esignatures/mcp-server
```

## Usage

```javascript
import { ESignaturesServer } from "@esignatures/mcp-server";

const server = new ESignaturesServer({
  apiKey: "your-esignatures-api-key",
});

// Create a new contract from template
const contract = await server.createContract({
  templateId: "template-123",
  signers: [{ email: "signer1@example.com", name: "John Doe" }],
  data: {
    clientName: "Acme Corp",
    startDate: "2025-03-01",
  },
});
```

## Dependencies

- Node.js >= 14.x
- eSignatures API key
- Active eSignatures account

## Related Servers

- None currently listed
