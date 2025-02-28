---
repo_url: https://github.com/21st-dev/magic-mcp
owner: 21st-dev
name: magic-mcp
stars: 41
last_updated: 2025-02-28
status: active
official: true
verified: true
sources:
  - inbox
tags:
  - status/active
  - status/official
  - category/ui
  - category/code-generation
  - tech/typescript
  - purpose/development
  - integration/vscode
  - integration/cursor
---

# 21st.dev Magic

#status/active #status/official #category/ui #category/code-generation #tech/typescript #purpose/development #integration/vscode #integration/cursor

## Description

Magic Component Platform (MCP) is a powerful AI-driven tool that helps developers create beautiful, modern UI components instantly through natural language descriptions. It integrates seamlessly with popular IDEs and provides a streamlined workflow for UI development.

## Features

- **AI-Powered UI Generation**: Create UI components by describing them in natural language
- **Multi-IDE Support**:
  - Cursor IDE integration
  - Windsurf support
  - VSCode + Cline integration (Beta)
- **Modern Component Library**: Access to a vast collection of pre-built, customizable components inspired by 21st.dev
- **Real-time Preview**: Instantly see your components as you create them
- **TypeScript Support**: Full type-safe development
- **SVGL Integration**: Access to a vast collection of professional brand assets and logos
- **Component Enhancement**: Improve existing components with advanced features and animations

## Installation

For Cursor IDE:

```bash
npx -y @smithery/cli@latest run @21st-dev/magic-mcp --config "{\"TWENTY_FIRST_API_KEY\":\"your-api-key\"}"
```

For Windsurf:
Add to `~/.codeium/windsurf/mcp_config.json`:

```json
{
  "mcpServers": {
    "magic": {
      "command": "npx",
      "args": [
        "-y",
        "@smithery/cli@latest",
        "install",
        "@21st-dev/magic-mcp",
        "--client",
        "windsurf"
      ],
      "env": {
        "TWENTY_FIRST_API_KEY": "your-api-key"
      }
    }
  }
}
```

For VSCode + Cline (Beta):
Add to Cline's MCP configuration:

```json
{
  "mcpServers": {
    "magic": {
      "command": "npx",
      "args": [
        "-y",
        "@smithery/cli@latest",
        "install",
        "@21st-dev/magic-mcp",
        "--client",
        "cline"
      ],
      "env": {
        "TWENTY_FIRST_API_KEY": "your-api-key"
      }
    }
  }
}
```

## Dependencies

- Node.js (Latest LTS version recommended)
- One of the supported IDEs:
  - Cursor
  - Windsurf
  - VSCode (with Cline extension)

## Related Servers

- [EverArt](https://github.com/modelcontextprotocol/servers/tree/main/src/everart)
- [Lingo.dev](https://github.com/lingodotdev/lingo.dev/blob/main/mcp.md)
