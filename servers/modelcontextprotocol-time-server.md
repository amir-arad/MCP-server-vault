--- 
type: server
repo_url: https://github.com/modelcontextprotocol/servers
name: Time
owner: modelcontextprotocol
stars: 11500
last_updated: 2025-02-28
status: active
official: true
verified: true
sources: ["inbox"]
tags:
  [
    "category/utility",
    "status/official",
    "purpose/development",
    "tech/typescript",
  ]
---

# Time

#category/utility #status/official #purpose/development #tech/typescript

## Description

A reference MCP server that provides time and timezone conversion capabilities. This server demonstrates handling of time-related operations and conversions.

## Features

- Timezone conversion
- Date and time formatting
- Duration calculations
- Calendar operations
- Time parsing
- UTC conversion
- DST handling

## Installation

```bash
npm install @modelcontextprotocol/time-server
```

## Usage

```javascript
import { Server } from "@modelcontextprotocol/sdk/server";
import { TimeServer } from "@modelcontextprotocol/time-server";

const server = new TimeServer({
  defaultTimezone: "UTC",
});
server.run();
```

## Dependencies

- @modelcontextprotocol/sdk
- moment-timezone
- TypeScript

## Related Servers

- Memory Server - For caching timezone data
- PostgreSQL Server - For storing time series data