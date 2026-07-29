# Endings -- Left Door (obey the Narrator)

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P1 + P2 (2026-06-02)

Endings reached by taking the **left door** at the Two Doors Room (following the Narrator). Routing detail lives in `paths/narrator_compliant.md`.

_source: P1 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline_
[Confirmed: community-wiki (Fandom) + editorial-en + editorial-non-en, 3 languages]

| Ending | Path summary | Spoiler | Missable |
|---|---|---|---|
| Freedom Ending | Left door → up stairs → Boss's Office → keypad **2845** → elevator down → Mind Control Facility → press **OFF** → step outside | progression (route) | No (replayable) |
| Countdown Ending | As Freedom but press **ON** → nuclear self-destruct countdown | progression | No |
| Bottom of the Mind Control Room Ending | In the Monitor Room, climb chair→desk→over the railing, fall to the bottom | progression | No |
| Museum Ending | At the facility take the **ESCAPE** hall → crush machine → a female Narrator rescues Stanley → Museum of beta/cut content | late-game | No |
| Press Conference Ending | Ride the Boss's secret elevator up/down **3 times** | late-game | No |
| Mariella / Dream Ending | At the Boss's stairway go **DOWN** not up → looping paradox rooms → Stanley passes out, found by Mariella | story | No (content-warning skippable) |
| Escape Pod Ending | Walk into Boss's Office then back out before the doors close (trapping the Narrator) → return, Door 428 now open → room 754 → stairs to escape pod floor 760 | late-game | No |
| Heaven Ending | Click 5 "Awaiting Input" computers in order across separate playthroughs (419 → 423 → Secretary's → 434 → Stanley's), resetting between each | progression | No (cross-playthrough) |
| Broom Closet Ending | Left door, after the Meeting Room enter the Broom Closet and wait | none | No |

## Notes

- **Freedom Ending** is the only ending that counts as "beating the game"; it is required for both the **Beat the game** and **Speed run** achievements. You must NOT be holding the Bucket. _The "real/canonical ending" framing -- that this is what the Narrator's whole script drives toward -- is the game's central thematic payoff._
  _source: P1 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 3 · category: lore · spoiler: story_
- **Escape Pod Ending** back-out window is **0.5s** by default; the **Low Dexterity Mode** accessibility setting widens it to **3.5s**. This near-undocumented detail appears only on the Fandom Options Menu page.
  _source: P1 deep-research 2026-06-02 · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 1 · category: easter-egg · spoiler: progression_
  [Single source -- verify · class: community-wiki]
- The **Bottom of the Mind Control Room Ending** was a 2013 bug, promoted to a proper ending in Ultra Deluxe.
- **8888888888888888** achievement is earned at the Boss's Office keypad on this path (enter 8 eight times instead of 2845). See `achievements.md`.

## Achievement bindings
- Beat the game → Freedom Ending. Speed run → Freedom Ending <4:22 (`paths/speedrun.md`). 8888888888888888 → Boss's Office keypad.

---

## Per-ending gate-lists (P2)

_source: P2 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline_
[Confirmed: Fandom Endings wiki (EN) + GameRant (EN) + gamepressure (EN) + okaygotcha (EN) + spieleboom Linke Tür (DE)]

### Freedom Ending gate sequence
**Branch root:** Two Doors Room → LEFT door. The canonical "real" ending required for *Beat the game* and *Speed run*.
**Access note:** Any run; the first playthrough.
**Estimated run time:** 8–10 min normal; under 4:22 speedrun-optimized.

