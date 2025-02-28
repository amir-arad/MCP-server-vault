---
type: server
repo_url: https://github.com/seanivore/mcp-code-analyzer
name: Python Code Analyzer MCP Server
owner: seanivore
stars: 10
last_updated: 2025-02-17
status: active
official: false
verified: false
sources: ["inbox/batch_006.md"]
tags:
  [
    "status/active",
    "category/development",
    "tech/python",
    "purpose/code-analysis",
    "purpose/quality-assurance",
    "purpose/code-review",
  ]
---

# Python Code Analyzer MCP Server

#status/active #category/development #tech/python #purpose/code-analysis #purpose/quality-assurance #purpose/code-review

## Description

Analyzes Python code structure, complexity, and dependencies using parsing tools to provide insights for automated quality checks and code reviews.

## Features

- Code structure analysis
- Complexity metrics
- Dependency tracking
- Quality assessment
- AST parsing
- Pattern detection
- Style checking
- Cyclomatic complexity
- Import analysis
- Report generation

## Installation

```bash
npm install @seanivore/mcp-code-analyzer
```

## Usage

```javascript
{
  "mcpServers": {
    "code-analyzer": {
      "command": "npx",
      "args": ["@seanivore/mcp-code-analyzer"],
      "env": {
        "PYTHON_PATH": "python3",
        "PROJECT_ROOT": "./",
        "IGNORE_PATTERNS": "__pycache__,*.pyc",
        "MAX_COMPLEXITY": "10",
        "REPORT_FORMAT": "json"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Python >= 3.8
- AST parser
- Complexity analyzer
- Style checker
- Report generator

## Related Servers

- saiprashanths/code-analysis-mcp
- davidvc/code-knowledge-mcptool
- kivo360-anthropic-mcp-code-analyzer
