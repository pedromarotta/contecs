# Contecs

Ask a colleague's AI coding session from your own chat. Their Claude Code, Codex or OpenCode session answers, from a copy that never changes it. They decide who may ask: people on their list ask directly, anyone else waits for their approval and can only read.

![Ana's Claude asks Pedro's AI while he's at lunch](demo.gif)

## Install in Claude Code

```bash
claude plugin install contecs --marketplace pedromarotta/contecs
```

(Claude Code 2.1.292 or newer. On older versions: `claude plugin marketplace add pedromarotta/contecs`, then `claude plugin install contecs@contecs`.)

Then try it alone: ask Claude *"ask the Contecs demo why billing uses Postgres"*. It answers from a sample team's session in a few seconds.

That adds the Contecs connector (sign in with Google or GitHub the first time you use it) and two skills: asking a colleague's AI, and setting up your own sessions to answer.

## Install in Codex

```bash
codex plugin marketplace add pedromarotta/contecs
codex plugin add contecs@contecs
```

Same connector and skills. If Codex doesn't prompt you to sign in, run `codex mcp login contecs`. To update later: `codex plugin marketplace upgrade`.

## Answer questions from your sessions

On a Mac with Claude Code, Codex or OpenCode:

```bash
curl -fsSL https://contex.fly.dev/install | zsh
```

Or start at [contex.fly.dev/start](https://contex.fly.dev/start).

## Other AI clients

The connector works in any client that supports remote MCP servers: claude.ai, ChatGPT, Cursor and others. Add `https://contex.fly.dev/mcp` as a custom connector.

Questions and bugs: open an issue.
