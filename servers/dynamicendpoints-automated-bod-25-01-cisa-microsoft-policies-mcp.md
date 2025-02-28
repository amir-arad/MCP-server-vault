---
type: server
repo_url: https://github.com/DynamicEndpoints/Automated-BOD-25-01-CISA-Microsoft-Policies-MCP
name: Automated BOD 25-01 CISA Microsoft Policies MCP Server
owner: DynamicEndpoints
stars: 2
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_003.md"]
tags: ["status/active", "category/security", "integration/microsoft365", "purpose/compliance", "tech/javascript", "integration/azure"]
---

# Automated BOD 25-01 CISA Microsoft Policies MCP Server

#status/active #category/security #integration/microsoft365 #purpose/compliance #tech/javascript #integration/azure

## Description

A Model Context Protocol (MCP) server implementing CISA Binding Operational Directive 25-01 security controls for Microsoft 365 (Azure AD/Entra ID). This server provides tools for configuring and managing Microsoft 365 security settings in accordance with BOD 25-01 requirements, integrating with Microsoft Graph API to enforce security controls, monitor compliance, and provide detailed reporting.

## Features

- Legacy authentication controls (blocks legacy authentication protocols)
- Risk-based access controls (blocks high-risk users and sign-ins)
- Multi-factor authentication management (enforces phishing-resistant MFA)
- Application registration and consent controls
- Password policy management (disables password expiration)
- Privileged role management (limits Global Administrator count)
- Cloud-only account enforcement
- PAM system integration
- Comprehensive compliance reporting
- Token-based authentication
- Type-safe argument validation
- Detailed error handling and logging

## Installation

```bash
# Clone the repository
git clone https://github.com/DynamicEndpoints/Automated-BOD-25-01-CISA-Microsoft-Policies-MCP.git
cd cisa-m365

# Install dependencies
npm install

# Build the server
npm run build
```

## Usage

```javascript
{
  "mcpServers": {
    "cisa-m365": {
      "command": "node",
      "args": ["path/to/cisa-m365/build/index.js"],
      "env": {
        "TENANT_ID": "your-tenant-id",
        "CLIENT_ID": "your-client-id",
        "CLIENT_SECRET": "your-client-secret"
      }
    }
  }
}
```

## Dependencies

- Node.js 18.x or higher
- Microsoft 365 tenant with admin access
- Azure AD application with required permissions:
  - Policy.ReadWrite.All
  - RoleManagement.ReadWrite.All
  - User.Read.All
  - Application.ReadWrite.All

## Related Servers

- [Microsoft Graph MCP Server](https://github.com/modelcontextprotocol/servers/tree/main/src/graph-server) - General Microsoft Graph API integration
- [Azure MCP Server](https://github.com/mashriram/azure-mcp-server) - Azure cloud services integration