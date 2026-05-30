---
description: Run a 3-round autonomous research loop on any topic. Searches, fetches, synthesizes, and files results into the wiki. Use for deep-dives, competitive intel, or fact-checking.
---

# /research [topic]

Trigger the `researcher` agent on the given topic.

## Rounds
1. **Discovery** — broad search, collect 5-8 sources, write hypothesis
2. **Deep dive** — evaluate sources, extract claims, find contradictions, generate follow-ups
3. **Synthesis** — 500-800 word synthesis with confidence levels

## Output
Filed to `obsidian/wiki/sources/research-[topic]-YYYY-MM-DD.md`
Then triggers `wiki-ingest` to create concept/entity pages from the synthesis.

## After research
- Run `/connect` to find vault connections
- Run `/ideas` with the topic as domain if exploring new territory
