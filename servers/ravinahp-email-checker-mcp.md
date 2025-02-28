---
type: server
repo_url: https://github.com/ravinahp/email-checker-mcp
name: Email Checker MCP Server
owner: ravinahp
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_010.md"]
tags:
  [
    "status/active",
    "category/utility",
    "purpose/email-validation",
    "tech/fastmcp",
    "purpose/verification",
    "tech/api",
  ]
---

# Email Checker MCP Server

#status/active #category/utility #purpose/email-validation #tech/fastmcp #purpose/verification #tech/api

## Description

Enables users to validate the existence of email addresses through a simple FastMCP tool, offering JSON responses without requiring an API key.

## Features

- Email address validation
- MX record checking
- Syntax verification
- Domain validation
- Response formatting
- Batch processing
- Fast validation
- No API key requirement
- JSON response format
- Error handling

## Installation

```bash
pip install email-checker-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "email-checker": {
      "command": "python",
      "args": ["-m", "email_checker_mcp"],
      "env": {
        "TIMEOUT": "5",
        "MAX_RETRIES": "3",
        "CACHE_DURATION": "3600"
      }
    }
  }
}
```

## Dependencies

- Python >= 3.7
- FastMCP framework
- DNS libraries
- Email validation tools
- Network connectivity

## Related Servers

- None currently listed
