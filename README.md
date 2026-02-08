# Weave for Zed

A [Zed](https://zed.dev) extension that integrates [Weave](https://github.com/Ataraxy-Labs/weave)'s entity-level semantic merge coordination into the Agent Panel via MCP.

## Tools

| Tool | Description |
|------|-------------|
| `weave_extract_entities` | List all functions, classes, methods in a file |
| `weave_claim_entity` | Claim an entity before editing (advisory lock) |
| `weave_release_entity` | Release a claim after editing |
| `weave_status` | Show entity status with claim/modification info |
| `weave_who_is_editing` | Check if anyone is editing a specific entity |
| `weave_potential_conflicts` | Detect entities being edited by multiple agents |
| `weave_preview_merge` | Dry-run merge analysis between branches |
| `weave_agent_register` | Register an agent in coordination state |
| `weave_agent_heartbeat` | Keep-alive with current working state |

## Install

Search for "Weave" in Zed's extension marketplace, or install as a dev extension during development.

## How it works

The extension downloads the `weave-mcp` binary from GitHub Releases and runs it as an MCP context server. Weave uses [sem-core](https://github.com/Ataraxy-Labs/sem) with tree-sitter to extract semantic entities from source code, enabling entity-level coordination for multi-agent development workflows.
