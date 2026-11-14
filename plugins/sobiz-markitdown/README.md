# Sobiz MarkItDown Claude plugin

This plugin connects Claude to Microsoft's published `markitdown-mcp` using `uvx`. It does **not** execute the fork's Python source; update the MCP package independently if needed.

## Windows prerequisites

Install [uv](https://docs.astral.sh/uv/getting-started/installation/) and ensure `uvx` is on PATH:

```powershell
winget install --id astral-sh.uv -e
uvx --version
```

## Install

In Claude Code:

```text
/plugin marketplace add bizsolutionbyai/markitdown
/plugin install sobiz-markitdown@sobiz-marketplace
```

Reload plugins or restart Claude if prompted. Verify the `markitdown` MCP server is connected using `/mcp`.

## Troubleshooting

- Marketplace not found: confirm `.claude-plugin/marketplace.json` is merged to the default branch.
- MCP fails: run `uvx markitdown-mcp` in a terminal to diagnose Python/package installation.
- Tool not visible: reload plugins and inspect MCP status.
- The MCP tool may not support every file format or preserve every layout element.

## Upstream

The parent repository is `microsoft/markitdown`. Keep Sobiz additions in `.claude-plugin/` and `plugins/sobiz-markitdown/`. Sync Microsoft upstream by reviewing a pull request, resolving conflicts, and rerunning validation.
