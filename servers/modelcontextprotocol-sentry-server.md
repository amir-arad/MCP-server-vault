--- 
type: server
repo_url: https://github.com/modelcontextprotocol/servers
name: Sentry
owner: modelcontextprotocol
stars: 11500
last_updated: 2025-02-28
status: active
official: true
verified: true
sources: ["inbox"]
tags:
  [
    "category/monitoring",
    "status/official",
    "purpose/development",
    "tech/typescript",
    "integration/sentry",
  ]
---

#category/monitoring #status/official #purpose/development #tech/typescript #integration/sentry

# Sentry

## Description

A reference MCP server that enables retrieving and analyzing issues from Sentry.io. This server provides integration with Sentry's error tracking and monitoring platform.

## Features

- Issue retrieval and analysis
- Error event tracking
- Performance monitoring
- Release tracking
- Project management
- Team collaboration
- Alert configuration

## Installation

```bash
npm install @modelcontextprotocol/sentry-server
```

## Usage

```javascript
import { Server } from "@modelcontextprotocol/sdk/server";
import { SentryServer } from "@modelcontextprotocol/sentry-server";

const server = new SentryServer({
  token: process.env.SENTRY_AUTH_TOKEN,
  organization: process.env.SENTRY_ORG,
});
server.run();
```

## Dependencies

- @modelcontextprotocol/sdk
- @sentry/node
- TypeScript

## Related Servers

- Memory Server - For caching issue data
- PostgreSQL Server - For storing error analytics