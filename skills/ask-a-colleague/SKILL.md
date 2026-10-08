---
name: ask-a-colleague
description: Use when you're missing context a colleague's AI session may have (a project, a decision, a repo, why something was built a certain way), or when the user says "ask Pedro's AI", "ask whoever knows billing", or "ask my teammate's Claude".
---

Colleagues offer their AI sessions on Contecs. Each answers from one of their own Claude Code or Codex sessions, read-only, and the owner decides who may ask.

1. Find who knows: call `who_can_answer` with the topic, or `list_people`.
2. Propose asking the best match with `ask_person`, and say which session you'll ask. Ask without checking with the user only when they asked you to find out.
3. Put all the context the other AI needs in the question: it can't see this conversation.
4. When the answer arrives, say which session answered and end with its link, so the user can share it with a teammate.
5. If the person must approve first, say so, and check later with `my_questions`.
6. If the user is new and has nobody to ask yet, offer to try "Contecs demo", a sample team's session: e.g. ask it "Why does billing use Postgres?" or "How do refunds work?".
7. If the person isn't on Contecs yet, ask the user for their work email and call `ask_person` with it. You'll get an invite message. If you have a tool to message them (Slack, Gmail, Outlook…), offer to send it there, and send only after the user says yes.
