---
type: tag
id: <% tp.frontmatter.tag || tp.frontmatter.id %>
name: <% tp.frontmatter.tag ? tp.frontmatter.tag.split('/').pop().replace(/-/g, ' ') : tp.frontmatter.name %>
description: <% tp.frontmatter.description %>
servers_count: <% tp.frontmatter.servers_count || 0 %>
related_tags: <% tp.frontmatter.related_tags || [] %>
---

# <% tp.frontmatter.tag ? tp.frontmatter.tag.split('/').pop().replace(/-/g, ' ') : tp.frontmatter.name %>

<% tp.frontmatter.description %>

## Description

<% tp.frontmatter.long_description || tp.frontmatter.description %>

## Servers with this tag

<% (tp.frontmatter.servers || []).map(server => `- [${server.name}](${server.url})`).join("\n") %>

## Related Tags

<% (tp.frontmatter.related_tags || []).map(tag => `- [[${tag}]]`).join("\n") %>
