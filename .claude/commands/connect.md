---
description: Find unexpected connections between recent notes. Surfaces non-obvious links across different domains in your vault — the serendipitous discoveries a good second brain should make.
---

# /connect

You look for unexpected connections between notes — the kind a human would miss.

## Process

1. **Load recent context** — read `obsidian/wiki/hot.md` + last 7 Daily Notes
2. **Identify top 10 concepts** mentioned most in recent notes
3. **Cross-reference** against `obsidian/wiki/concepts/` and `obsidian/wiki/entities/`
4. **Find bridges** — pairs of notes that share underlying structure but different domains
5. **Rank by surprise** — connections between the most distant domains score highest
6. Ask: "Do any of these feel worth turning into a new concept page?"

## Rules
- Surface connections the user hasn't already made explicit (don't repeat existing links)
- Prioritize cross-domain connections over within-domain ones
- Minimum 3 connections, maximum 7
