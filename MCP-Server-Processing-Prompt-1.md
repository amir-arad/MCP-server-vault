# MCP Server Vault Processing Prompt

## Step 1: Understand the Project Context

```
First, review the vault structure to understand the project. Read these files in order:

1. README.md - For overall design philosophy and structure
2. templates/server.md - Template for server notes
3. templates/tag.md - Template for tag records
4. templates/source.md - Template for source records
5. tags/source/inbox.md - Information about the primary source
6. Processing-Status.md - Current progress and next steps
7. servers/cloudflare-mcp-server-cloudflare.md - Example server note
```

## Step 2: Process New Servers

```
Now, process the next batch of servers from Inbox.md:

1. For each server entry:
   - Extract GitHub URL, owner, name, description
   - Create a server note using the template
   - Fill frontmatter metadata with available information
   - Add "inbox" to sources list
   - Set status to "active" unless repository shows inactivity
   - Set official to "true" for servers in the "Official Integrations" section
   - Apply appropriate category tags based on server functionality

2. Avoid creating duplicates:
   - Check if filename "[owner]-[name].md" already exists
   - If exists, update the note with new sources instead

3. Extract information systematically:
   - Include full description from the repository
   - List key features based on the description
   - Add basic installation instructions if available
   - Link to related servers with similar functionality

4. Save each note in the servers/ directory with filename format:
   "[owner]-[name].md"
```

## Step 3: Create Missing Tag Records

```
For each tag you apply to a server note:

1. Check if a corresponding tag record exists in tags/
2. If not, create a new tag record using the template
3. Place it in the appropriate subdirectory:
   - tags/category/ for functionality categories
   - tags/tech/ for implementation technologies
   - tags/purpose/ for server purposes
   - tags/integration/ for specific service integrations
```

## Step 4: Track Progress

```
After processing each batch of servers:

1. Update Processing-Status.md with:
   - Number of servers processed
   - Number of new tags created
   - Current statistics on the vault
   - Any challenges encountered
```

## Processing Examples

- "**[Stripe](https://github.com/stripe/agent-toolkit)** - Interact with Stripe API" should be saved as "servers/stripe-agent-toolkit.md" with tags including #status/active #status/official #integration/stripe
- "**[Any Chat Completions](https://github.com/pyroprompts/any-chat-completions-mcp)** - Interact with any OpenAI SDK Compatible Chat Completions API" should be saved as "servers/pyroprompts-any-chat-completions-mcp.md" with tags including #status/active #status/community #category/llm

Process servers in batches of 5-10 to maintain quality and avoid exhausting the context window.
