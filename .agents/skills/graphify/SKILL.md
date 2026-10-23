---
name: graphify
description: "Use for questions about Overtone code, architecture and file relationships. Query the checked-in local Graphify graph first; refresh it after code or dependency changes."
---

# Graphify for Overtone

Use this skill only for the Overtone repository. Follow its root instructions: work offline, keep Graphify outside the application dependencies, and never send project content to a remote service.

## Query the existing graph

When `graphify-out/graph.json` exists, use the local CLI before broad source searches:

```powershell
graphify query "<question about the codebase>"
graphify explain "<symbol or file>"
graphify path "<source node>" "<destination node>"
graphify affected "<symbol or file>"
```

Treat the graph as a navigation aid. Verify consequential findings in source files and distinguish Graphify's `EXTRACTED` relationships from `INFERRED` ones. Cite the source path and line returned by the graph when helpful.

## Refresh after code or dependency changes

Regenerate the local graph and its portable report and visualization:

```powershell
graphify extract . --code-only --cargo
graphify cluster-only . --no-label
```

Then inspect `graphify-out/GRAPH_REPORT.md` and open `graphify-out/graph.html`. Update `docs/project-map.md` to reflect source relationships, repository structure and current factual counts. `.graphifyignore` keeps generated output out of its own graph; Git ignores only machine-specific cache and root-marker files.

## Boundaries

- Never use URL inputs, `add`, GitHub/PR commands, MCP/HTTP services, semantic extraction, model backends, API keys, hooks, or file watchers for this repository.
- Never run installation or upgrade commands as part of a normal query or graph refresh. If Graphify is missing, report that and use the setup instructions in `docs/workflow.md`.
- Graphify parses code locally in `--code-only` mode. The checked-in graph covers code relationships; the Mermaid diagram and ownership table cover broader documentation and architecture.