1. Leave Room 427 — exit Stanley's office. `spoiler: none · puzzle-tier: 0`
2. Walk through the two open-plan office rooms to the Two Doors Room. `spoiler: none · puzzle-tier: 0`
3. Take the **LEFT** door. `spoiler: none · puzzle-tier: 0`
4. Walk through the Meeting Room; continue down the corridor to the stairwell. `spoiler: progression · puzzle-tier: 0`
5. Stairwell — climb **UP** (going DOWN leads to the Dream/Mariella Ending). `spoiler: progression · puzzle-tier: 1`
6. Enter the Boss's Office past the secretary's desk. `spoiler: progression · puzzle-tier: 0`
7. Keypad behind the desk — enter **2845**. Wait for the Narrator to finish to avoid a ~15-sec music penalty; skip the wait if the fireplace auto-opens (after ≥3 prior Boss's Office visits entering 2845 early). `spoiler: progression · puzzle-tier: 1`
8. Fireplace opens — walk through and press **DOWN** in the elevator. `spoiler: progression · puzzle-tier: 0`
9. Mind Control Facility — press the lightbulb button then the camera button to light the monitors; ride platforms/elevator UP. `spoiler: progression · puzzle-tier: 0`
10. Facility Power Room — press **OFF**. `spoiler: story · puzzle-tier: 1`
11. Step out the opened door into the green field — Freedom Ending cutscene plays; auto-loops to Room 427. `spoiler: story · puzzle-tier: 0`

**Common confusions:** Stairwell DOWN → Dream Ending; Power Room ON → Countdown Ending; holding the Bucket → bucket variant in the Power Room (disqualifies *Beat the game* / *Speed run*).
**Achievement window:** *8888888888888888* can be grabbed at gate 7 in the same run — press 8 sixteen times before entering 2845 (no timing constraint; Narrator accepts the 8s at any point).
_ach: beat_the_game, speed_run · achievement-hidden: no, no · trigger_type: progression, mastery · spoiler: progression_

> **Cross-system dependency** -- see `dependencies.md` DEP-004: the Reassurance Bucket (post-Sequel) disqualifies both Beat the game and Speed run if held here.
> **Cross-system dependency** -- see `dependencies.md` SEQ-002: gate 7 fireplace skip requires ≥3 prior Boss's Office visits (cross-run prep); critical for Speed run.

---

### Countdown Ending gate sequence
**Branch root:** Same as Freedom through gate 9.
**Access note:** Any run.
**Estimated run time:** ~9 min.

1–9. Identical to Freedom gates 1–9.
10. Facility Power Room — press **ON** instead of OFF. `spoiler: story`
11. Nuclear self-destruct countdown; explosion → auto-loops to Room 427. `spoiler: story`

**Branch notes:** Repeating this ending slightly changes Narrator dialogue (one of few tracked endings). With the bucket, a "Silly Birds" surveillance variant plays.
_source: P2 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · spoiler: story_
[Confirmed: Fandom (EN), GameRant (EN), spieleboom (DE)]

---

### Museum Ending gate sequence
**Branch root:** Freedom gates 1–8 (through the fireplace elevator), then the ESCAPE corridor.
**Access note:** The red ESCAPE sign appears only after at least one reset; not visible on the very first run.
**Estimated run time:** ~6 min + free exploration time.

1–8. Identical to Freedom gates 1–8 (reach the bottom of the fireplace elevator).
9. Before entering the Mind Control Facility, turn **LEFT** at the red **ESCAPE** sign. `spoiler: progression`
10. Walk the narrow corridor; jump into the vent at the end. `spoiler: progression`
11. Saved by the Female Narrator (the Curator) and dropped into the Museum of beta/cut content. `spoiler: story`
12. Explore exhibits; find the ON/OFF switch room and interact with it to trigger the ending. Manual restart then required. `spoiler: story`

**Branch notes:** Does not auto-loop — requires manual switch interaction then manual quit. With the bucket, the Curator's rescue focuses on the bucket (Bucket Museum variant).
_source: P2 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · spoiler: story_
[Confirmed: Fandom (EN), okaygotcha (EN), spieleboom (DE)]

---

### Dream / Mariella Ending gate sequence
**Branch root:** Stairwell — go DOWN.
**Access note:** Any run.
**Estimated run time:** ~6 min.

1–4. Freedom gates 1–4 (reach the stairwell).
5. Stairwell — go **DOWN** instead of up. `spoiler: progression`
6. Walk the paradoxically looping rooms; Stanley goes mad and passes out. `spoiler: story`
7. Mariella finds Stanley; monologue → auto-loops to Room 427. `spoiler: story`

**Branch notes:** Content-warning skippable (completing it still counts toward New Content threshold). With the bucket, the madness is attributed to carrying "an everyday bucket" (Mariella bucket variant).
_source: P2 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · spoiler: story_
[Confirmed: Fandom (EN), kosgames (EN), spieleboom (DE)]

---

### Escape Pod Ending gate sequence
**Branch root:** Boss's Office — back out immediately as the double doors close.
**Access note:** Any run.
**Estimated run time:** ~5 min.

1–5. Freedom gates 1–5 (top of the stairwell).
6. Step INTO the Boss's Office then immediately **back out** before the double doors close. Doors lock; Narrator falls silent. Back-out window: **0.5s** default (or **3.5s** with Low Dexterity Mode in settings). `spoiler: progression`
7. Backtrack all the way to Room 427; Door 428 is now open. `spoiler: progression`
8. Enter Door 428 → teleported to Room 754; climb the stairs toward Floor 760. `spoiler: story`
9. (No bucket) Escape Pod at Floor 760 is non-functional — manual restart. (With bucket) place the bucket inside the pod to launch it → Bucket Escape Pod variant. `spoiler: story`

**Branch notes:** Bucket Escape Pod removes the podium bucket for the next two restarts (replacement bucket appears). Manual restart needed for the non-bucket version.
_source: P2 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · spoiler: story_
[Confirmed: Fandom (EN), GameRant (EN), nintendosmash (EN)]

> **Cross-system dependency** -- see `dependencies.md` DEP-001: enabling Low Dexterity Mode in Settings widens the back-out window from 0.5s to 3.5s, making this ending significantly easier to trigger.

---

### Heaven Ending gate sequence
**Branch root:** Click 5 "Awaiting Input" computers in order across separate resets.
**Access note:** Multi-run; one PC per reset in a fixed order.
**Estimated run time:** 5 short runs.

Run 1: Click Employee **419**'s computer (2nd desk room, "Awaiting Input"). `spoiler: progression`
Run 2: Click Employee **423**'s computer (same room, opposite corner). `spoiler: progression`
Run 3: Click the **Secretary's** computer (desk outside the Boss's Office). `spoiler: progression`
Run 4: Click Employee **434**'s computer (first office room). `spoiler: progression`
Run 5: Click **Stanley's own** computer in Room 427 → transported to Heaven. `spoiler: story`
Then: push buttons in Heaven until you choose to restart — manual quit needed. `spoiler: story`

