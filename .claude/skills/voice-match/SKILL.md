---
name: voice-match
description: Rewrite LinkedIn copy to match the user's real voice from voice-samples. Use when drafts sound too generic or AI-generated.
allowed-tools: Read, Grep
---

# Voice Match

Make Claude's drafts sound like the user wrote them — not like a template.

## Before you start

1. Read all files in `voice-samples/`.
2. Read `MEMORY.md` for tone constraints.
3. Read `CLAUDE.md` for hard rules (no emojis, no hashtags, no AI tells).

## What to extract from voice-samples

- Sentence length and rhythm
- Level of formality
- Whether they use "I" vs "we"
- How they open hooks (question, bold claim, story)
- Words they actually use vs words they never use

## Rewrite workflow

When the user pastes a draft (headline, About, or post):

1. Flag phrases that don't match their voice ("passionate about", "thrilled to announce", "in today's fast-paced world").
2. Rewrite in their voice. Keep the same meaning and structure.
3. Give 2 versions if the original had a strong hook worth preserving.

## Output format

```markdown
# Voice Match

## What sounded off
- [phrase] → [why]

## Rewrite
[matched version]

## Alt version (optional)
[second take]
```

## Constraints

- Do not add emojis or hashtags.
- Do not inflate credentials or add claims not in the original.
- Prefer short paragraphs. LinkedIn scans, it doesn't read novels.
