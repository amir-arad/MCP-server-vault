---
type: server
repo_url: https://github.com/baryhuang/mcp-server-aws-resources-python
name: AWS Resources Python MCP Server
owner: baryhuang
stars: 2
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_003.md"]
tags: ["status/active", "category/cloud", "integration/aws", "tech/python", "purpose/devops", "tech/docker", "integration/boto3"]
---

# AWS Resources Python MCP Server

#status/active #category/cloud #integration/aws #tech/python #purpose/devops #tech/docker #integration/boto3

## Description

A Model Context Protocol (MCP) server implementation that provides the ability to run generated Python code to query any AWS resources through boto3. This server enables DevOps tasks and cloud resource management with full access to AWS services based on the provided credentials.

## Features

- Execute Python code using boto3 to query AWS resources
- Support for multiple AWS services (S3, CodePipeline, EC2, etc.)
- Docker-based deployment for cross-platform compatibility
- Secure credential handling through environment variables or AWS profiles
- Sandboxed code execution environment
- Support for complex queries with multiple AWS services
- Available through Docker Hub for easy installation
- Cross-platform support (Linux/amd64, Linux/arm64, Linux/arm/v7)

## Installation

```bash
# Install via Smithery (recommended)
npx -y @smithery/cli install mcp-server-aws-resources-python --client claude

# Or pull Docker image
docker pull buryhuang/mcp-server-aws-resources:latest
```

## Usage

```javascript
{
  "mcpServers": {
    "aws-resources": {
      "command": "docker",
      "args": [
        "run",
        "-i",
        "--rm",
        "-e",
        "AWS_ACCESS_KEY_ID=your_access_key_id_here",
        "-e",
        "AWS_SECRET_ACCESS_KEY=your_secret_access_key_here",
        "-e",
        "AWS_DEFAULT_REGION=us-east-1",
        "buryhuang/mcp-server-aws-resources:latest"
      ]
    }
  }
}
```

## Dependencies

- Docker (for container-based deployment)
- AWS credentials with appropriate permissions
- Python >= 3.8 (if running from source)
- boto3 (AWS SDK for Python)

## Related Servers

- modelcontextprotocol/aws-kb-retrieval-server - AWS knowledge base retrieval
- RafalWilinski/aws-mcp - Node.js-based AWS integration
- rishikavikondala/mcp-server-aws - Alternative AWS integration
- baryhuang/mcp-server-any-openapi - OpenAPI integration server by the same author