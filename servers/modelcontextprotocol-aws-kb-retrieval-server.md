---
type: server
repo_url: https://github.com/modelcontextprotocol/servers/tree/main/src/aws-kb-retrieval-server
name: AWS KB Retrieval Server
owner: modelcontextprotocol
stars: 9794
last_updated: 2025-02-28
status: active
official: true
verified: true
sources: ["inbox/batch_003.md"]
tags:
  [
    "status/active",
    "status/official",
    "category/knowledge-base",
    "integration/aws",
    "integration/bedrock",
  ]
---

# AWS KB Retrieval Server

#status/active #status/official #category/knowledge-base #integration/aws #integration/bedrock

## Description

An MCP server implementation for retrieving information from the AWS Knowledge Base using the Bedrock Agent Runtime.

## Features

- **RAG (Retrieval-Augmented Generation)**: Retrieve context from the AWS Knowledge Base based on a query and a Knowledge Base ID.
- **Supports multiple results retrieval**: Option to retrieve a customizable number of results.

## Tools

- **retrieve_from_aws_kb**
  - Perform retrieval operations using the AWS Knowledge Base.
  - Inputs:
    - `query` (string): The search query for retrieval.
    - `knowledgeBaseId` (string): The ID of the AWS Knowledge Base.
    - `n` (number, optional): Number of results to retrieve (default: 3).

## Configuration

### Setting up AWS Credentials

1.  Obtain AWS access key ID, secret access key, and region from the AWS Management Console.
2.  Ensure these credentials have appropriate permissions for Bedrock Agent Runtime operations.

### Usage with Claude Desktop

Add this to your `claude_desktop_config.json`:

#### Docker

```json
{
  "mcpServers": {
    "aws-kb-retrieval": {
      "command": "docker",
      "args": [
        "run",
        "-i",
        "--rm",
        "-e",
        "AWS_ACCESS_KEY_ID",
        "-e",
        "AWS_SECRET_ACCESS_KEY",
        "-e",
        "AWS_REGION",
        "mcp/aws-kb-retrieval-server"
      ],
      "env": {
        "AWS_ACCESS_KEY_ID": "YOUR_ACCESS_KEY_HERE",
        "AWS_SECRET_ACCESS_KEY": "YOUR_SECRET_ACCESS_KEY_HERE",
        "AWS_REGION": "YOUR_AWS_REGION_HERE"
      }
    }
  }
}
```

```json
{
  "mcpServers": {
    "aws-kb-retrieval": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-aws-kb-retrieval"],
      "env": {
        "AWS_ACCESS_KEY_ID": "YOUR_ACCESS_KEY_HERE",
        "AWS_SECRET_ACCESS_KEY": "YOUR_SECRET_ACCESS_KEY_HERE",
        "AWS_REGION": "YOUR_AWS_REGION_HERE"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- AWS account
- Bedrock access
- Knowledge base setup
