---
type: server
repo_url: https://github.com/morinokami/mcp-server-bluesky
name: Bluesky MCP Server
owner: morinokami
stars: 1
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/social-media",
    "integration/bluesky",
    "purpose/social-networking",
  ]
---

# Bluesky MCP Server

#status/active #category/social-media #integration/bluesky #purpose/social-networking

## Description

Integrates with Bluesky's social network API to enable profile management, posting, following, and engagement actions.

## Features

- Profile management
- Post creation
- Following management
- Engagement tracking
- Content discovery
- Feed management
- User interactions
- Content moderation

## Usage

To use with Claude Desktop:

```json
{
  "mcpServers": {
    "bluesky": {
      "command": "npx",
      "args": ["-y", "mcp-server-bluesky"],
      "env": {
        "BLUESKY_USERNAME": "username",
        "BLUESKY_PASSWORD": "password"
      }
    }
  }
}
```

## Tools

- `bluesky_get_profile`
- `bluesky_follow`
- `bluesky_delete_follow`
- `bluesky_get_follows`
- `bluesky_get_followers`
- `bluesky_search_posts`
- `bluesky_post`
- `bluesky_delete_post`
- `bluesky_repost`
- `bluesky_delete_repost`
- `bluesky_get_timeline`
- `bluesky_get_post_thread`
- `bluesky_get_likes`
- `bluesky_like`
- `bluesky_delete_like`

## Dependencies

- Node.js >= 14
- Bluesky account
- API access
- Network connectivity

## Related Servers

- keturiosakys/bluesky-context-server
- laulauland/bluesky-context-server
- berlinbra/BlueSky-MCP
