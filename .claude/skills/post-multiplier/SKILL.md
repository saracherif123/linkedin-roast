---
name: post-multiplier
description: Turn one rough idea into multiple LinkedIn post drafts with hook variations. Use when the user has a lesson, story, or POV to share.
allowed-tools: Read, Grep
---

# Post Multiplier

Turn one messy idea into a week of LinkedIn content — not a ghostwriter, a multiplier.

## Before you start

1. Read `MEMORY.md` for audience and content lanes.
2. Read `CLAUDE.md` for formatting rules (no emojis, no hashtags).
3. Read `voice-samples/*.txt` and the user's About section for tone.

## Input

The user provides 3–5 sentences. Messy is fine. Ask for it if missing:

> Here's a rough idea / lesson / story I want to share: [DUMP 3-5 SENTENCES]

## Steps

1. Pull out the single sharpest insight.
2. Draft 3 LinkedIn posts in different formats:
   - **a.** A short personal story (under 120 words)
   - **b.** A contrarian take (one bold claim + 3 reasons)
   - **c.** A how-to (numbered, scannable, no fluff)
3. For each post, give 3 alternative hook lines (line 1 only).

## Constraints

- Hook in line 1. One idea per post.
- Match voice from About section and voice-samples.
- No emojis. No hashtags.
- Stay within the user's 3 content lanes from MEMORY.md.

## Output format

```markdown
# Content Multiplier Output

## Core insight
[one sentence]

## Post A — Personal story
[post]

**Hook alternatives:** 1. ... 2. ... 3. ...

## Post B — Contrarian take
[post]

**Hook alternatives:** 1. ... 2. ... 3. ...

## Post C — How-to
[post]

**Hook alternatives:** 1. ... 2. ... 3. ...
```

Save drafts to `posts-draft/` with a descriptive filename unless the user says otherwise.
