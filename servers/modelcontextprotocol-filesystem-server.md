---
type: server
repo_url: https://github.com/modelcontextprotocol/servers/src/filesystem
name: Filesystem
owner: modelcontextprotocol
stars: 9794
last_updated: 2025-02-28
status: active
official: true
verified: true
sources: ["inbox"]
tags: ["category/filesystem", "status/official", "purpose/development"]
---

# Filesystem

#category/filesystem #status/official #purpose/development

## Description

A reference MCP server that provides secure file operations with configurable access controls. This server demonstrates best practices for implementing filesystem operations in an MCP context.

## Features

- Secure file operations with configurable access controls
- Directory listing and file search capabilities
- File content reading and writing
- Path validation and security checks
- Configurable file access permissions

## Installation

```bash
npm install @modelcontextprotocol/filesystem-server
```

## Usage

```javascript
import { Server } from "@modelcontextprotocol/sdk/server";
import { FilesystemServer } from "@modelcontextprotocol/filesystem-server";

const server = new FilesystemServer();
server.run();
```

## Dependencies

- @modelcontextprotocol/sdk
- Node.js filesystem APIs
