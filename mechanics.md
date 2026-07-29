# The Stanley Parable -- Mechanics

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P1 (2026-06-02)

Narrative branching is the core mechanic. No combat, no inventory, no progression system. Each playthrough is a short (5-20 min) directed narrative shaped by player compliance or defiance of the Narrator.

## The Narrator mechanic (mechanism, not inventory)

The Narrator is a **reactive, evaluative branching system**, not a passive voice. His dialogue is a pre-authored decision tree keyed to the player's Point-of-Divergence choices: obeying advances the "script" toward the Freedom Ending; disobeying triggers branch-specific lines that either (a) **re-rail** you (the Maintenance Room re-routes a right-door player back onto left-door content) or (b) **break the fourth wall**. His emotional register (sad / angry / obnoxious / happy / confused) is a function of accumulated deviation.

_source: P1 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_
[Confirmed: community-wiki + editorial-en (Wikipedia, PopMatters, academic)]

**Documented exceptions to "you must follow the Narrator":**
- The **Maintenance Room** lets right-door players reach virtually all left-door endings.
- The **Not Stanley / Incorrect Ending** has the Narrator discover that the *player* (not Stanley) is in control.

_source: P1 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

## Branching system

At each decision point (primarily door choices), the path taken determines the ending. The full Point-of-Divergence list and named spaces live in `paths/decision_tree.md`; per-branch routing in the other `paths/` files; ending payoffs in `endings/`.

## Ultra Deluxe additions

**New Content path.** A "New Content" door (Door 416) appears in the corridor once you have earned enough ending-points. It opens the UD progression chain (New Content → Memory Zone → Sequel → Infinite Hole → Figurines → Epilogue). See `paths/new_content.md` and `endings/progression_ud.md`.

**Collectibles.** 6 Stanley figurines + the Reassurance Bucket, both unlocked after the Sequel Ending. See `items/collectibles.md`.

**Prologue / Epilogue.** The Epilogue appears on the main menu after the Figurines Ending + ~5 Settings-Person reboots.

## Cross-playthrough state (UD-exclusive)

Ultra Deluxe tracks several values between runs rather than starting completely fresh -- these persistent flags gate the UD progression chain (New Content door threshold, Heaven Ending computer sequence, Epilogue prerequisites) and Sequel-unlocked collectibles. The authoritative list with datamined variable names lives in `paths/decision_tree.md`.

_source: P1 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_
[Confirmed: datamining (tcrf.net) + community-wiki]

## Playtime structure

- **No save state** -- each run starts fresh from Stanley's office (or the title screen). Reset by automatic loop-back (most endings) or quit-to-title.
- HowLongToBeat: **~2 hours** main objectives; **~10.5 hours** to 100% completion -- excluding the Commitment and Super Go Outside real-time gates, which push a true 1000G run to **~27-30 hours** (Xbox roadmap estimate).
- **Speed run** target: complete the Freedom Ending in under 4:22 (excluding load times). See `paths/speedrun.md`.

_source: P1 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_
[Confirmed: HowLongToBeat + editorial-en roadmaps]

## Spoiler tier note

This file documents mechanic-level rules only. Specific Narrator reactions, ending content, and meta-narrative payoffs live in `endings/`, `paths/`, and `sections/story_notes.md` behind appropriate tier gates.

## Sources
- P1 deep-research handoff (2026-06-02): Fandom wiki, tcrf.net (datamining), Wikipedia/PopMatters (editorial), HowLongToBeat.
