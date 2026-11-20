---
name: cybersecurity
description: "Use for security review of AI agents, MCP servers, applications, APIs, Docker and Compose configurations, secrets handling and dependencies. Loads the matching Cybersecurity workflow through the cybersecurity MCP server and checks exact package versions or vulnerability ids against OSV and CISA KEV."
---

# Cybersecurity

Security workflows and vulnerability checks for AI coding agents, through an AIhacks account.

## How to use

1. Call `list_workflows` and pick the workflow that matches the task (for example MCP server security, AI agent security, authentication, API security, Docker and Compose, dependencies).
2. Call `get_workflow` with its `id` and follow it while you review the user's project in this session.
3. For dependencies, call `check_dependencies` with the ecosystem, package name and exact installed version (from the lockfile, not a version range). For a known id, call `lookup_vulnerability` with the CVE, GHSA or OSV id.
4. Report each finding with evidence, a confidence of `confirmed`, `potential` or `unknown`, the impact and a fix (see the `security-finding-report` workflow).

## Rules (always apply, even without access)

- This is an assisted review, not an audit or a penetration test, and it does not guarantee that all vulnerabilities are found. Never claim the project is secure.
- A tool status of `unknown` means the check could not be completed. Say so; never present it as "no known vulnerabilities".
- Only test systems the user owns or is authorised to test.
- Send the server only package names, versions and vulnerability ids. Never send source code, secrets or tokens.
- Without active access the server returns availability information only. Tell the user and do not invent the workflow content.