**Branch notes:** Order is fixed; the next "Awaiting Input" PC only activates after the previous reset. With the bucket on run 5: Bucket Heaven/Hell variant.
_source: P2 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · spoiler: story_
[Confirmed: Fandom (EN), Arburo Steam guide (EN), spieleboom (DE)]

> **Cross-system dependency** -- see `dependencies.md` DEP-002: the game's cross-playthrough state tracking system records which computer in this sequence is next across separate runs.

---

### Broom Closet Ending gate sequence (gag)
**Branch root:** LEFT door → enter the Broom Closet after the Meeting Room.
**Access note:** Any run.
**Estimated run time:** ~5 min (requires waiting).

1–3. Freedom gates 1–3 (LEFT door, through the Meeting Room).
4. After the Meeting Room, enter the **Broom Closet** on the right. `spoiler: none`
5. Remain inside; the Narrator grows frustrated and then asks to take Stanley's place. `spoiler: progression`
6. Exit, then re-enter the closet; leave once the Narrator finishes. `spoiler: progression`

**Branch notes:** A gag/non-forced-reset — you can continue to other endings afterward. Does not auto-loop. No distinct bucket dialogue.
_source: P2 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · spoiler: progression_
[Confirmed: Fandom (EN), MasterGuide German Steam (DE)]

---

### Press Conference Ending gate sequence
**Branch root:** Boss's secret fireplace elevator — ride up/down 3 times total.
**Access note:** Any run after the keypad opens.
**Estimated run time:** ~6 min.

1–8. Freedom gates 1–8 (reach the bottom of the elevator).
9. Ride the elevator DOWN, then back UP to the Boss's Office; repeat once more. `spoiler: progression`
10. On the third ride up, the Narrator takes Stanley to a Press Conference. `spoiler: story`
11. Press Conference sequence → auto-loops to Room 427. `spoiler: story`

**Branch notes:** The **Cheese Trigger** checkbox is accessible backstage during this ending — checking it changes the New Content cart-ride narrator voice to "GrilledCheese" for future runs (persists until the Elevator Ending is replayed unchecked or game is fully quit).
_source: P2 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · spoiler: story_
[Confirmed: Fandom (EN), New Content Ending wiki (EN)]

> **Cross-system dependency** -- see `dependencies.md` DEP-003: the Cheese Trigger set here modifies the New Content cart-ride narrator voice in paths/new_content.md.

---

### Bottom of the Mind Control Room Ending gate sequence
**Branch root:** Monitor Room — fall to the bottom.
**Access note:** Any run reaching the Mind Control Facility.
**Estimated run time:** ~7 min.

1–9. Freedom gates 1–9 (into the Monitor Room, reaching the first button platform).
10. Climb onto the chair, then the desk, then over the railing — **fall to the bottom** of the Monitor Room. `spoiler: progression`
11. Narrator explains this was a bug promoted to an ending; jingle plays → manual restart. `spoiler: story`

**Branch notes:** Originally a glitch in the 2013 game; officially made a real ending in Ultra Deluxe. Manual restart required. With the bucket: Stanley and the bucket live in the pit together.
_source: P2 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · spoiler: story_
[Confirmed: Fandom (EN), spieleboom (DE), Arburo Steam guide (EN)]
