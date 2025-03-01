--- 
type: server
repo_url: https://github.com/modelcontextprotocol/servers
name: Git
owner: modelcontextprotocol
stars: 11500
last_updated: 2025-02-28
status: active
official: true
verified: true
sources: ["inbox"]
tags:
  [
    "category/version-control",
    "status/official",
    "purpose/development",
    "tech/typescript",
  ]
---

#category/version-control #status/official #purpose/development #tech/typescript

# Git

## Description

A reference MCP server that provides tools to read, search, and manipulate Git repositories. This server demonstrates integration with Git operations and version control systems.

## Features

- Repository cloning and initialization
- Branch management and switching
- Commit history exploration
- File content retrieval from specific commits
- Git operations (pull, push, fetch)
- Repository status checking

## Installation

```bash
npm install @modelcontextprotocol/git-server
```

## Usage

```javascript
import { Server } from "@modelcontextprotocol/sdk/server";
import { GitServer } from "@modelcontextprotocol/git-server";

const server = new GitServer();
server.run();
```

## Dependencies

- @modelcontextprotocol/sdk
- nodegit or simple-git
- TypeScript

## Related Servers

- GitHub Server - For GitHub-specific operations
- GitLab Server - For GitLab-specific operations
- Filesystem Server - For local file operations