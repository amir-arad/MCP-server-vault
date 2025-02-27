---
type: server
repo_url: https://github.com/modelcontextprotocol/servers/src/gdrive
name: Google Drive
owner: modelcontextprotocol
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
tags:
  [
    "category/filesystem",
    "status/official",
    "purpose/development",
    "tech/typescript",
    "integration/google",
  ]
---

#category/filesystem #status/official #purpose/development #tech/typescript #integration/google

# Google Drive

## Description

A reference MCP server that provides file access and search capabilities for Google Drive. This server enables seamless integration with Google Drive's storage and file management features.

## Features

- File and folder operations
- Advanced search capabilities
- File metadata retrieval
- Permission management
- File content streaming
- Document conversion
- Shared drive support

## Installation

```bash
npm install @modelcontextprotocol/gdrive-server
```

## Usage

```javascript
import { Server } from "@modelcontextprotocol/sdk/server";
import { GoogleDriveServer } from "@modelcontextprotocol/gdrive-server";

const server = new GoogleDriveServer({
  credentials: process.env.GOOGLE_APPLICATION_CREDENTIALS,
});
server.run();
```

## Dependencies

- @modelcontextprotocol/sdk
- @google-cloud/storage
- googleapis
- TypeScript

## Related Servers

- Filesystem Server - For local file operations
- GitHub Server - For repository file management
- GitLab Server - For repository file management
