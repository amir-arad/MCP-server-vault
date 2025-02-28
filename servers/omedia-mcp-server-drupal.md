---
type: server
repo_url: https://github.com/Omedia/mcp-server-drupal
name: Drupal MCP Server
owner: Omedia
stars: 24
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_010.md"]
tags:
  [
    "status/active",
    "category/cms",
    "integration/drupal",
    "purpose/content-management",
    "purpose/user-administration",
    "purpose/site-configuration",
  ]
---

# Drupal MCP Server

#status/active #category/cms #integration/drupal #purpose/content-management #purpose/user-administration #purpose/site-configuration

## Description

Integrates with Drupal's API to enable content management, user administration, and site configuration for automated website operations and personalized content delivery.

## Features

- Content management
- User administration
- Site configuration
- Content type management
- Taxonomy management
- User role management
- Module administration
- Theme configuration
- View management
- Block placement

## Installation

```bash
composer require omedia/mcp-server-drupal
```

## Usage

```javascript
{
  "mcpServers": {
    "drupal": {
      "command": "vendor/bin/drupal-mcp",
      "env": {
        "DRUPAL_ROOT": "/var/www/html",
        "DRUPAL_BASE_URL": "https://example.com",
        "DRUPAL_USER": "admin",
        "DRUPAL_PASS": "your-secure-password"
      }
    }
  }
}
```

## Dependencies

- PHP >= 8.0
- Drupal >= 9.0
- Composer
- Drush
- Database (MySQL/PostgreSQL)
- Web server (Apache/Nginx)

## Related Servers

- None currently listed
