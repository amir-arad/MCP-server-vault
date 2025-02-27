---
type: server
repo_url: https://github.com/JetBrains/mcp-jetbrains
name: JetBrains
owner: JetBrains
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
tags:
  [
    "status/active",
    "status/official",
    "category/development",
    "integration/jetbrains",
  ]
---

# JetBrains

#status/active #status/official #category/development #integration/jetbrains

## Description

Work on your code with JetBrains IDEs. This MCP server provides integration with JetBrains' suite of development tools, enabling AI agents to interact with and control JetBrains IDEs for enhanced development workflows.

## Features

- IDE control and automation
- Code navigation and manipulation
- Project management
- Code analysis and inspection
- Refactoring capabilities
- Version control integration
- Build and run configurations
- Debug session management
- Multiple IDE support (IntelliJ, PyCharm, WebStorm, etc.)

## Installation

```bash
npm install @jetbrains/mcp-server
```

## Usage

```javascript
import { JetBrainsServer } from "@jetbrains/mcp-server";

const server = new JetBrainsServer({
  apiKey: "your-jetbrains-api-key",
  ide: "intellij", // or 'pycharm', 'webstorm', etc.
});

// Open a project
await server.openProject({
  path: "/path/to/your/project",
});

// Navigate to a file and make changes
await server.editFile({
  file: "src/main/java/com/example/App.java",
  actions: [
    {
      type: "navigate",
      position: {
        line: 10,
        column: 15,
      },
    },
    {
      type: "refactor",
      action: "rename",
      from: "oldMethodName",
      to: "newMethodName",
    },
  ],
});

// Run code analysis
const issues = await server.analyze({
  scope: "project",
  severity: ["error", "warning"],
});
```

## Dependencies

- Node.js >= 14.x
- JetBrains IDE installation
- JetBrains API key
- JetBrains Gateway (for remote development)

## Related Servers

- None currently listed
