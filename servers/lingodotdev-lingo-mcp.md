---
type: server
repo_url: https://github.com/lingodotdev/lingo.dev/blob/main/mcp.md
name: Lingo.dev
owner: lingodotdev
stars: 1400
last_updated: 2025-02-28
status: active
official: true
verified: true
sources: ["inbox"]
tags:
  [
    "status/active",
    "status/official",
    "category/utility",
    "category/communication",
    "tech/javascript",
  ]
---

# Lingo.dev

#status/active #status/official #category/utility #category/communication

## Description

Make your AI agent speak every language on the planet, using [Lingo.dev](https://lingo.dev) Localization Engine. This MCP server provides comprehensive localization and translation capabilities for AI agents.

## Features

- Multi-language support
- Real-time translation
- Context-aware localization
- Cultural adaptation
- Language detection
- Translation memory
- Terminology management
- Quality assurance checks
- Machine learning optimization
- Batch translation processing

## Installation

```bash
npm install @lingo/mcp-server
```

## Usage

```javascript
import { LingoServer } from "@lingo/mcp-server";

const server = new LingoServer({
  apiKey: "your-lingo-api-key",
  defaultLanguage: "en",
});

// Translate text to multiple languages
const translations = await server.translate({
  text: "Welcome to our platform!",
  targetLanguages: ["es", "fr", "de", "ja"],
  context: {
    domain: "website",
    component: "header",
  },
});

// Localize with cultural adaptation
const localizedContent = await server.localize({
  content: {
    greeting: "Good morning!",
    currency: "$10.99",
    dateFormat: "MM/DD/YYYY",
  },
  targetLocale: "fr-FR",
  adaptations: ["currency", "dateFormat", "timeFormat"],
});

// Batch process translations
const batchResults = await server.batchTranslate({
  items: [
    { key: "welcome", text: "Welcome" },
    { key: "goodbye", text: "Goodbye" },
  ],
  targetLanguages: ["es", "fr", "de"],
  preserveFormatting: true,
});
```

## Dependencies

- Node.js >= 14.x
- Lingo.dev API key
- Active Lingo.dev account

## Related Servers

- None currently listed
