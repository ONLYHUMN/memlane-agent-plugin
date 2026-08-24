# Memlane for Cursor

Cursor Agent Plugin for the [Memlane](https://memlane.app) MCP server.

Memlane is a relationship manager synced with Apple Contacts. Connect Cursor to [search contacts](https://memlane.app/guides/find-and-favorite-contacts), [read notes](https://memlane.app/guides/contact-dossiers), [move people on Lanes](https://memlane.app/guides/create-your-first-lane) as you build friendships, [work the Queue](https://memlane.app/guides/use-the-queue) of tasks, and [log promises](https://memlane.app/guides/open-promises). Destructive tools ask for a second yes. Requires [Memlane Pro](https://memlane.app/guides/memlane-pro) and [iCloud](https://memlane.app/guides/connect-icloud).

## What you can do

**Search contacts** — Find people by name, company, email, or phone. Cursor can pull up the right card before it drafts a message or answers a question about someone you know.

**Read notes** — Each contact has a dossier: facts, preferences, significant experiences, and free-form notes. Cursor can summarize what you already wrote so you do not repeat yourself in chat.

**Move people on Lanes** — Lanes are relationship tracks with stages (for example Met → Acquaintance → Friend on a Friendship lane). Cursor can move someone when a conversation shifts the relationship, and Memlane keeps the history.

**Work the Queue** — The Queue holds tasks from your Routines: reach-out nudges, birthday reminders, open promises, Meetup reminders, and more. Cursor can list what is pending and help you act on it.

**Log promises** — Track small commitments you owe or that others owe you, with optional due dates. Cursor can add or close promises so they stay visible until they are done.

**Deletes need your yes** — Tools that remove data return a confirmation summary first. Cursor reads it to you; nothing is deleted until you agree in the chat.

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
