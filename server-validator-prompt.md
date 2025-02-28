# MCP Server Validation Instructions

## Objective

Validate unverified servers (`verified: false`) by checking repository information and updating server details.

## Process Flow

1. **Find Unverified Servers**

   ```javascript
   search_vault({
     query: "{\"and\\":[{\"==\":[{\"var\\":\"type\\"},\"server\"]},{\"==\":[{\"var\":\"verified\"},false]}]}",
     queryType: "jsonlogic",
   });
   ```

2. **For Each Server:**

   - Get server file content: `get_vault_file({filename: "servers/owner-repo.md"})`
   - Visit repository URL to check:
     - Does repository exist?
     - Current star count
     - Repository activity
     - Ownership accuracy
     - Technology/Programming language
     - 3rd party systems integration
     - Documentation/README
     - Installation instructions
     - Examples, dependencies

3. **Update Server File:**

   - Set `verified: true`
   - Update `last_updated: YYYY-MM-DD` to current date
   - Correct `stars` count
   - Confirm/update `official` status
   - Update `status` if needed (active/inactive/deprecated)
   - Enhance description, features if better information found
   - Improve installation/usage examples if available
   - Add missing dependencies
   - Add related servers to inbox if discovered
   - Update or add missing tags (tech, integration etc.)

4. **Save Updated File:**
   ```javascript
   create_vault_file({
     filename: "servers/owner-repo.md",
     content: "complete updated content",
   });
   ```

## Validation Checklist

| Field           | Validation Action                                      |
| --------------- | ------------------------------------------------------ |
| repo_url        | Check existence and correctness                        |
| name            | Verify against repository name                         |
| owner           | Confirm GitHub owner matches                           |
| stars           | Update with current count                              |
| last_updated    | Set to today's date                                    |
| status          | Confirm if active/inactive/deprecated                  |
| official        | Verify if endorsed by official organization of product |
| verified        | Change to `true`                                       |
| tags            | Add/update based on actual functionality, tech etc.    |
| description     | Improve with information from README                   |
| features        | Add any missing features                               |
| installation    | Update if better instructions found                    |
| usage           | Enhance with actual examples from docs                 |
| dependencies    | List all required dependencies                         |
| related_servers | Add any connected servers                              |

## Handling Edge Cases

- **Repository doesn't exist:** Mark `status: "inactive"` or `status: "deprecated"`
- **Repository moved:** Update `repo_url` and note the change in description
- **Major changes to functionality:** Update all relevant sections to reflect current state
- **Limited documentation:** Extract what's available, note gaps in description

## Processing Strategy

1. For each server, follow all validation steps in order
2. Process all unverified servers until complete

## Tool Discipline

- Always include complete file content when updating
- Use proper date format: YYYY-MM-DD
- Maintain consistent formatting with existing standards
- Preserve any existing high-quality content
