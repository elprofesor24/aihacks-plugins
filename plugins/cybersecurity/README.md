# Cybersecurity

Security workflows and vulnerability checks for AI coding agents and MCP servers, through an AIhacks account. Published by MaxStrategy s.r.o.

## Installation in Claude Code

```
/plugin install cybersecurity --marketplace elprofesor24/aihacks-plugins
```

For Claude, ChatGPT or Codex, follow the connection guide at https://aihacks.cz/cybersecurity/.

## What the plugin includes and sends

- Entry skill `cybersecurity` with the working rules.
- Connection to the AIhacks MCP server at https://app.aihacks.cz/mcp/cybersecurity.

The plugin runs no code itself. The agent calls read-only tools:

- `list_workflows` and `get_workflow`: send the workflow id and file name.
- `check_dependencies`: sends ecosystem, package name and version; the server checks them against OSV (osv.dev) and the CISA Known Exploited Vulnerabilities catalog.
- `lookup_vulnerability`: sends a vulnerability id.

Conversation content, source code and secrets are not sent to the server.

## Account and access

Sign in with an AIhacks account (OAuth) on first use. Access requires an active Cybersecurity subscription managed at https://aihacks.cz, not in the plugin.

## Limits

Assisted review only, not an audit or penetration test; no guarantee that all vulnerabilities are found.

Operator: MaxStrategy s.r.o. · https://aihacks.cz · info@aihacks.cz · [Terms](https://aihacks.cz/podminky/) · [Privacy](https://aihacks.cz/soukromi/)
