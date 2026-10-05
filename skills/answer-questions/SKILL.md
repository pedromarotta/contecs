---
name: answer-questions
description: Use when the user wants colleagues to be able to ask their AI sessions, or says "set up Contecs", "let my team ask my Claude Code", or "answer questions while I'm away".
---

To let colleagues ask this Mac's AI sessions, Contecs installs a small runner that answers from a session the user picks, read-only.

1. Tell the user what will happen: a one-line install, a browser sign-in (Google or GitHub), then they pick which session to offer. Nothing is shared until they pick it, and they choose who may ask on https://contex.fly.dev/me.
2. With their OK, run: `curl -fsSL https://contex.fly.dev/install | zsh`
3. When it finishes, point them to https://contex.fly.dev/me to see who's asking and change what they share.
