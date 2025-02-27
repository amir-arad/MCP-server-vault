---
type: server
repo_url: https://github.com/fireproof-storage/mcp-database-server
name: Fireproof
owner: fireproof-storage
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
tags: ["status/active", "status/official", "category/database"]
---

#status/active #status/official #category/database

# Fireproof

## Description

Immutable ledger database with live synchronization. This MCP server provides a robust database solution with built-in immutability and real-time synchronization capabilities, powered by [Fireproof](https://fireproof.storage).

## Features

- Immutable ledger-based storage
- Real-time data synchronization
- Cryptographic verification
- Audit trail capabilities
- Conflict-free replication
- Offline-first architecture
- Secure data storage
- Multi-device synchronization

## Installation

```bash
npm install @fireproof/mcp-server
```

## Usage

```javascript
import { FireproofServer } from "@fireproof/mcp-server";

const server = new FireproofServer({
  apiKey: "your-fireproof-api-key",
  databaseName: "my-ledger-db",
});

// Create a new record
const record = await server.create({
  collection: "transactions",
  data: {
    amount: 100,
    description: "Payment for services",
    timestamp: new Date().toISOString(),
  },
});

// Subscribe to changes
server.subscribe("transactions", (changes) => {
  console.log("New changes:", changes);
});
```

## Dependencies

- Node.js >= 14.x
- Fireproof API key
- Active Fireproof account

## Related Servers

- None currently listed
