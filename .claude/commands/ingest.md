---
description: Add a source (article, book, video, URL, file) to the knowledge vault. Triggers the wiki-ingest agent to extract concepts, entities, and key ideas into interconnected notes.
---

# /ingest [source]

Trigger the `wiki-ingest` agent with the provided source.

## What counts as a source
- A URL (article, blog post, paper, YouTube video)
- A file path (PDF, text file, markdown)
- A block of pasted text (paste after running the command)
- A book title + author (triggers a research-based ingest)

## What happens
1. The `wiki-ingest` agent reads the source
2. Extracts 8-15 concepts, entities, and relationships
3. Creates pages in `obsidian/wiki/`
4. Updates `obsidian/wiki/index.md` and `obsidian/wiki/log.md`
5. Refreshes `obsidian/wiki/hot.md`

## After ingest
- Run `/connect` to find unexpected links with existing notes
- If it's a major source, run `/trace` on the key concept to see if it extends existing thinking
