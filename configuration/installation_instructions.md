The Weave MCP server binary is downloaded automatically from [GitHub Releases](https://github.com/Ataraxy-Labs/weave/releases).

No additional configuration is required. Weave auto-detects the git repository from your project's working directory.

Weave provides entity-level tools for multi-agent coordination:

- **weave_extract_entities** — list functions, classes, and methods in a file
- **weave_claim_entity** / **weave_release_entity** — advisory locks before editing
- **weave_status** / **weave_who_is_editing** — see what's being edited
- **weave_potential_conflicts** — detect concurrent edits on related code
- **weave_preview_merge** — dry-run merge analysis between branches
- **weave_diff** — semantic diff showing entity-level changes
