# MCP Server Vault Processing Prompt

## Context and Purpose

You will help process the inbox into structured notes for my vault. This vault serves as a comprehensive database of Model Context Protocol (MCP) servers with rich metadata and tagging. Before beginning any processing tasks, please review the following files to understand the project structure:

1. First read `README.md` to understand the overall design philosophy and organization
2. Examine the template files in the `templates/` directory
3. Review a few example server notes in the `servers/` directory
4. Check the tag records in `tags/` to understand the tagging system
5. Finally, review `Processing-Status.md` to see what has been done and what remains

After examining these files, please continue processing the MCP server entries from `Inbox.md` into individual structured notes following the established pattern.

## Processing Instructions

For each MCP server in the inbox that doesn't already have a note:

1. **Extract Essential Information**:

   - Repository URL (GitHub)
   - Owner and repository name
   - Description
   - Features and capabilities
   - Installation instructions (if available)
   - Related servers

2. **Apply Metadata in Frontmatter**:

   - Use the repository URL as the canonical identifier
   - Structure the frontmatter according to the server template
   - Include sources where this server was found
   - Set appropriate status (active/inactive)
   - Mark as official if maintained by the service provider

3. **Apply Appropriate Tags**:

   - Status tags (`status/active`, `status/official`, etc.)
   - Category tags based on server functionality
   - Technology tags based on implementation
   - Purpose and integration tags as appropriate

4. **Format Content Sections** according to the server template:

   - Description
   - Features
   - Installation
   - Authentication (if applicable)
   - Dependencies
   - Related Servers

5. **Naming Convention**:
   - Use `owner-name.md` format for the filename
   - Place in the `servers/` directory

## Processing Guidelines

1. **Process in Batches**: Work on 5-10 servers at a time rather than attempting to process all entries at once
2. **Focus on Quality**: Prioritize accuracy in categorization and metadata over quantity
3. **Maintain Consistency**: Follow the established patterns from the templates precisely
4. **Avoid Duplicates**: Check if a server already exists before creating a new note
5. **Infer Missing Information**: Make reasonable inferences when information is incomplete, but note uncertainties
6. **Preserve Original Links**: Always maintain all repository URLs exactly as they appear
7. **Record Progress**: Update `Processing-Status.md` after each batch to track progress

## Starting Instructions

1. Read the specified context files to familiarize yourself with the project structure
2. Identify the next 5 unprocessed servers from the inbox
3. Process each server according to the guidelines, using the existing templates
4. For each server, create a note following the server template format
5. Update the progress tracking in `Processing-Status.md`

Thank you for your assistance in building this comprehensive MCP server database.
