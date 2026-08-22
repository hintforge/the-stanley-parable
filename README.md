# The Stanley Parable — Hintforge Companion

![The Stanley Parable companion status — coverage, how current it is, and spoiler control](assets/readme-status-card.svg)

A spoiler-controlled hint companion for **The Stanley Parable**, the narrative game about choice and an increasingly exasperated Narrator. Built in the [Hintforge](https://github.com/hintforge/builder) format: a loyal sidekick that answers only from these guide files — never from guesswork — at the spoiler level you set.

## Use it

You need a Hintforge reader running in Claude Code, Codex, or OpenClaw. Point it at this repo:

> Load the Stanley Parable guide from github.com/hintforge/the-stanley-parable

Then just ask — *"where does this door go," "how many endings are there," "did I miss a path."* Runtime setup lives in [`hintforge/reader`](https://github.com/hintforge/reader).

## Spoilers

This game is almost *entirely* story, so spoiler control matters more here than anywhere. **You** set two independent dials — enemy warnings (Tier 0–5) and puzzle/hint warnings (Tier 0–3) — both **silent by default**; the guide volunteers nothing until you raise one. It only honors what you set. There's no save-state reader (the game has no save worth reading), so every answer simply comes from this guide's files.

## What's inside

A structured Markdown corpus — every path and ending mapped, plus mechanics and all achievements. It's a short game and the guide covers it end to end. Interactive tools (an endings map is the obvious fit) aren't built yet. The companion reads and writes only the files you control.
