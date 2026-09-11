# Human

Claude/Antigravity skill that rewrites or drafts text so it doesn't read as AI-generated.

## Modes

- **academic** — essays, papers, lit reviews, research writing
- **post** — Reddit, Twitter/X, forums, LinkedIn, comments
- **normal** — email, Slack/Teams, cover letters, everyday messages

Mode is picked from context (essay → academic, tweet → post, email → normal) or set explicitly.

## What it kills

Stock AI vocabulary (delve, tapestry, leverage, robust, etc.), tricolon lists, em-dash spam, throat-clearing openers, "not only X but also Y," forced both-sidesing, horizon-gazing conclusions, metronomic sentence rhythm. Full breakdown and research basis in `SKILL.md` and `references/`.

## Install

Drop the `human/` folder into your skills directory (e.g. `.agents/skills/human/`).

## Structure

```
human/
├── SKILL.md
└── references/
    ├── academic.md
    ├── online.md
    └── normal.md
```

## License

MIT
