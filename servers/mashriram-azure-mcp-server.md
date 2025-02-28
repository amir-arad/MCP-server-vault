---
type: server
repo_url: https://github.com/mashriram/azure_mcp_server
name: Azure MCP Server
owner: mashriram
stars: 0
last_updated: 2025-02-28
status: active
official: false
verified: true
sources: ["inbox/batch_003.md"]
tags:
  [
    "status/active",
    "category/cloud",
    "integration/azure",
    "integration/blob-storage",
    "integration/cosmos-db",
  ]
---

# Azure MCP Server

#status/active #category/cloud #integration/azure #integration/blob-storage #integration/cosmos-db

## Description

This server implements the Model Context Protocol for seamless interaction with Azure Blob Storage and Cosmos DB, enabling automatic logging and audit tracking of operations. All operations performed through this server are automatically logged and accessible via the `audit://azure-operations` resource endpoint.

## Features

### Azure Blob Storage Operations

- blob_container_create: Creates a new Blob Storage container. Requires the `container_name`.
- blob_container_list: Lists all Blob Storage containers in the configured account.
- blob_container_delete: Deletes a Blob Storage container. Requires the `container_name`.
- blob_upload: Uploads a blob (file) to a Blob Storage container. Requires the `container_name`, `blob_name`, and the `file_content` (Base64 encoded).
- blob_delete: Deletes a blob from a Blob Storage container. Requires the `container_name` and `blob_name`.
- blob_list: Lists the blobs within a Blob Storage container. Requires the `container_name`.
- blob_read: Reads the content of a blob from Blob Storage. Requires the `container_name` and `blob_name`. Returns the content as text.

### Azure Cosmos DB (NoSQL API) Operations

#### Container Operations

- cosmosdb_container_create: Creates a new Cosmos DB container within a database. Requires the `container_name` and `partition_key`. The `database_name` is optional and defaults to `defaultdb`. The `partition_key` should be a JSON object defining the partition key (e.g., `{"paths": ["/myPartitionKey"], "kind": "Hash"}`).
- cosmosdb_container_describe: Retrieves details about a Cosmos DB container. Requires the `container_name`. The `database_name` is optional and defaults to `defaultdb`.
- cosmosdb_container_list: Lists all Cosmos DB containers within a database. The `database_name` is optional and defaults to `defaultdb`.
- cosmosdb_container_delete: Deletes a Cosmos DB container. Requires the `container_name`. The `database_name` is optional and defaults to `defaultdb`.

#### Item Operations

- cosmosdb_item_create: Creates a new item within a Cosmos DB container. Requires the `container_name` and the `item` (a JSON object representing the item). The `database_name` is optional and defaults to `defaultdb`. Make sure your `item` includes the partition key field and value.
- cosmosdb*item_read: Reads an item from a Cosmos DB container. Requires the `container_name`, `item_id`, and `partition_key`. The `database_name` is optional and defaults to `defaultdb`. The `partition_key` \_must* match the partition key value of the item being read.
- cosmosdb*item_replace: Replaces an existing item within a Cosmos DB container. Requires the `container_name`, `item_id`, `partition_key`, and the `item` (a JSON object representing the \_complete* updated item). The `database_name` is optional and defaults to `defaultdb`. The `partition_key` _must_ match the partition key value of the item being replaced.
- cosmosdb*item_delete: Deletes an item from a Cosmos DB container. Requires the `container_name`, `item_id`, and `partition_key`. The `database_name` is optional and defaults to `defaultdb`. The `partition_key` \_must* match the partition key value of the item being deleted.
- cosmosdb_item_query: Queries items in a Cosmos DB container using a SQL query. Requires the `container_name` and `query`. The `database_name` is optional and defaults to `defaultdb`. Optionally accepts a `parameters` array for parameterized queries.

**Important Cosmos DB Notes:**

- **Partition Keys:** Cosmos DB requires a partition key for efficient data storage and retrieval. When creating containers, you _must_ define a partition key. When reading, replacing, or deleting items, you _must_ provide the correct partition key value for the item you are accessing. The partition key is a property _within_ your data.
- **Case Sensitivity:** Cosmos DB resource names (databases, containers, item IDs) and partition key values are case-sensitive. Ensure that you use the correct casing in your tool calls.
- **Default Database:** If the `database_name` is not provided, the server defaults to a database named `SampleDB`. Ensure this database exists, or explicitly provide the name of your desired database in the tool call arguments.

## Installation

To install Azure MCP Server for Claude Desktop automatically via [Smithery](https://smithery.ai/server/@mashriram/azure_mcp_server):

```bash
npx -y @smithery/cli install @mashriram/azure_mcp_server --client claude
```

## Usage

1.  **Clone the Repository:** Clone this repository to your local machine.
2.  **Configure Azure Credentials:** Configure your Azure credentials. This server requires an Azure account with appropriate permissions for Blob Storage and Cosmos DB. We recommend using `DefaultAzureCredential` which attempts to authenticate via various methods in order.

    - **Environment Variables:** Set the following environment variables:
      - `AZURE_STORAGE_ACCOUNT_URL`: The URL of your Azure Storage account (e.g., `https://<your_account_name>.blob.core.windows.net`).
      - `AZURE_COSMOSDB_ENDPOINT`: The endpoint URL for your Azure Cosmos DB account.
      - `AZURE_COSMOSDB_KEY`: The primary or secondary key for your Azure Cosmos DB account. **Important: Treat this key like a password and keep it secure.**
    - **Azure CLI:** Alternatively, you can authenticate using the Azure CLI. Ensure you are logged in with an account that has the necessary permissions. This server uses `DefaultAzureCredential` so it will automatically authenticate with the Azure CLI credentials if environment variables are not specified. Use `az login` to log in.

3.  **Configure Claude Desktop:** Add the following configuration to your `claude_desktop_config.json` file:

    - **macOS:** `~/Library/Application\ Support/Claude/claude_desktop_config.json`
    - **Windows:** `%APPDATA%/Claude/claude_desktop_config.json`

```json
"mcpServers": {
  "mcp-server-azure": {
    "command": "uv",
    "args": [
      "--directory",
      "/path/to/repo/azure-mcp-server",
      "run",
      "azure-mcp-server"
    ]
  }
}
```

Replace `/path/to/repo/azure-mcp-server` with the actual path to the cloned repository.

4.  **Install and Launch Claude Desktop:** Install and open the [Claude desktop app](https://claude.ai/download).
5.  **Test the Setup:** Ask Claude to perform a read or write operation using the Azure tools (e.g., create a Blob Storage container or add an item to Cosmos DB). If you encounter issues, consult the MCP debugging documentation [here](https://modelcontextprotocol.io/docs/tools/debugging).

## Dependencies

- Node.js >= 14
- Azure subscription
- Storage account
- Cosmos DB instance
