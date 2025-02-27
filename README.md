# MCP Server Vault

A comprehensive, searchable database of Model Context Protocol (MCP) servers.

## Design Philosophy

This vault is designed to maintain a complete and useful database of MCP servers for quick searching and browsing. Each MCP server is documented in a single note with extensive tagging, creating an authoritative source for the MCP ecosystem.

## For Human Users

### Setup Instructions

1. Install [Obsidian](https://obsidian.md/) if you haven't already
2. Clone this repository: `git clone https://github.com/amir-arad/MCP-server-vault.git`
3. Open the repository as a vault in Obsidian: "Open folder as vault" → select the cloned directory
4. Install these recommended community plugins:
   - [Obsidian Local REST API](https://github.com/coddingtonbear/obsidian-local-rest-api) - For AI integration
   - [Obsidian Git](https://github.com/denolehov/obsidian-git) - For version control
   - [Smart Connections](https://github.com/brianpetro/obsidian-smart-connections) - For semantic searching
   - [Templater](https://github.com/SilentVoid13/Templater) - For advanced templating
   - [MCP Tools](https://github.com/modelcontextprotocol/obsidian-mcp-tools) - For MCP-specific functionality

### Using the Vault

- Browse servers in the `servers/` directory
- Use tags to filter and discover servers by category, technology, or purpose
- Search using queries like:
  - `tag:#category/database` to find all database servers
  - `tag:#tech/typescript tag:#purpose/rag` to find TypeScript RAG servers
  - `stars:>100` to find popular servers with over 100 GitHub stars

### Contributing

1. Fork the repository from https://github.com/amir-arad/MCP-server-vault
2. Add new servers using the template in `templates/server.md`
3. Ensure proper frontmatter metadata and tagging
4. Submit a pull request

## For AI Agents

### Vault Structure

- `servers/` - Individual MCP server documentation files (filename format: `[owner]-[repo-name].md`)
- `templates/` - Templates for creating new notes

### Effective Searching Methods

1. First list directories to understand structure:

   ```
   list_vault_files(directory: "")
   list_vault_files(directory: "servers")
   ```

2. For searching by metadata:

   ```
   search_vault(query: "file.frontmatter.stars > 100", queryType: "dataview")
   search_vault(query: "file.frontmatter.status = 'active'", queryType: "dataview")
   ```

3. For text-based searches:

   ```
   search_vault_simple(query: "vector database")
   ```

4. For retrieving specific files:
   ```
   get_vault_file(filename: "servers/example-server.md", format: "markdown")
   ```

### Submitting Updates

To propose changes, format your output as a complete markdown file ready for inclusion in the vault. Include:

1. Full frontmatter metadata
2. Properly formatted sections following the template
3. Appropriate tagging
4. Source citations

Example PR format:

```
## Proposed Addition/Change
Server: [server-name]
Repository: [repo-url]
Reason for addition: [brief explanation]

[Complete formatted markdown for the server file]
```

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
