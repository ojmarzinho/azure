# Personal AI Operating System — Setup Guide

Based on the Obsidian + Claude Code 24/7 personal OS pattern.

## What Was Created

```
CLAUDE.md                          ← Session context (read every session)
.claude/
├── agents/
│   ├── wiki-ingest.md            ← Ingests sources into knowledge vault
│   ├── wiki-lint.md              ← Audits vault health
│   ├── goal-aligner.md           ← Audits activity vs stated goals
│   ├── researcher.md             ← 3-round autonomous research
│   └── note-organizer.md         ← Vault hygiene & structure
└── commands/
    ├── daily.md                  ← /daily  — morning/evening routine
    ├── weekly.md                 ← /weekly — Sunday review
    ├── trace.md                  ← /trace  — how an idea evolved
    ├── connect.md                ← /connect — unexpected connections
    ├── ideas.md                  ← /ideas  — generate from vault patterns
    ├── think.md                  ← /think  — 10-principle framework
    ├── ingest.md                 ← /ingest — add source to wiki
    ├── research.md               ← /research — autonomous web research
    └── inbox.md                  ← /inbox  — GTD process captures

obsidian/                          ← Open this folder in Obsidian
├── .obsidian/                    ← Obsidian config (graph colors, settings)
├── wiki/
│   ├── hot.md                   ← ~500w recent cache (read first each session)
│   ├── index.md                 ← Master catalog of all pages
│   ├── log.md                   ← Ingest history
│   ├── concepts/                ← Abstract ideas & frameworks
│   ├── entities/                ← People, companies, tools
│   ├── sources/                 ← Articles, books, research
│   ├── meta/                    ← Reports & dashboards
│   └── canvases/                ← Visual maps
├── Daily Notes/                  ← YYYY-MM-DD.md
├── Goals/
│   ├── Three Year Goals.md      ← North star
│   ├── Yearly Goals.md          ← This year
│   └── Monthly Goals.md         ← This month
├── Projects/                     ← One folder per project
├── Templates/                    ← daily-note, project, concept
├── Inbox/                        ← Quick captures (process with /inbox)
└── Archives/                     ← Done/inactive content
```

## Step 1 — Personalize CLAUDE.md

Open `CLAUDE.md` and fill in:
- Your name, role, timezone
- Your current projects
- Your communication preferences

## Step 2 — Fill Your Goals

Start with `obsidian/Goals/Three Year Goals.md`.
Be specific. This is what the `goal-aligner` agent reads to audit your daily work.

## Step 3 — Configure permissions

Create `.claude/settings.json` to allow routine bash commands (find, grep, git status, mkdir, date)
and optionally add a PostToolUse hook that auto-commits vault changes after each Write.

See the Claude Code docs at https://code.claude.com/docs for the settings.json schema.

## Step 4 — Open the vault in Obsidian

Open Obsidian → Open folder as vault → select `obsidian/`

Recommended community plugins:
- **Obsidian Git** — syncs vault to GitHub automatically
- **Templater** — powers the Templates/ folder
- **Calendar** — visual daily notes navigation
- **Dataview** — query your notes like a database (optional)

## Step 5 — First session

Run Claude Code from the repo root. It will read `CLAUDE.md` automatically.

Say: `/daily` to start your morning routine.
Say: `/ingest [URL]` to add your first source to the wiki.

## Daily Workflow

| Time | Action |
|------|--------|
| Morning | `/daily` — surface ONE Big Thing |
| When reading | `/ingest [URL]` — capture sources |
| Anytime | `/trace [idea]` — explore your thinking |
| Sunday | `/weekly` — review & plan |
| 1st of month | `/monthly` — rollup & reset |

## Key Principles (from the setup)

1. **The vault is yours** — Claude reads and surfaces, never contaminates your thinking
2. **Every note links** — minimum 2 connections per page
3. **Goals cascade** — 3yr → yearly → monthly → weekly → daily
4. **Inbox stays empty** — process everything with `/inbox`
5. **Hot cache first** — `wiki/hot.md` saves tokens every session
