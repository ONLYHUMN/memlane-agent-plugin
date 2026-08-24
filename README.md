# Memlane for Cursor

Cursor Agent Plugin for the [Memlane](https://memlane.app) MCP server.

Memlane is a relationship manager synced with Apple Contacts. Connect Cursor to search contacts, read notes, move people on Lanes, work the Queue, and log promises. Destructive tools ask for a second yes. Requires Memlane Pro and iCloud.

## Install

1. Submit or install this plugin from the [Cursor Marketplace](https://cursor.com/marketplace).
2. Open **Customize → MCPs** in Cursor and enable **Memlane**.
3. Sign in to Memlane and choose **Allow** when OAuth opens.

## Manual setup

Copy `mcp.json` into your Cursor MCP config, or symlink this repo:

```bash
ln -s "$(pwd)" ~/.cursor/plugins/local/memlane
```

Then reload Cursor (**Developer: Reload Window**).

## Token auth (optional)

Create a token in Memlane **Settings → MCP server**. Use `mcp.token.example.json` as a template and set `MEMLANE_MCP_TOKEN`.

## Docs

- Agent landing: https://memlane.app/developers
- Tool reference: https://memlane.app/developers/mcp
- Setup guide: https://memlane.app/guides/connect-an-ai-agent-with-mcp
- Privacy: https://memlane.app/privacy
- Support: support@memlane.app

## License

MIT
