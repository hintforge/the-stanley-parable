# The Stanley Parable -- Architecture Manifest

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P1 + P2 (deep-research handoff, 2026-06-02)

Corpus manifest and structural metadata. This file serves as the manifest because `nav/` is absent (game-type: narrative-no-nav). Cross-zone structural primitives are minimal; the persona reads this file for all structural reasoning about the game's narrative layout.

## Hintforge manifest

```
corpus-core-version: 5
game-version: "latest"
game-version-platform: "PC / Steam"
game-version-as-of: 2026-06-02
vector-extensions: endings, paths
```

## Vector extensions

- `endings/` -- ending files indexed by `endings/index.md`. Primary content surface; documents how to reach each of the **45 accessible endings** (P1-confirmed; grouped into left-door / right-door / pre-two-doors / UD-progression / bucket-variant files), missability, and spoiler tier.
- `paths/` -- branching decision tree files. Documents which choices at which branch points lead to which endings. Companion to `endings/`.

## Zone Graph

**Game-type label:** narrative-no-nav
**Localization-mechanism class:** none
**Entry node:** stanley_office
**Hub nodes:** office_corridor
**Source-language set:** English (dev: Galactic Cafe / Crows Crows Crows, US/UK/AU); top player regions: English, German, Russian, French

**Note:** The Stanley Parable does not have a traditional zone graph. The "zones" below are the primary narrative spaces the player inhabits. The game's meaningful structure is a **decision tree** (see `paths/decision_tree.md` for the full Point-of-Divergence list and the complete named-spaces inventory), not a spatial map. P1 confirmed the structure below; the authoritative routing detail lives in `paths/`.

**Nodes (P1-confirmed; full room list in `paths/decision_tree.md`):**
- `stanley_office` -- Stanley's starting cubicle (Room 427) and surrounding office floor
- `office_corridor` -- the main corridor where narrative branching begins; contains the Two Doors Room and (in Ultra Deluxe) the New Content door (Door 416, once unlocked)
- `boss_office` -- up the stairwell; keypad (2845 / 8888); fireplace passage to the facility
- `mind_control_facility` -- reached via the Boss's Office fireplace elevator; 3 button platforms, Monitor Room, Facility Power room (ON/OFF)
- `warehouse` -- right-door space (cargo lift, vent, planks) → Phone Room / Colored Doors
- `new_content_area` -- Ultra Deluxe exclusive: New Content ride, Memory Zone, TSP2 Expo Hall, Epilogue Wasteland

**Edges (P1-confirmed):**

| From | To | Type | Direction | Condition | Point of no return | Notes |
|---|---|---|---|---|---|---|
| stanley_office | office_corridor | story-gate | one-way src→tgt | Game start | none | Stanley leaves his office at start of each run |
| office_corridor | mind_control_facility | hub-spoke | bidirectional | Follow Narrator through main path | none | Returning to corridor possible in some paths |
| office_corridor | new_content_area | conditional | one-way src→tgt | Ultra Deluxe only; enter New Content door | none | Available before the Two Doors room |

**Point-of-no-return notes:** Most narrative paths in The Stanley Parable are run-scoped -- once you commit to an ending branch, you complete it and restart. There are no cross-run points of no return for the base game. Ultra Deluxe introduces mild cross-playthrough state (title screen changes); P1 research should document any achievement or collectible access windows that close across runs.

## Chapter ↔ Zone Mapping

Not applicable in the traditional sense. "Chapters" are narrative paths to specific endings. See `paths/` for the decision tree and `endings/` for individual ending documentation.

## Optional Content

| Name | Unlock condition | Access window | Parent zone | Failure mode |
|---|---|---|---|---|
| New Content path (Ultra Deluxe) | Earn 6 ending-points ("yes, played before") or 15 ("no"); Door 416 becomes "New Content" | From ~3rd run (yes) / ~4th run (no) | office_corridor | always-available |
| 6 Stanley figurines | Complete the Sequel Ending | Any run after Sequel; requires multiple resets | various (see `items/collectibles.md`) | always-available (re-collectible) |
| Reassurance Bucket | Complete the Sequel Ending | Spawns in 2nd office room each run | second office area | always-available |
| Epilogue (Ultra Deluxe) | Figurines Ending + reboot/Settings Person ~5× | Appears on main menu | title screen | always-available once unlocked |
| Settings World Champion room + bumpscosity | Earn the Settings World Champion achievement | Permanent after unlock | TSP2 Expo | always-available |

