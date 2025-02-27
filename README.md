# MCP Server Vault

A comprehensive, searchable database of Model Context Protocol (MCP) servers.

## Design Philosophy

This vault is designed to maintain a complete and useful database of MCP servers for quick searching and browsing. Each MCP server is documented in a single note with extensive tagging, creating an authoritative source for for the MCP ecosystem.

## Key Design Decisions

### 1. Single Note Per Server

- Filename convention: `[Repository Owner]-[Repository Name].md`
- Canonical repository URL as unique identifier to avoid duplicates

### 2. Rich Metadata in Frontmatter

```yaml
---
repo_url: https://github.com/owner/repo-name
owner: repository_owner
name: repository_name
stars: 42
last_updated: 2025-02-21
status: active|inactive|deprecated
official: true|false
verified: true|false
sources:
  - awesome-mcp-servers-wong2
  - mcpservers-org
---
```

### 3. Multi-dimensional Tagging System

- Core tags: `#mcp/server`, `#status/active`
- Category tags: `#category/database`, `#category/search`
- Tech stack tags: `#tech/typescript`, `#tech/python`
- Purpose tags: `#purpose/rag`, `#purpose/memory`
- Integration tags: `#integration/slack`, `#integration/github`
- Feature tags: `#feature/authentication`, `#feature/vector-search`
- Source tags: `#source/mcpservers-org`, `#source/awesome-mcp-servers-wong2`

### 4. Tag Record Notes

Each tag has its own record note:

```yaml
---
type: tag
id: source/awesome-mcp-servers-wong2
name: Wong2's Awesome MCP Servers
url: https://github.com/wong2/awesome-mcp-servers
last_checked: 2025-02-27
servers_count: 142
---
```

Benefits:

- Self-documenting taxonomy
- Tag metadata tracking
- Hierarchical organization
- Detailed source attribution
- Improved discoverability

### 5. Automation Workflow

1. **Source Scanning**: Fetch data from known sources and append raw data to inbox
2. **Duplicate Processing**: Extract GitHub URLs, compare against existing notes, update sources
3. **Source Discovery**: Extract links to new aggregator sites for expanding sources
4. **Source & Feature Tagging**: Maintain comprehensive tagging

## Server Note Template

- Description (from repository)
- Features
- Installation instructions
- Usage examples
- Dependencies
- Related servers (similar functionality)

This design enables powerful querying, cross-referencing, and discovery of MCP servers while maintaining a structured, organized knowledge base that can grow with the ecosystem.
