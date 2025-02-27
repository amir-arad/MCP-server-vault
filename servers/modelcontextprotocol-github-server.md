---
type: server
repo_url: https://github.com/modelcontextprotocol/servers/src/github
name: GitHub
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
    "integration/github",
  ]
---

#category/version-control #status/official #purpose/development #tech/typescript #integration/github

# GitHub

## Description

A reference MCP server that provides repository management, file operations, and GitHub API integration. This server enables comprehensive interaction with GitHub repositories and services.

## Features

- Repository management (create, delete, fork)
- Issue and pull request handling
- File content operations
- Repository search and metadata retrieval
- Workflow and action management
- GitHub API integration
- Team and organization management

## Installation

```bash
npm install @modelcontextprotocol/github-server
```

## Usage

```javascript
import { Server } from "@modelcontextprotocol/sdk/server";
import { GitHubServer } from "@modelcontextprotocol/github-server";

const server = new GitHubServer({
  auth: process.env.GITHUB_TOKEN,
});
server.run();
```

## Dependencies

- @modelcontextprotocol/sdk
- @octokit/rest
- TypeScript

## Related Servers

- Git Server - For local Git operations
- GitLab Server - For GitLab-specific operations
- Filesystem Server - For local file operations
