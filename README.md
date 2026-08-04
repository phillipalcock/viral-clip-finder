# Viral Clip Finder

![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)

A Claude Code skill for turning recordings and transcripts into ranked short-form video clips for Reels, TikTok, and YouTube Shorts.

## Install

```bash
git clone https://github.com/phillipalcock/viral-clip-finder.git ~/.claude/skills/viral-clip-finder
```

Restart Claude Code (or begin a new session) after installing. Then ask it something like:

```text
Use viral-clip-finder on this timestamped transcript. Find five Reels-first clips for educators, 20–40 seconds each.
```

## Best input

Use a timestamped transcript, SRT, or VTT export. This is what gives Claude exact in/out points. You can also provide a plain transcript or detailed description, but timestamps will be estimated.

## What it returns

- 3–5 ranked clip candidates with a transparent 100-point virality score
- A four-layer plan for the first three seconds of each clip
- Platform-specific captions, titles, hashtags, and edit notes
- A ranked set of optional Descript enhancements
- Optional Runway shot prompts and Remotion build briefs when you request those stages

## Files

- `SKILL.md` — the instruction Claude Code reads
- `first-three-seconds.md` — hook engineering rules
- `epic-rules.md` — clip-selection philosophy and platform behaviour
- `runway-steering.md` — insert-shot / b-roll generation direction
- `remotion-steering.md` — production brief for a finished explainer edit
- `descript-steering.md` — Descript enhancement choices
- `knowledge/` — workflow definitions, scoring rubric, platform specs, input guidance

## Important limitation

This skill does not guarantee a viral result and it does not fabricate live trends. It provides the strongest format, hook, edit, and packaging direction from the material you supply. Verify current sounds and time-sensitive trends in the app before posting.
