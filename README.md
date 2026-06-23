# linkedin-post-writing

A **Claude Code plugin (skill)** that turns one idea into a publish-ready LinkedIn
post — written in **your own voice**, not a generic "copywriter" voice.

It runs a proven **9-step process** as a collaborative draft (it checks in with you
between steps, you steer), and formats the result aggressively by default so the
post is scannable on the feed.

> This is the **installable skill** version. There is also a public web-app version
> (`linkedin-post-writer`) — that one is a deployed tool, not a plugin. If you want
> to *install and use the process inside Claude Code*, this is the repo.

## Install

```
/plugin marketplace add victor-shulga/linkedin-post-writing
/plugin install linkedin-post-writing@linkedin-post-writing
```

Then just say: **"write a LinkedIn post"**, paste an idea, and follow the steps.

## What it does

```
idea
 └─ 1 post type   expert (authority + lead-gen) vs personal (trust + relatability)
 └─ 2 format      text · text+photo · poll · lead-magnet · infographic · carousel · screenshot
 └─ 3 angle       How-To / How-I / Lessons / Mistakes / Villain / Framework / Story / Case / Bold …
 └─ 4 meat        the one key thought + the problem + what you teach or the insight
 └─ 5 body        the angle drives the framework (structural vs PAS/BAB/AIDA); 2 variants
 └─ 6 summary     a strong ending baked in (internal — not shown)
 └─ 7 trailer     5 hook + re-hook combos to stop the scroll and earn the "…more" tap
 └─ 8 humanize    strip AI tells, tame em dashes, keep your pulse
 └─ 9 layout      one idea per line · "fir-tree" lists (short→long, →) · ragged rhythm
```

## Voice is yours

Before writing, the skill collects **your** context and reuses it for the session:

- **Audience / ICP** — who you write for and what they struggle with.
- **Voice sample** — 1–3 of your own posts; the skill imitates their rhythm and formality.
- **Language** — defaults to the language of your idea/voice sample.
- **Proof bank** — real numbers and lived experience you can cite.

If you keep a personal-context skill (e.g. `about-<you>`) or a de-AI skill, the
process reads and defers to them.

## Structure

```
.claude-plugin/
  plugin.json
  marketplace.json
skills/linkedin-post-writing/
  SKILL.md          # the full 9-step process, rules, and worked example
scripts/validate.sh # structure check (run in CI)
```

## License

MIT — see [LICENSE](LICENSE).
