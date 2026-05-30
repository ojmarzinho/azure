---
description: GTD-style processing of everything in Inbox/. Categorizes, routes, and acts on captured notes. Keeps the inbox at zero.
---

# /inbox

Process everything in `obsidian/Inbox/` to zero.

## GTD Decision Tree (per item)

1. **What is it?** — Read the capture
2. **Is it actionable?**
   - NO: Archive, Reference, or Delete
   - YES: continue...
3. **Will it take < 2 minutes?**
   - YES: Do it now (or note the action)
   - NO: continue...
4. **Route it**:
   - Project: add to `obsidian/Projects/[project]/` and update CLAUDE.md
   - Reference: trigger `/ingest`
   - Goal-related: add to relevant Goals/ file
   - Daily task: add to today's Daily Note
   - Someday/Maybe: `obsidian/Archives/someday.md`

## Output
Report counts: items routed, ingested, added to goals, archived. Inbox empty when done.
