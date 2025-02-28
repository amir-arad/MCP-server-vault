---
type: server
repo_url: https://github.com/DMontgomery40/mcp-canvas-lms
name: Canvas LMS MCP Server
owner: DMontgomery40
stars: 0
last_updated: 2024-12-14
status: active
official: false
verified: false
sources: ["inbox/batch_005.md"]
tags:
  [
    "status/active",
    "category/education",
    "integration/canvas",
    "purpose/course-management",
    "tech/typescript",
  ]
---

# Canvas LMS MCP Server

#status/active #category/education #integration/canvas #purpose/course-management #tech/typescript

## Description

Manage courses and assignments in Canvas learning system. This MCP server provides integration with the Canvas Learning Management System, enabling automated course management and assignment handling.

## Features

- Course management
- Assignment creation and tracking
- Grade management
- Student enrollment handling
- Course content organization
- Calendar integration
- File management
- Announcement distribution
- Discussion board management
- Quiz administration

## Installation

```bash
npm install @dmontgomery40/mcp-canvas-lms
```

## Usage

```javascript
{
  "mcpServers": {
    "canvas": {
      "command": "npx",
      "args": ["@dmontgomery40/mcp-canvas-lms"],
      "env": {
        "CANVAS_API_URL": "https://your-institution.instructure.com/api/v1",
        "CANVAS_API_TOKEN": "your-canvas-api-token"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Canvas LMS instance
- Canvas API token
- TypeScript runtime

## Related Servers

- None currently listed
