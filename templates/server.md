---
type: server
repo_url: <% tp.frontmatter.url %>
name: <% tp.frontmatter.title %>
owner: <% tp.frontmatter.owner %>
stars: <% tp.frontmatter.stars || 0 %>
last_updated: <% tp.date.now("YYYY-MM-DD") %>
status: <% tp.frontmatter.status %>
official: <% tp.frontmatter.official %>
verified: false
sources: <% tp.frontmatter.sources %>
related_tags: <% tp.frontmatter.related_tags || [] %>
---

# <% tp.file.title %>

## Description

<% tp.frontmatter.description %>

## Features

<% (tp.frontmatter.features || []).join("\n") %>

## Installation

```bash
<% tp.frontmatter.installation || "" %>
```

## Usage

```javascript
<% tp.frontmatter.usage || "" %>
```

## Dependencies

<% (tp.frontmatter.dependencies || []).join("\n") %>

## Related Servers

<% (tp.frontmatter.related || []).map(server => `- [${server.name}](${server.url})`).join("\n") %>
