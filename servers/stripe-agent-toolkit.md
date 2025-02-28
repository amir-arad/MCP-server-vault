---
type: server
repo_url: https://github.com/stripe/agent-toolkit
name: Stripe Agent Toolkit
owner: stripe
stars: 418
last_updated: 2025-02-28
status: active
official: true
verified: true
sources: ["inbox/batch_001.md"]
tags:
  [
    "status/active",
    "status/official",
    "category/integration",
    "integration/stripe",
    "purpose/payment-processing",
  ]
---

# Stripe Agent Toolkit

#status/active #status/official #category/integration #integration/stripe #purpose/payment-processing

## Description

Interact with Stripe API. This MCP server provides comprehensive integration with Stripe's payment processing and financial services platform.

## Features

- Payment processing
- Customer management
- Subscription handling
- Invoice generation
- Refund processing
- Payment method management
- Webhook handling
- Dispute management
- Account management
- Transaction reporting

## Installation

```bash
npm install @stripe/agent-toolkit
```

## Usage

```javascript
{
  "mcpServers": {
    "stripe": {
      "command": "npx",
      "args": ["@stripe/agent-toolkit"],
      "env": {
        "STRIPE_SECRET_KEY": "your-stripe-secret-key",
        "STRIPE_WEBHOOK_SECRET": "your-webhook-secret",
        "STRIPE_API_VERSION": "2025-02-21"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Stripe account
- Stripe API keys
- Webhook endpoint (optional)

## Related Servers

- None currently listed
