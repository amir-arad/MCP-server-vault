---
type: server
repo_url: https://github.com/modelcontextprotocol/servers/src/gitlab
name: GitLab
owner: modelcontextprotocol
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
tags:
  [
    "category/version-control",
    "status/official",
    "purpose/development",
    "tech/typescript",
    "integration/gitlab",
  ]
---

#category/version-control #status/official #purpose/development #tech/typescript #integration/gitlab

# GitLab

## Description

A reference MCP server that enables GitLab API integration, providing comprehensive project management capabilities and repository operations through the GitLab platform.

## Features

- Project management and configuration
- Repository operations (clone, fork, merge)
- Issue and merge request handling
- CI/CD pipeline management
- User and group administration
- Repository metadata retrieval
- File content operations

## Installation

```bash
npm install @modelcontextprotocol/gitlab-server
```

## Usage

```javascript
import { Server } from "@modelcontextprotocol/sdk/server";
import { GitLabServer } from "@modelcontextprotocol/gitlab-server";

const server = new GitLabServer({
  token: process.env.GITLAB_TOKEN,
});
server.run();
```

## Dependencies

- @modelcontextprotocol/sdk
- @gitbeaker/rest
- TypeScript

## Related Servers

- Git Server - For local Git operations
- GitHub Server - For GitHub-specific operations
- Filesystem Server - For local file operations
