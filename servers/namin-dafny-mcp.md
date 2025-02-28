---
type: server
repo_url: https://github.com/namin/dafny-mcp
name: Dafny Verification MCP Server
owner: namin
stars: 2
last_updated: 2025-01-19
status: active
official: false
verified: false
sources: ["inbox/batch_008.md"]
tags:
  [
    "status/active",
    "category/verification",
    "integration/dafny",
    "purpose/formal-verification",
    "purpose/code-analysis",
    "tech/proofs",
  ]
---

# Dafny Verification MCP Server

#status/active #category/verification #integration/dafny #purpose/formal-verification #purpose/code-analysis #tech/proofs

## Description

Integrates with Dafny to verify code correctness through analysis of formal specifications and proofs. This server enables automated verification of program correctness using formal methods.

## Features

- Code verification
- Formal specifications
- Proof checking
- Error detection
- Specification analysis
- Verification reporting
- Proof generation
- Code analysis
- Result explanation
- Documentation support

## Installation

```bash
npm install @namin/dafny-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "dafny": {
      "command": "npx",
      "args": ["@namin/dafny-mcp"],
      "env": {
        "DAFNY_PATH": "/usr/local/bin/dafny",
        "TIMEOUT": "60",
        "VERIFICATION_LEVEL": "full",
        "PROOF_OUTPUT": "./proofs",
        "DEBUG_MODE": "false"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Dafny compiler
- Z3 theorem prover
- Proof checker
- Verification engine
- Report generator

## Related Servers

- modelcontextprotocol-verification-server
- kivo360-anthropic-mcp-code-analyzer
- skydeckai-mcp-server-aidd
