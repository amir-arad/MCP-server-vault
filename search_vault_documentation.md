# search_vault Tool Documentation

This document contains validated information about using the `search_vault` tool in the MCP-server-vault MCP server.

## Basic Usage

The `search_vault` tool allows searching for documents in an Obsidian vault using structured queries. While the tool documentation mentions support for two query formats (Dataview DQL and JsonLogic), testing has confirmed that only JsonLogic queries are working reliably in the current implementation.

```javascript
// Tool parameters
{
  "query": string,       // Required: The query string
  "queryType": string    // Required: Use "jsonlogic" for reliable results
}
```

## Query Type Support

- **JsonLogic**: ✅ Fully functional when properly formatted
- **Dataview DQL**: ❌ Currently returns errors ("Cannot read properties of undefined (reading 'tryQuery')")

## Validated JsonLogic Query Format

When using JsonLogic queries (`queryType: "jsonlogic"`), the query must be provided as a **JSON string**, not a JSON object:

```javascript
// Correct
{
  "query": "{\"var\": \"tags\"}",
  "queryType": "jsonlogic"
}

// Incorrect - will produce an error
{
  "query": {"var": "tags"},
  "queryType": "jsonlogic"
}
```

## Getting All Tags

The following query successfully retrieves all tags from all files in the vault:

```javascript
{
  "query": "{\"var\": \"tags\"}",
  "queryType": "jsonlogic"
}
```

This returns an array of objects, each containing a filename and its associated tags:

```javascript
[
  {
    filename: "path/to/file.md",
    result: ["tag1", "tag2", "tag3"],
  },
  // ... more files
];
```

## Response Format

The response is an array of objects with the following structure:

```javascript
{
  "filename": string,    // Path to the matching file
  "result": any          // The query result (can be string, number, array, object, or boolean)
}
```

## Practical Usage Examples

### Find Files with a Specific Tag

```javascript
{
  "query": "{\"in\": [\"category/database\", {\"var\": \"tags\"}]}",
  "queryType": "jsonlogic"
}
```

### Find All Files (returns all files with result: true)

```javascript
{
  "query": "{\"!==\": [{\"var\": \"\"}, null]}",
  "queryType": "jsonlogic"
}
```

# JsonLogic Query for Unverified Servers

This document demonstrates a working JsonLogic query that lists all files with `verified: false` in their frontmatter.

### Unverified Servers

```javascript

{
  "query": "{\"and\": [{\"===\": [{\"var\": \"frontmatter.verified\"}, false]}, {\"===\": [{\"var\": \"frontmatter.type\"}, \"server\"]}]}",
  "queryType": "jsonlogic"
}

```

## Notes

- When constructing JsonLogic queries, remember to escape quotes and properly stringify the JSON object
- Files without the queried property (e.g., files without tags when querying for tags) will not appear in the results
