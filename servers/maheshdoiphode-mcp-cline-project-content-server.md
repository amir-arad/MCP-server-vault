---
type: server
repo_url: https://github.com/MaheshDoiphode/mcp-cline-project-content-server
name: Cline Project Content MCP Server
owner: MaheshDoiphode
stars: 3
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/development",
    "tech/cline",
    "purpose/file-access",
    "purpose/content-management",
    "tech/filesystem",
  ]
---

# Cline Project Content MCP Server

#status/active #category/development #tech/cline #purpose/file-access #purpose/content-management #tech/filesystem

## Description

An MCP server that provides access to project files and their contents, allowing users to retrieve file data from specified project directories with error handling and configuration options.

## Features

- File content access
- Directory navigation
- Error handling
- Content retrieval
- Path resolution
- File type detection
- Access control
- Content caching
- Search capabilities
- Change monitoring

### API

#### latest_project_data

Get all files and their contents from a project directory.

**Parameters:**

- `projectPath` (string): Path to the project directory

**Example Request:**

```json
{
  "name": "latest_project_data",
  "arguments": {
    "projectPath": "/path/to/project"
  }
}
```

**Example Response:**

```json
{
  "file1.txt": "Contents of file1",
  "subdir/file2.js": "Contents of file2"
}
```

## Installation

1.  Clone the repository
2.  Install dependencies:

```bash
npm install
```

3.  Build the project:

```bash
npm run build
```

## Usage

Start the server:

```bash
node build/index.js
```

## Configuration

The server can be configured using environment variables:

- `PORT`: Port to run the server on (default: stdio)

## Error Handling

The server returns errors in the following format:

```json
{
  "content": [
    {
      "type": "text",
      "text": "Error message"
    }
  ],
  "isError": true
}
```

Common errors include:

- Invalid project path
- Permission denied errors
- File system errors

## Dependencies

- Node.js >= 16
- File system access
- Content parser
- Cache system
- File watcher
- Path resolver
