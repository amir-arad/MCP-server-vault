---
type: server
repo_url: https://github.com/nguyenvanduocit/all-in-one-model-context-protocol
name: All In One Model Context Protocol
owner: nguyenvanduocit
stars: 29
last_updated: 2025-02-19
status: active
official: false
verified: false
sources: ["inbox/batch_001.md"]
tags: ["status/active", "category/integration", "integration/qdrant", "integration/google", "integration/jira", "integration/gitlab"]
---

# All In One Model Context Protocol

#status/active #category/integration #integration/qdrant #integration/google #integration/jira #integration/gitlab

## Description

All In One Model Context Protocol: qdrant, google suite (gmail, calendar, ...), jira, gitlab, CLI, and more integrations in a single server.

## Features

- Qdrant vector database integration
- Google Suite integration (Gmail, Calendar)
- Jira project management
- GitLab version control
- CLI capabilities
- Multi-service support
- Unified API interface
- Extensible architecture

## Installation

```bash
npm install @nguyenvanduocit/all-in-one-mcp
```

## Usage

```javascript
{
  "mcpServers": {
    "all-in-one": {
      "command": "npx",
      "args": ["@nguyenvanduocit/all-in-one-mcp"],
      "env": {
        "QDRANT_URL": "your-qdrant-url",
        "GOOGLE_CREDENTIALS": "path/to/credentials.json",
        "JIRA_TOKEN": "your-jira-token",
        "GITLAB_TOKEN": "your-gitlab-token"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 16
- Various service credentials
- API access tokens
- Service accounts

## Related Servers

- None currently listed