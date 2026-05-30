---
description: Morning planning and evening reflection. Creates today's daily note from template, surfaces ONE Big Thing, reviews active projects, and links to goals.
---

# /daily

## Morning Mode (run before noon)

1. Create `obsidian/Daily Notes/YYYY-MM-DD.md` if it doesn't exist:
   ```markdown
   ---
   type: daily
   created: YYYY-MM-DD
   updated: YYYY-MM-DD
   tags: [daily]
   ---
   # YYYY-MM-DD
   
   ## ONE Big Thing
   > [Surface from Goals/ — what matters most today]
   
   ## Active Projects
   - [[Project A]] — next action: ...
   - [[Project B]] — next action: ...
   
   ## Captures
   - 
   
   ## Evening Reflection
   - What did I actually do?
   - Did it align with the ONE Big Thing?
   - One thing I learned:
   ```

2. Read `obsidian/Goals/Monthly Goals.md` and surface the single most important task for today
3. List the 2-3 most active Projects (those with recent updates)
4. Check `obsidian/Inbox/` — if >3 items, remind to run `/inbox`
5. Ask: "What's blocking the ONE Big Thing?"

## Evening Mode (run after 5pm)

1. Open today's note
2. Prompt user to fill Evening Reflection section
3. Count: tasks planned vs completed
4. Update `obsidian/wiki/hot.md` with today's key events/decisions
5. Flag any new captures for tomorrow's processing
