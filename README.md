# Frostpunk — Hintforge Companion

![Frostpunk companion status — coverage, how current it is, and spoiler control](assets/readme-status-card.svg)

A spoiler-controlled hint companion for **Frostpunk**, 11 bit studios' frostbitten survival city-builder where you keep the last city on Earth alive around a coal generator — and decide what a society will do to survive. Built in the [Hintforge](https://github.com/hintforge/builder) format: a loyal sidekick that answers only from these guide files — never from guesswork — at the spoiler level you set.

## Use it

You need a Hintforge reader running in Claude Code, Codex, or OpenClaw. Point it at this repo:

> Load the Frostpunk guide from github.com/hintforge/frostpunk

Then just ask — *"how do I keep heat up," "which law should I pass," "how does this scenario end."* Runtime setup lives in [`hintforge/reader`](https://github.com/hintforge/reader).

## Spoilers

**You** set two independent dials — enemy/threat warnings (Tier 0–5) and puzzle/decision warnings (Tier 0–3) — both **silent by default**; the guide volunteers nothing pre-emptively until you raise one. Late laws and scenario turns are spoiler-tiered, so they stay hidden until your dial allows. There's no save-state reader, so every answer comes from this guide's files.

## What's inside

A structured Markdown corpus — core systems (heat, economy, the Book of Laws), every scenario, the law paths, endings, and all achievements. Interactive tools (a generator-ring city planner is the obvious fit) aren't built yet. The companion reads and writes only the files you control.
