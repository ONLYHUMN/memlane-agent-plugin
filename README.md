# Memlane for Cursor

Cursor Agent Plugin for the [Memlane](https://memlane.app) MCP server.

Memlane is a relationship manager synced with Apple Contacts. Connect Cursor to [search contacts](https://memlane.app/guides/find-and-favorite-contacts), [read notes](https://memlane.app/guides/contact-dossiers), [move people on Lanes](https://memlane.app/guides/create-your-first-lane), [work the Queue](https://memlane.app/guides/use-the-queue), and [log promises](https://memlane.app/guides/open-promises). Destructive tools ask for a second yes. Requires [Memlane Pro](https://memlane.app/guides/memlane-pro) and [iCloud](https://memlane.app/guides/connect-icloud).

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

Create a token in Memlane **Settings → MCP server**. Use `mcp.token.example.json` as a template and set `MEMLANE_MCP_TOKEN`. See the [MCP setup guide](https://memlane.app/guides/connect-an-ai-agent-with-mcp).

## Docs

- Agent landing: [memlane.app/developers](https://memlane.app/developers)
- Tool reference: [memlane.app/developers/mcp](https://memlane.app/developers/mcp)
- Setup guide: [Connect an AI agent with MCP](https://memlane.app/guides/connect-an-ai-agent-with-mcp)
- Privacy: [memlane.app/privacy](https://memlane.app/privacy)
- Support: support@memlane.app

## License

MIT
