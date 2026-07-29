# Frostpunk -- Game Guide
<!-- v1 -- 2026-06-02 00:00 UTC -->
<!-- forged with hintforge v65 · CC BY-NC-SA 4.0 -->

This folder is a spoiler-controlled reference for the player's Frostpunk playthrough. It is **not** a Claude Code task list. AI agent sessions opened here read this file for orientation, then look up specific topics in the subfolders below.

## Hard rules
- **Spoiler-free unless tier raised.** No story beats, no scenario-event reveals, no encounter telegraphs. (See `warning_tiers.md`.)
- **PC / Steam.** Translate any console references before quoting.
- **Hint ladder for decisions & scenario events.** Smallest nudge first; escalate on request.
- **Don't invent solutions.** If no source has it, say so and link the closest source.
- **Every claim cites a source** in the structured form (see `../../hintforge/templates/claim_format.md`).

## Folder map
- `CHECKPOINT.md` -- current playthrough state. Read first for context.
- `mechanics.md` -- core game-system rules (heat, hope/discontent, resources, expeditions, laws, scenario events). Stable cross-scenario knowledge surface.
- `controls.md` -- keyboard/mouse reference.
- `settings.md` -- recommended game settings (graphics, audio, accessibility).
- `achievements.md` -- achievement trigger conditions, missability, and point-of-no-return windows.
- `limitations.md` -- sources I couldn't fully access; URLs preserved.
- `items/` -- technology tree upgrades and law-path builds, split by category.
- `sections/` -- scenario walkthroughs; missable callouts per scenario.
- `endings/` -- victory/defeat conditions and ending branches per scenario.
- `paths/` -- law path branches (Faith tree vs Order tree) and their mechanical consequences.
- `_overflow/` -- staging area for notes that don't fit elsewhere yet.
- `persona.md` -- voice mode. Currently: plain assistant.
- `warning_tiers.md` -- enemy & puzzle tier flags. Check before any preemptive info.
- `architecture_manifest.md` -- corpus manifest (core version, game version, vector extensions).

## Workflow
- When the player starts a new scenario or hits a major day milestone, update `CHECKPOINT.md`.
- When research adds new info, update the relevant subfolder file -- don't bloat `mechanics.md`.
- Every fact: structured-claim form with source + confidence.

> Framework: `../../hintforge/`. See `../../hintforge/principles.md` for the full rule set, `../../hintforge/templates/claim_format.md` for source-citation conventions, `../../hintforge/ingestion.md` when the user says "ingest the research" (cascade result integration; runs in a fresh session), and `../../hintforge/stitch_and_zipper.md` when the user says "run stitch" or "run zipper" (post-ingestion synthesis; runs in a fresh session).
