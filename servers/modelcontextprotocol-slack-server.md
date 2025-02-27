---
type: server
repo_url: https://github.com/modelcontextprotocol/servers/src/slack
name: Slack
owner: modelcontextprotocol
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
tags:
  [
    "category/communication",
    "status/official",
    "purpose/development",
    "tech/typescript",
    "integration/slack",
  ]
---

#category/communication #status/official #purpose/development #tech/typescript #integration/slack

# Slack

## Description

A reference MCP server that provides channel management and messaging capabilities through Slack's platform. This server enables comprehensive interaction with Slack workspaces and channels.

## Features

- Channel management
- Message sending and retrieval
- User and group management
- File sharing capabilities
- Reaction and thread handling
- Webhook integration
- Real-time event subscription

## Installation

```bash
npm install @modelcontextprotocol/slack-server
```

## Usage

```javascript
import { Server } from "@modelcontextprotocol/sdk/server";
import { SlackServer } from "@modelcontextprotocol/slack-server";

const server = new SlackServer({
  token: process.env.SLACK_BOT_TOKEN,
  signingSecret: process.env.SLACK_SIGNING_SECRET,
});
server.run();
```

## Dependencies

- @modelcontextprotocol/sdk
- @slack/web-api
- @slack/events-api
- TypeScript

## Related Servers

- Memory Server - For caching message data
- PostgreSQL Server - For storing conversation history