## Support Topology

### Save system
No save system. Each run starts fresh from Room 427 (or a semi-random alternate spawn). Nothing is preserved within a single run. **Cross-playthrough state that PERSISTS:** ending-points count (→ New Content threshold 6/15), Heaven 5-computer sequence progress, figurine count, Settings-Person reboot/survey count (→ Epilogue), Cheese Trigger checkbox, and post-Sequel permanent bucket/figurines/jumps. Datamined persistence flags: `Stanley_Parable_2`, `TSP3_Sequel_Count`, `TSP3_LetsDoIt`. The Cheese Trigger persists even after quitting to the main menu; it only clears on full game exit or replaying the Elevator Ending with the checkbox unchecked.

_source: P2 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_
[Confirmed: Fandom UD wiki (EN), PSNProfiles (EN), tcrf.net datamining]

### Fast-travel network
None. The player returns to start only via auto-loop or manual quit-to-menu → "Begin the game again" (ESC). After the Epilogue/Sequel, the Executive Bathroom and New Content door serve as in-world replay hubs for progression endings.

### Per-ending reset behavior (P2-confirmed full table)

_source: P2 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_
[Confirmed: Fandom (EN) + PSNProfiles (EN) + gamepressure (EN) + spieleboom (DE) per branch grouping]

| Ending | Auto-loop? | Loop destination | Manual quit needed? | Notes |
|---|---|---|---|---|
| Freedom | Yes | Stanley's office (427) | No | Cutscene then reset |
| Countdown | Yes | 427 | No | Dialogue changes on repeat |
| Museum | No | n/a | Yes (interact with ON/OFF switch) | Free exploration first |
| Dream / Mariella | Yes | 427 | No | — |
| Escape Pod (no bucket) | No | n/a | Yes | Narrator gone; restart manually |
| Escape Pod (bucket) | Yes | 427 | No | Pod launches; auto-loops |
| Heaven | No | n/a | Yes | Push buttons until you manually restart |
| Broom Closet | No | n/a | No (not a forced reset) | Gag; continue onward afterward |
| Press Conference | Yes | 427 | No | — |
| Bottom of Mind Control Room | No | n/a | Yes | — |
| Confusion | Yes | 427 | No | Multiple scripted resets during ending |
| Powerful | Yes | 427 | No | — |
| Cold Feet | Yes | 427 | No | — |
| Tape Recorder | No | n/a | Yes | Voice loops indefinitely |
| Apartment | Yes | 427 | No | — |
| Incorrect / Not Stanley | Yes | 427 | No | Credits roll then reset |
| Zending | Yes | 427 | No | After 4 staircase falls |
| Games / Playtest | Yes | 427 | No | Softlock risk if entering door as leaderboard appears (patched 1.05) |
| Art | Yes | 427 | No | After ~4 hours |
| No Buckets | Yes | 427 | No | — |
| Coward / Reluctance | Yes | 427 | No | — |
| Out of Map / Window | No | n/a | Yes | YES/NO choice then manual restart |
| Whiteboard | No | n/a | No (not a forced reset) | Can proceed onward to other endings |
| New Content | Yes | Memory Zone | No | — |
| Skip Button | Yes | 427 | No | — |
| Sequel | Yes | 427 (with new mechanics added) | No | — |
| Infinite Hole | Yes | Expo entrance | No | The ONLY ending that does not return to Room 427 |
| Figurines | Yes | 427 | No | Triggers "REBOOT THE GAME ENTIRELY" whiteboard |
| Epilogue | Yes | 427 | No | Reached from main menu; Free Achievement lever becomes functional after |

## Locks and Keys

P1 + P2 confirmed gate structure. No item keys exist; all "keys" are narrative choices or cross-playthrough state.

_source: P2 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_
[Confirmed: Fandom (EN) + gamepressure (EN) + PSNProfiles (EN) + xboxachievements (EN)]

