# Dependencies -- The Stanley Parable
<!-- hintforge · stitch pass · last run: 2026-06-03 -->
<!-- Every stitch run re-audits ALL existing edges + adds new ones. The per-edge convergence audit (open each cited source, verify the specific value) applies to every row in this file on every run, not just new candidates. A game patch, DLC, or new ingestion phase can change facts that existing edges cite -- only a full re-audit catches that. See `stitch_and_zipper.md` Phase B "Re-run scope: always full." Inconsistencies (cited source contradicts edge text) land in the `## Corpus inconsistencies` section; the edge row stays in place. -->

## Cross-system edges

| Edge ID | System A | System B | Dependency description | Confidence | Source files |
|---------|----------|----------|------------------------|------------|--------------|
| DEP-001 | Settings (Low Dexterity Mode) | Escape Pod Ending | Low Dexterity Mode widens the Escape Pod back-out window from 0.5s (default) to 3.5s, making it significantly easier to execute this timing-sensitive ending. | high | settings.md, endings/left_door.md, paths/narrator_compliant.md, architecture_manifest.md |
| DEP-002 | Heaven Ending | Cross-playthrough state tracking | The Heaven Ending requires clicking 5 "Awaiting Input" computers in a fixed order (419→423→Secretary's→434→Stanley's) across 5 separate resets; the game's cross-playthrough state system tracks which computer in the sequence is next. | high | endings/left_door.md, paths/decision_tree.md |
| DEP-003 | Press Conference Ending | New Content ride narrator | The Cheese Trigger checkbox, accessible backstage during the Press Conference Ending, changes the New Content cart-ride narrator to "GrilledCheese" for all future runs (persists until the Elevator Ending checkbox is unchecked or the game is fully quit). | high | endings/left_door.md, paths/new_content.md, paths/decision_tree.md, architecture_manifest.md |
| DEP-004 | Reassurance Bucket (post-Sequel) | Beat the game / Speed run achievements | Carrying the Reassurance Bucket during the Freedom Ending disqualifies both Beat the game and Speed run achievements; the Bucket must not be held when pressing the OFF button and stepping outside. | high | items/collectibles.md, achievements.md, endings/left_door.md, paths/speedrun.md, architecture_manifest.md |
| DEP-005 | Reassurance Bucket (post-Sequel) | Colored Doors Room endings | Carrying the Reassurance Bucket into the Colored Doors Room diverts to the No Buckets Ending instead of Zending, Games/Playtest, or Art Ending; the Bucket blocks all three colored-door paths. | high | endings/bucket_variants.md, endings/right_door.md, architecture_manifest.md, paths/narrator_defiant.md |
| DEP-006 | Door 430 click-chain | New Content door (Door 416 replacement) | If the New Content door has replaced Door 416, step 10 of the Door 430 chain is blocked; workaround is to visit the Boss's Office and return (restores Door 416 mid-chain) or complete the chain before accumulating 6/15 ending-points. | high | paths/door_430.md, achievements.md |

## PoNR / lockout edges

None -- all endings are replayable; no cross-run points of no return exist in The Stanley Parable. Run-scoped lockouts (e.g., missing a branch) reset on the next restart.

## Missable / sequencing dependencies

| Edge ID | Action | Window | Consequence | Source files |
|---------|--------|--------|-------------|--------------|
| SEQ-001 | Collect figurine #6 (Executive Washroom) before figurine #5 (catwalk / Red-Blue Doors room) | Within the same run | Figurine #5's path can lock out figurine #6 for that run; #6 is still collectible on the next reset (not permanently missable). | items/collectibles.md, sections/missables.md |
| SEQ-002 | Enter the Boss's Office and input keypad 2845 before the Narrator finishes speaking | ≥3 times across prior runs (prep before the timed run) | Fireplace auto-opens on future entries, eliminating the ~15-second keypad-music wait; required prep for a reliable Speed run achievement attempt. | paths/speedrun.md, endings/left_door.md, achievements.md |
| SEQ-003 | Spam Space (jump key) while climbing onto Desk 434 during the Out of Map Ending | During the desk climb, or anywhere in-run while not interacting with a door or button | Triggers the You can't jump achievement; Out of Map desk is a reliable in-run trigger point (also works during the Games Ending segments). | endings/pre_two_doors.md, achievements.md |
| SEQ-004 | Enter the Two Doors Room during the Door 430 click-chain | Mid-chain, before the final five-click sequence on Door 430 | Resets the Narrator's chain state, requiring the entire click sequence to restart from Door 430 ×5. | paths/door_430.md, achievements.md |

## Stitch run log

| Date | Scope | Edges written | Edges proposed (pending) | Inconsistencies surfaced | Model |
|------|-------|---------------|--------------------------|--------------------------|-------|
| 2026-06-03 | full | 10 | 0 | 0 | claude-sonnet-4-6 |

## Corpus inconsistencies

None surfaced in this run.
