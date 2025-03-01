---
type: server
repo_url: https://github.com/lamemind/coder-toolbox-mcp-server
name: Coder Toolbox MCP Server
owner: lamemind
stars: 2
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/development",
    "tech/java",
    "tech/javascript",
    "purpose/code-analysis",
    "purpose/testing",
    "purpose/automation",
  ]
---

# Coder Toolbox MCP Server

#status/active #category/development #tech/java #purpose/code-analysis #purpose/testing #purpose/automation

## Description

Integrates Java code analysis, manipulation, and testing tools for efficient software development workflows and automated code operations.

## Features

- Java code analysis
- Code manipulation
- Testing automation
- Workflow integration
- Static analysis
- Test generation
- Code formatting
- Quality checks
- Refactoring tools
- Performance profiling

## Installation

```bash
npm install @lamemind/coder-toolbox-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "coder-toolbox": {
      "command": "npx",
      "args": ["@lamemind/coder-toolbox-mcp"],
      "env": {
        "JAVA_HOME": "/path/to/java",
        "PROJECT_ROOT": "./",
        "TEST_PATH": "./src/test",
        "CHECKSTYLE_CONFIG": "./checkstyle.xml",
        "SPOTBUGS_ENABLED": "true"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Java JDK >= 11
- Maven/Gradle
- Testing frameworks
- Static analyzers
- Code formatters

## Related Servers

- seanivore/mcp-code-analyzer
- saiprashanths/code-analysis-mcp
- davidvc/code-mcp
