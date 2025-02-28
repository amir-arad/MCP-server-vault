---
type: server
repo_url: https://github.com/nguyenvanduocit/all-in-one-model-context-protocol
name: All In One Model Context Protocol
owner: nguyenvanduocit
stars: 34
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_001.md"]
tags: ["status/active", "category/integration", "integration/qdrant", "integration/google", "integration/jira", "integration/gitlab", "tech/go", "integration/confluence", "integration/youtube"]
---

# All In One Model Context Protocol

#status/active #category/integration #integration/qdrant #integration/google #integration/jira #integration/gitlab #tech/go #integration/confluence #integration/youtube

## Description

A powerful Model Context Protocol (MCP) server implementation with integrations for GitLab, Jira, Confluence, YouTube, and more. This server provides AI-powered search capabilities and various utility tools for development workflows. Note: The project has been split into individual repositories for specific functionality domains.

## Features

- Qdrant vector database integration for AI-powered search
- Google Suite integration (Gmail, Calendar, Chat)
- Jira project management tools
- GitLab version control integration
- Confluence documentation tools
- YouTube integration
- RAG (Retrieval Augmented Generation) capabilities
- Fetch and web scraping tools
- Research and academic tools
- Multi-service support with unified API interface
- Extensible architecture

## Installation

```bash
# Install via Smithery (recommended)
npx -y @smithery/cli install @nguyenvanduocit/all-in-one-model-context-protocol --client claude

# Or install via Go
go install github.com/nguyenvanduocit/all-in-one-model-context-protocol@latest
```

## Usage

```javascript
{
  "mcpServers": {
    "my_mcp_server": {
      "command": "all-in-one-model-context-protocol",
      "args": ["-env", "/path/to/.env"],
      "env": {
        "ENABLE_TOOLS": "",  // Leave empty to enable all tools
        "QDRANT_HOST": "your-qdrant-host",
        "ATLASSIAN_HOST": "your-atlassian-host",
        "ATLASSIAN_TOKEN": "your-atlassian-token",
        "GITLAB_HOST": "your-gitlab-host",
        "GITLAB_TOKEN": "your-gitlab-token",
        "GOOGLE_CREDENTIALS_FILE": "path/to/credentials.json",
        "GOOGLE_TOKEN_FILE": "path/to/token.json"
      }
    }
  }
}
```

## Dependencies

- Go 1.23.2 or higher
- Various API keys and tokens for integrated services:
  - Qdrant for vector database
  - Google API credentials
  - Atlassian (Jira/Confluence) tokens
  - GitLab access tokens
  - Optional: Brave API, OpenAI API, DeepSeek API

## Related Servers

- [Google Kit](https://github.com/nguyenvanduocit/google-kit) - Tools for Gmail, Google Calendar, Google Chat
- [RAG Kit](https://github.com/nguyenvanduocit/rag-kit) - Tools for RAG, Memory
- [Dev Kit](https://github.com/nguyenvanduocit/dev-kit) - Tools for developers, Jira, Confluence, GitLab, GitHub
- [Fetch Kit](https://github.com/nguyenvanduocit/fetch-kit) - Tools for fetch, scrape
- [Research Kit](https://github.com/nguyenvanduocit/research-kit) - Tools for research, academic, reasoning