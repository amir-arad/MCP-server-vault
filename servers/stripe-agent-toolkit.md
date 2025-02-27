---
type: server
repo_url: https://github.com/stripe/agent-toolkit
name: Stripe
owner: stripe
stars: 0
last_updated: 2025-02-27
status: active
official: true
verified: false
sources: ["inbox"]
tags: ["status/active", "status/official", "category/integration"]
---

#status/active #status/official #category/integration

# Stripe

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
npm install @stripe/mcp-server
```

## Usage

```javascript
import { StripeServer } from "@stripe/mcp-server";

const server = new StripeServer({
  apiKey: "your-stripe-secret-key",
  webhookSecret: "your-webhook-secret",
});

// Create a payment intent
const paymentIntent = await server.createPaymentIntent({
  amount: 2000, // $20.00
  currency: "usd",
  paymentMethodTypes: ["card"],
  metadata: {
    orderId: "12345",
  },
});

// Handle subscriptions
const subscription = await server.createSubscription({
  customer: "cus_123",
  items: [{ price: "price_H123" }],
  paymentBehavior: "default_incomplete",
  metadata: {
    plan: "premium",
  },
});

// Process refunds
const refund = await server.createRefund({
  paymentIntent: "pi_123",
  amount: 1000, // $10.00
  reason: "requested_by_customer",
});

// Handle disputes
const dispute = await server.updateDispute({
  disputeId: "dp_123",
  evidence: {
    productDescription: "Detailed product description",
    serviceDate: "2025-02-27",
    shippingDocumentation: "file_123",
  },
});
```

## Dependencies

- Node.js >= 14.x
- Stripe account
- Stripe API keys
- Webhook endpoint (optional)

## Related Servers

- None currently listed
