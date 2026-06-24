# linkedin-roast

A Claude workspace for building a LinkedIn brand that actually works — roast your profile, rewrite it with constraints, and multiply one idea into a week of posts.

From the **Hold my Club · LinkedIn x Claude** session.

## Quick start

1. Clone this repo and open it in Claude Code (or Cursor with Claude).
2. Edit `MEMORY.md` with your role, audience, and voice.
3. Paste your live profile into `profile/current.md`.
4. Add 3–5 real messages you wrote to `voice-samples/`.
5. Run the roast:

```bash
/linkedin-roast profile/current.md
```

6. Ship one rewrite to LinkedIn before the week ends.

## Project structure

```
linkedin-roast/
├── .claude/
│   └── skills/
│       ├── linkedin-roast/     # Brutally honest profile review
│       ├── post-multiplier/    # One idea → 3 post formats + hooks
│       └── voice-match/        # Make drafts sound like you
├── MEMORY.md                   # Who you are, audience, voice
├── CLAUDE.md                   # Repo-wide rules (no emojis, no hashtags)
├── voice-samples/              # Real text you wrote — tone reference
├── profile/
│   └── current.md              # Your live profile text
├── posts-draft/                # Work in progress
└── posts-shipped/              # Published posts for reference
```

## Skills

| Skill | Invoke | What it does |
|-------|--------|--------------|
| **linkedin-roast** | `/linkedin-roast` | Scores headline, roasts About, audits Top Skills. Outputs 5 issues + rewrites + 3 hook alternatives. |
| **post-multiplier** | `/post-multiplier` | Turns a rough idea into 3 post formats (story, contrarian, how-to) with 9 hook variations. |
| **voice-match** | `/voice-match` | Rewrites AI-sounding drafts to match your voice-samples. |

## The workflow

```
Profile roast  →  Rewrite with constraints  →  Voice match  →  Ship
       ↑                                              ↓
   MEMORY.md + voice-samples              posts-draft/ → LinkedIn
```

## Session takeaways

1. Fix the profile before you post — the funnel starts above the fold.
2. Pick three content lanes. Stay for 90 days.
3. Comments and DMs compound faster than posts.
4. Roast with Claude. Rewrite with constraints. Multiply with prompts.
5. Productionize the workflow as `SKILL.md` files in `.claude/skills/`.
6. Ship one rewrite this week. Done > perfect.

## Customize

- Fill in `MEMORY.md` with your role, audience, and voice.
- Paste your live profile into `profile/current.md`.
- Add 3–5 real messages to `voice-samples/`.
- Add shipped posts to `posts-shipped/` so skills get better over time.

## License

MIT — use it, fork it, roast yourself first.
