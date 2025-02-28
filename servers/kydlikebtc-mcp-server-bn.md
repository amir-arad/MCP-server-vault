---
type: server
repo_url: https://github.com/kydlikebtc/mcp-server-bn
name: Binance Spot Trading MCP Server
owner: kydlikebtc
stars: 2
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_004.md"]
tags:
  [
    "status/active",
    "category/finance",
    "integration/binance",
    "purpose/trading",
    "category/cryptocurrency",
  ]
---

# Binance Spot Trading MCP Server

#status/active #category/finance #integration/binance #purpose/trading #category/cryptocurrency

## Description

This server provides a robust interface for Binance spot trading operations, including secure management of API credentials, execution and management of spot orders, and monitoring of account balances and open orders.

## Features

### Spot Trading Operations

- Execute spot trading operations (LIMIT/MARKET orders)
- Monitor account balances
- Track and manage open orders
- Cancel existing orders

## Tools

#### API Configuration

##### `configure_api_keys`

Securely store your Binance API credentials:

```javascript
await configureBinanceApiKeys({
  apiKey: "your-api-key",
  apiSecret: "your-api-secret",
});
```

#### Spot Trading Tools

##### `create_spot_order`

Create LIMIT or MARKET orders:

```javascript
// LIMIT order
await createSpotOrder({
  symbol: "BTCUSDT",
  side: "BUY",
  type: "LIMIT",
  quantity: "0.001",
  price: "40000",
});

// MARKET order
await createSpotOrder({
  symbol: "BTCUSDT",
  side: "BUY",
  type: "MARKET",
  quantity: "0.001",
});
```

##### `cancel_order`

Cancel an existing order:

```javascript
await cancelOrder({
  symbol: "BTCUSDT",
  orderId: "12345678",
});
```

##### `get_balances`

Check your account balances:

```javascript
const balances = await getBalances();
// Returns: { BTC: '0.1', USDT: '1000', ... }
```

##### `get_open_orders`

List all open orders:

```javascript
const orders = await getOpenOrders({
  symbol: "BTCUSDT", // Optional: specify symbol
});
```

## Usage

```javascript
{
  "mcpServers": {
    "binance-spot": {
      "command": "npx",
      "args": ["@kydlikebtc/mcp-server-bn"],
      "env": {
        "BINANCE_API_KEY": "your-api-key",
        "BINANCE_SECRET_KEY": "your-secret-key",
        "TRADE_PAIRS": "BTC/USDT,ETH/USDT",
        "ORDER_TIMEOUT": "30"
      }
    }
  }
}
```

## Dependencies

- Node.js >= 14
- Binance account
- API credentials
- Trading permissions

## Related Servers

- qeinfinity/binance-mcp-server
