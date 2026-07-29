# The Stanley Parable -- Game Guide
<!-- v1 -- 2026-06-02 -->
<!-- forged with hintforge v65 · CC BY-NC-SA 4.0 -->

This folder is a spoiler-controlled, plain-assistant-mode reference for the player's The Stanley Parable playthrough. It is **not** a Claude Code task list. AI agent sessions opened here read this file for orientation, then look up specific topics in the subfolders below.

## Hard rules
- **Spoiler-free unless tier raised.** No story beats, no ending reveals, no decision telegraphs. (See `warning_tiers.md`.)
- **PC mouse+keyboard.** Translate any other-platform references before quoting.
- **Hint ladder for narrative branches & ending discovery.** Smallest nudge first; escalate on request.
- **Don't invent solutions.** If no source has it, say so and link the closest source.
- **Every claim cites a source** in the structured form (see `../../hintforge/templates/claim_format.md`).
- **The game is meta-aware.** The Narrator and game systems actively comment on and subvert player behavior. Treat fourth-wall content as in-scope lore, not an error.

## Folder map
- `CHECKPOINT.md` -- current playthrough state. Read first for context.
- `mechanics.md` -- core game-system rules (branching logic, Narrator interaction, Ultra Deluxe collectibles). Stable cross-playthrough knowledge.
- `limitations.md` -- sources I couldn't fully access; URLs preserved.
- `endings/` -- each ending indexed; how to reach it, missability, notes.
- `paths/` -- the branching decision trees; which choices at which branch points lead where.
- `items/` -- collectibles and in-game objects (minimal for this game -- no weapons/abilities/upgrades).
- `sections/` -- main-path segments; missables-only callouts and story notes.
- `achievements.md` -- all 11 Steam achievements with trigger conditions and missability.
- `architecture_manifest.md` -- corpus manifest (version, platform, vector extensions, structural metadata).
- `persona.md` -- voice: plain assistant mode (no character voice active).
- `warning_tiers.md` -- enemy & puzzle tier flags. Check before any preemptive info.

## Workflow
- When the player starts a new playthrough path, note it in `CHECKPOINT.md`.
- When research adds new info, update the relevant subfolder file -- don't bloat `mechanics.md`.
- Every fact: structured-claim form with source + confidence.

> Framework: `../../hintforge/`. See `../../hintforge/principles.md` for the full rule set, `../../hintforge/templates/claim_format.md` for source-citation conventions, `../../hintforge/ingestion.md` when the user says "ingest the research" (cascade result integration; runs in a fresh session), and `../../hintforge/stitch_and_zipper.md` when the user says "run stitch" or "run zipper" (post-ingestion synthesis; runs in a fresh session).
