# AI Abilities

Bricks 2.4 introduced experimental abilities through the WordPress Abilities
API. When the user's authorized site exposes them through MCP or WP-CLI, prefer
these permission-aware operations over direct post-meta or option mutation.

## Start and discover

1. Call the start, version, and ability-status operations before planning a
   mutation.
2. Confirm the connected Bricks version, enabled abilities, authenticated user,
   and relevant WordPress and Builder permissions.
3. Use runtime schema and read operations for the exact resource. Do not assume
   that every registered ability is enabled or directly exposed as an MCP tool.
4. If an ability is not a direct tool, discover and call it through the MCP
   Adapter dispatcher rather than guessing a tool name or input shape.

Direct MCP tool names use hyphens while WordPress ability names use slashes.
Treat the runtime tool or ability schema as authoritative for its inputs and
outputs.

## Read, preview, apply, verify

- Read the current resource and its dependencies before editing.
- Prefer the focused checkout/preview/apply workflow for one resource and the
  site-changeset workflow for coordinated edits.
- Review preview warnings, omitted content, dependency changes, and destructive
  effects before applying.
- Re-read the resource after apply, then verify it in the Builder and on the
  frontend. Use returned revision IDs for rollback when supported.
- Remember that post and template element writes can create Bricks revisions,
  while global classes, variables, Theme Styles, components, and other global
  data are not protected by post revisions. Keep a separate recoverable backup
  for global writes.

If the required ability is unavailable, fall back to the Builder UI, supported
imports or public APIs, and finally the guarded direct-persistence workflow in
`validation-and-safety.md`.

## Security boundaries

- Treat the connection as the authenticated WordPress user. Site-wide ability
  toggles do not grant WordPress capabilities, Builder access, or Bricks
  permissions.
- Use a dedicated least-privilege user and enable only the abilities needed for
  the task. Test experimental write workflows on local or staging first.
- Require clear user authorization before an ability marked destructive or an
  operation that removes or overwrites data.
- Keep application passwords and MCP configuration secrets out of prompts,
  repositories, and output. Revoke credentials that are no longer needed.
- Do not enable PHP abilities merely to complete an ordinary content task. PHP
  execution is unsandboxed and requires its separate opt-in and permission
  checks; use it only in an explicitly authorized trusted environment.
