1. Scan the vault for existing tags, and comprehend the taxonomy and tagging standards

2. Template Schemas:

   Server Template Schema:

   ```json
   {
     "type": "object",
     "required": [
       "url",
       "title",
       "owner",
       "description",
       "status",
       "official",
       "sources",
       "tags"
     ],
     "properties": {
       "url": {
         "type": "string",
         "description": "Repository URL, maps to repo_url in template"
       },
       "title": {
         "type": "string",
         "description": "Human-readable title, maps to name in template"
       },
       "owner": {
         "type": "string",
         "description": "Repository owner"
       },
       "description": {
         "type": "string",
         "description": "Server description"
       },
       "status": {
         "type": "string",
         "enum": ["active", "inactive", "deprecated"],
         "description": "Current status of the server"
       },
       "official": {
         "type": "boolean",
         "description": "Whether this is an official server"
       },
       "sources": {
         "type": "array",
         "items": {
           "type": "string"
         },
         "description": "Array of source identifiers"
       },
       "tags": {
         "type": "array",
         "items": {
           "type": "string"
         },
         "description": "Array of associated tags"
       }
     }
   }
   ```

   Tag Template Schema:

   ```json
   {
     "type": "object",
     "required": ["tag", "description", "tags"],
     "properties": {
       "tag": {
         "type": "string",
         "description": "Full tag path (e.g., 'category/tag-name')"
       },
       "description": {
         "type": "string",
         "description": "Brief description of tag purpose"
       },
       "tags": {
         "type": "array",
         "items": {
           "type": "string"
         },
         "description": "Array of related tags"
       }
     }
   }
   ```

3. Load template:

   ```
   execute_template(name: "templates/server.md", createFile: "false")
   ```

   Note: Always use "false" or "true" as strings for createFile parameter, not boolean values.

4. For each entry in inbox:

   - Parse owner name and server name. If the server has its own designated git repository, then extract these names from the repository's URL. else, try guess according to the link in the entry.
   - Check if `servers/owner-repo.md` exists

5. For new servers:

   - Transform data for template:

     - Format current date as YYYY-MM-DD for last_updated
     - Convert single source string to YAML array format: ["inbox"]
     - Convert "true"/"false" string to proper boolean for official field
     - Set default values:
       - stars: 0
       - verified: false
       - related_tags: []

   - Create note using template:

     ```
     execute_template(
       name: "templates/server.md",
       createFile: "true",  // Must be string "true", not boolean
       targetPath: "servers/owner-repo.md",
       arguments: {
         "url": "https://github.com/owner/repo",      // Maps to repo_url in template
         "title": "Human-readable title",             // Maps to name in template
         "owner": "owner",                            // Direct mapping
         "description": "Description from inbox",      // Used in content section
         "status": "active",                          // Must be one of: active, inactive, deprecated
         "official": true,                            // Must be boolean, not string
         "sources": ["inbox"],                        // Must be array format
         "tags": []                                   // Required empty array if no tags
       }
     )
     ```

   - Add appropriate tags based on functionality, affiliation and status

6. For each new tag:

   - Transform data for template:

     - Extract category and name from tag path
     - Format tag name for display
     - Set default values:
       - type: "tag"
       - servers_count: 0
       - related_tags: []

   - Create tag record:
     ```
     execute_template(
       name: "templates/tag.md",
       createFile: "true",  // Must be string "true", not boolean
       targetPath: "tags/category/tag-name.md",
       arguments: {
         "tag": "category/tag-name",                  // Maps to id and name in template
         "description": "Brief description of tag purpose", // Direct mapping
         "tags": []                                   // Required empty array if no tags
       }
     )
     ```

7. Process in batches of 5, updating Processing-Status.md after each batch.

Note: As an LLM agent, you are responsible for:

1. Extracting category and tag name from full tag paths
2. Formatting tag names for display (humanizing)
3. Converting single source strings to proper YAML array format: ["source"]
4. Converting "true"/"false" strings to proper boolean values
5. Generating current dates in YYYY-MM-DD format
6. Setting appropriate default values for required fields
7. Ensuring all template arguments match their schema definitions:
   - createFile must be string "true" or "false"
   - tags must be an array, even if empty
   - arrays must be properly formatted (e.g., ["item"])
   - boolean values must be actual booleans, not strings
   - status must be one of the enumerated values

Processing Examples

- "**[Stripe](https://github.com/stripe/agent-toolkit)** - Interact with Stripe API" should be saved as "servers/stripe-agent-toolkit.md" with tags including #status/active #integration/stripe
- "**[Any Chat Completions](https://github.com/pyroprompts/any-chat-completions-mcp)** - Interact with any OpenAI SDK Compatible Chat Completions API" should be saved as "servers/pyroprompts-any-chat-completions-mcp.md" with tags including #status/active #category/llm
