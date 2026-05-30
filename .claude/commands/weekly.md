---
description: Sunday weekly review. Aggregates 7 days of daily notes, checks project status, measures goal progress, and plans the week ahead.
---

# /weekly

## Process (30-minute structured review)

### Phase 1 — Look Back (10 min)
1. Read all Daily Notes from the past 7 days
2. Aggregate: tasks done, decisions made, new captures, patterns noticed
3. Trigger `goal-aligner` agent to compute alignment scores
4. Surface top wins (3) and top misses (3)

### Phase 2 — Project Status (10 min)
For each active project in `obsidian/Projects/`:
- Read its CLAUDE.md
- Status: On Track / At Risk / Blocked / Done
- Next action required

### Phase 3 — Look Ahead (10 min)
1. Read `obsidian/Goals/Monthly Goals.md`
2. What's the ONE Big Thing for this coming week?
3. Propose 3-5 focus areas for the week
4. Identify anything that should move to Archives/

## Output
Write to `obsidian/Goals/Weekly Review YYYY-MM-DD.md`
