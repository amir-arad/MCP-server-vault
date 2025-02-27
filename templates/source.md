---
type: source
id: <% tp.frontmatter.id %>
name: <% tp.frontmatter.name %>
url: <% tp.frontmatter.url %>
last_checked: <% tp.date.now("YYYY-MM-DD") %>
servers_count: <% tp.frontmatter.servers_count || 0 %>
curator: <% tp.frontmatter.curator %>
---

# <% tp.frontmatter.name %>

A curated list of MCP servers maintained by <% tp.frontmatter.curator || "unknown curator" %>.

## Description

<% tp.frontmatter.description || "No description provided." %>

## Last Check

This source was last checked on <% tp.date.now("YYYY-MM-DD") %>.

## Servers from this source

<% (tp.frontmatter.servers || []).map(server => `- [${server.name}](${server.url})`).join("\n") %>

## Unique Servers

<% (tp.frontmatter.unique_servers || []).map(server => `- [${server.name}](${server.url})`).join("\n") %>