| Lock (what's gated) | Key (what unlocks it) | Key source | Visible before key? | Notes |
|---|---|---|---|---|
| Freedom / Countdown / Museum / Press Conference / Bottom of MCR / Escape Pod / Heaven / Dream | Left door at the Two Doors Room | Narrative choice | Yes (both doors visible) | Right door loops back via Maintenance Room |
| Freedom vs. Countdown | Final button: **OFF** vs. **ON** in the Power Room | Narrative choice | Yes (both buttons visible) | — |
| Museum corridor | ESCAPE sign + take LEFT at the facility | Appears after ≥1 reset | ESCAPE sign: not on first run | — |
| Escape Pod | Back out of Boss's Office before doors close (0.5s; 3.5s with Low Dexterity Mode) | Timing window at gate | No | Narrator disappears; Door 428 opens |
| Heaven | Click 5 "Awaiting Input" PCs in fixed order across 5 resets | Cross-run sequence | PCs visible; sequence not | One per reset, fixed order |
| Boss's Office fireplace passage | Keypad code **2845** | Narrator dialogue (always 2845) | Keypad visible; code spoken | Early entry → ~15-sec music penalty unless fireplace already auto-opens |
| *8888888888888888* achievement | Press **8** sixteen times (8888 ×2) at the Boss's Office keypad | Keypad visible | Yes | No timing constraint; can precede 2845 in the same run |
| Confusion / Powerful / Cold Feet / Tape Recorder / Apartment / Incorrect / Zending / Games / Art | Right door at the Two Doors Room | Narrative choice | Yes | Some routes require sub-choices inside the right-door path |
| Zending / Games / Art | Colored Doors Room (red/blue doors) after the Warehouse catwalk | Catwalk path off the cargo lift | Yes | Bucket blocks all three → No Buckets Ending instead |
| Apartment vs. Incorrect | Answer vs. unplug the phone | Phone Room | Yes (phone + outlet both visible) | — |
| New Content door (Door 416) | **6 ending-points** (answered "yes, played before") or **15** ("no") | Cross-playthrough ending count | Door visible; label changes when unlocked | Gates the entire UD progression chain; per-ending point values not fully documented — check Fandom "Have you played…" article |
| Skip Button Ending | Complete New Content → take Memory Zone vent | Follows directly from New Content reset | No | Sequential gate |
| Sequel Ending / bucket / jumps / figurines | Complete Skip Button → enter New New Content door | Follows from Skip Button reset | No | Unlocks bucket, permanent jumps, figurine spawns |
| Figurines Ending | Collect all 6 figurines (post-Sequel) then restart | Figurines appear around office post-Sequel | Figurines visible post-Sequel | Triggers "REBOOT THE GAME ENTIRELY" whiteboard |
| Epilogue (main menu) | New Content + Skip Button + Sequel + Figurines endings + bucket + exhaust Settings Person (~5 full reboots) | Cross-playthrough reboot counter | No | "REBOOT THE GAME ENTIRELY" whiteboard is the cue |
| *Beat the game* achievement | Freedom Ending without holding the Bucket | Freedom route | n/a | Bucket disqualifies |
| *Speed run* achievement | Freedom Ending in under 4:22 (no bucket) | Optimized Freedom route + fireplace prep + short spawn | n/a | Prep: auto-open fireplace + short-spawn reset |
| *Door 430* achievement | Complete the full ~75-click multi-room chain | Narrator-guided chain starting at Door 430 | Door 430 visible | Bugged if New Content replaced Door 416 — use fresh run or Boss's Office round-trip to restore 416 |
| *You can't jump* achievement | Spam Space/jump key in-run while not interacting | In-run; any point before a door/button | n/a | Rebinding Space in Options can break the trigger |
| *Test achievement please ignore* | Agree to the plan in the Epilogue + flip the Free Achievement lever in the Expo | Epilogue completion | No | The deepest achievement gate in the game |
| Cheese Trigger (cart narrator voice → "GrilledCheese") | Check the backstage checkbox during the Press Conference Ending | Press Conference backstage | Checkbox visible backstage | Persists until Elevator Ending replay (checkbox unchecked) or full game exit |
| Serious Ending | `sv_cheats 1` Source console command | Developer console | n/a | NOT possible in UD (Unity engine; console removed) |
