# MCP Server Vault Inbox Processor

## Tools Instructions

- Only use the MCP-server-vault tool
- Read templates using get_vault_file
- Strictly adhere to template structure
- Always include complete file content after changes
- Never use "// rest of code remains the same" or similar shortcuts
- Never truncate with "..." or ellipses

## Processing Workflow

1. **Fetch Templates**

   - Read templates/server.md
   - Use these templates as strict reference for how to create new files
   - DO NOT include the templates or their schema in your work
   - NEVER use the `execute_template` command

2. **Scan Existing Structure**

   - Scan the vault for existing tags using the `search_vault` tool to understand the taxonomy and tagging standards
     ```javascript
     // Use this JsonLogic query to retrieve all tags from all files:
     {
       "query": "{\"var\": \"tags\"}",
       "queryType": "jsonlogic"
     }
     // This will return an array of objects containing filenames and their associated tags
     ```
   - Review existing server files to understand the format and content structure

3. **Process Inbox Entries**

   - Pick a file in ./inbox/\*:
   - For each entry in the file:
     - Parse owner name and server name from the repository URL or other link
     - Check if `servers/owner-repo.md` already exists
     - If it exists, update it with new information
     - If it doesn't exist, create a new server file

4. **For New Servers**

   - Create a new file at `servers/owner-repo.md` following the server.md template structure
   - Fill in all required fields:
     - repo_url: Repository URL from the entry
     - name: Human-readable title
     - owner: Repository owner
     - stars: Default to 0 if unknown
     - last_updated: Current date in YYYY-MM-DD format
     - status: Default to "active" unless specified otherwise
     - official: Boolean value (true/false)
     - verified: Default to false
     - sources: Array of source identifiers
     - tags: Array of relevant tags
   - Add appropriate content sections:
     - Description: Based on the entry description
     - Features: List of server features and capabilities
     - Installation: Installation instructions in bash format
     - Usage: Usage example in JavaScript format
     - Dependencies: List of required dependencies
     - Related Servers: Leave empty initially or add known related servers

5. **For New Sources**

   - Create a new file at `tags/source/source-name.md` following the source.md template structure
   - Fill in all required fields:
     - id: Unique identifier for the source
     - name: Display name of the source
     - url: URL where the source can be found
     - last_checked: Current date in YYYY-MM-DD format
     - servers_count: Default to 0
     - curator: Name of the curator maintaining the source
   - Add appropriate content sections:
     - Description: Brief description of the source
     - Servers from this source: Leave empty initially
     - Unique Servers: Leave empty initially

6. **Add Appropriate Tags**

   - Create or use existing tags based on:
     - Functionality (category tags)
     - Affiliation (integration tags)
     - Status (active, inactive, deprecated)
     - Technology (programming language, framework)
     - Purpose (development, data analysis, etc.)

7. **Process in Batches**
   - delete source file after each batch.
   - continue processing until the inbox is empty

## Important Notes

As an LLM agent, you are responsible for:

1. Extracting category and tag name from full tag paths
2. Formatting tag names for display (humanizing)
3. Converting single source strings to proper array format
4. Converting string booleans to proper boolean values
5. Generating current dates in YYYY-MM-DD format
6. Setting appropriate default values for required fields
7. Generating meaningful default content for new fields:
   - Features list based on description
   - Appropriate installation commands
   - Relevant usage examples
   - Required dependencies

## Processing Examples

- "**[Stripe](https://github.com/stripe/agent-toolkit)** - Interact with Stripe API" should be saved as "servers/stripe-agent-toolkit.md" with tags including #status/active #integration/stripe
- "**[Any Chat Completions](https://github.com/pyroprompts/any-chat-completions-mcp)** - Interact with any OpenAI SDK Compatible Chat Completions API" should be saved as "servers/pyroprompts-any-chat-completions-mcp.md" with tags including #status/active #category/llm
