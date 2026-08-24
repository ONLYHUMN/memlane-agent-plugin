# Memlane for Cursor

Cursor Agent Plugin for the [Memlane](https://memlane.app) MCP server.

Memlane is a relationship manager synced with Apple Contacts. Connect Cursor to search and update contacts, read and add notes, move people on [Lanes](https://memlane.app/guides/create-your-first-lane) as you build friendships, work the [Queue](https://memlane.app/guides/use-the-queue) of tasks, and log [promises](https://memlane.app/guides/open-promises). Destructive tools ask for a second yes. Requires [Memlane Pro](https://memlane.app/guides/memlane-pro) and [iCloud](https://memlane.app/guides/connect-icloud).

The server exposes **50 tools** — reads, writes, and guarded deletes. Full list: [memlane.app/developers/mcp](https://memlane.app/developers/mcp).

## What you can do

**Contacts** — [Search](https://memlane.app/guides/find-and-favorite-contacts) and open profiles, create new people, set [contact lists](https://memlane.app/guides/use-contact-lists), and link [related people](https://memlane.app/guides/related-people). Cursor can find someone before it drafts a message or updates a card.

**Notes (dossiers)** — [Read, search, add, and edit](https://memlane.app/guides/contact-dossiers) notes in categories such as Facts, Preferences, and Significant Experiences. Cursor can capture what you learned in chat and save it to the right person.

**Lanes** — List lanes and stages, add people, and [move them as relationships grow](https://memlane.app/guides/create-your-first-lane). Cursor can create lanes and stages, rename them, and reorder stages when your workflow changes.

**Queue and Routines** — [List the Queue](https://memlane.app/guides/use-the-queue), complete items, and inspect [Routines](https://memlane.app/guides/routines-and-queue) that feed it. Reach-out nudges, birthday reminders, and promise tasks can be cleared from chat.

**Promises** — [List, create, update, and close](https://memlane.app/guides/open-promises) commitments you owe or that others owe you. Cursor can log a promise when someone asks you to follow up.

**Meetups** — List recurring gatherings, edit schedules, skip the next occurrence, or turn a contact list into a Meetup. See [Meetups](https://memlane.app/guides/meetups).

**Relationship Map** — Read how people connect on the [Map](https://memlane.app/guides/relationship-map). Cursor can answer “how is Alex related to Jordan?” from your graph.

**Reconciliation** — List and resolve [reconciliation tasks](https://memlane.app/guides/reconciliation-inbox) when iCloud sync needs a human decision.

**Reach-out schedules** — Set or change when Memlane nudges you to [stay in touch](https://memlane.app/guides/reach-out-schedules) with someone.

**Log connections** — Record that you reached out, which can clear Queue items and update last-connected dates. See [Log a connection](https://memlane.app/guides/log-a-connection).

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
