# Endings -- Pre-Two-Doors

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P1 + P2 (2026-06-02)

Endings reachable **before** the Two Doors Room.

_source: P1 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline_
[Confirmed: community-wiki (Fandom) + editorial-en]

| Ending | Path summary | Spoiler | UD-exclusive? | Missable |
|---|---|---|---|---|
| Coward / Reluctance Ending | Close the Office 427 door from inside and wait | none | No | No |
| Out of Map Ending | Climb Desk 434 via the chair, exit the window into the white void; choose **YES** (Narrator sings) / **NO** (monologue) | progression | No | No |
| Whiteboard Ending | In the (semi-random) blue office, open Room 426 → whiteboard; **DOG MODE** checkbox | none | partial (UD replaces console `bark` with a checkbox) | No |
| Serious Ending | **NOT ACCESSIBLE in UD** | n/a | Original only | Unreachable in UD |

## The Serious Ending (not accessible in UD)

The Serious Ending required the 2013 launch option `-console` + `sv_cheats 1`; Ultra Deluxe's Unity engine removed the developer console, so it cannot be reached. The **Serious Room** survives only as an Easter egg inside the Memory Zone. Flag any source treating the Serious Ending as accessible in UD as conflating the 2013 original (AppID 221910) with Ultra Deluxe (AppID 1703340).

_source: P1 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_
[Confirmed: datamining (tcrf.net) + community-wiki]

## Notes
- The **Whiteboard Ending's** DOG MODE checkbox is the UD replacement for the original's console `bark` command -- hence "partial" UD-exclusivity.
- The **blue office** that holds Room 426 is semi-randomized between runs.

---

## Per-ending gate-lists (P2)

_source: P2 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline_
[Confirmed: Fandom (EN) + GameRant (EN) + MasterGuide German Steam (DE)]

### Coward / Reluctance Ending gate sequence
**Branch root:** Room 427 office door — close it from the inside and wait.
**Access note:** Any run; the very first possible ending.
**Estimated run time:** ~1 min.

1. From inside Room 427, **close the office door** and wait. `spoiler: none`
2. The Narrator mocks Stanley's cowardice → auto-loops to Room 427. `spoiler: progression`

**Branch notes:** No distinct bucket dialogue.
_source: P2 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · spoiler: progression_
[Confirmed: Fandom (EN), GameRant (EN), MasterGuide German (DE)]

---

### Out of Map / Window Ending gate sequence
**Branch root:** Desk 434 in the first office room — climb out the window.
**Access note:** Any run.
**Estimated run time:** ~2 min.

1. Leave Room 427; go to the first open-plan room and Desk **434**. `spoiler: none`
2. Use the **chair** to climb onto the desk (there is no jump mechanic in normal gameplay). `spoiler: progression`
3. Move out through the window into the white void. `spoiler: story`
4. The Narrator asks YES/NO: **YES** → he sings a song; **NO** → a meta monologue. `spoiler: story`
5. Manual restart required — this ending does NOT auto-loop. `spoiler: story`

**Branch notes:** Spamming Space (jump key) while on the desk also pops *You can't jump*. With the bucket: the Gambhorra'ta reveal plays.

> **Cross-system dependency** -- see `dependencies.md` SEQ-003: the desk-climbing step of this ending is a reliable in-run trigger point for the You can't jump achievement.
_source: P2 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · spoiler: story_
[Confirmed: Fandom (EN), GameRant (EN), kosgames (EN)]

---

### Whiteboard Ending gate sequence
**Branch root:** Room 426 in the blue-office layout.
**Access note:** Any run when the semi-random spawn produces the blue/alternate layout.
**Estimated run time:** ~1 min.

1. Leave Room 427; open the door to Room **426**. `spoiler: none`
2. Read the whiteboard ("Welcome to the... WHITEBOARD ENDING!!"). `spoiler: progression`
3. Optional: interact with the bottom-right checkbox to enable the dog-bark USE sound for one run (the DOG MODE). `spoiler: progression`

**Branch notes:** This is NOT a forced reset — you can continue forward to another ending after reading the whiteboard. No bucket dialogue change. The blue-office layout with Room 426 is semi-randomized; if the standard layout spawns, this ending is not reachable that run.
_source: P2 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · spoiler: progression_
[Confirmed: Fandom (EN), GameRant (EN)]

---

### Serious Ending — NOT ACCESSIBLE (confirmed by P2)
The Serious Ending required `sv_cheats 1` via the Source engine developer console. Ultra Deluxe uses Unity (released April 27, 2022) and does not expose any console commands. Per the Fandom UD wiki: "the game was written in C# using the Unity game engine" and the Serious Ending is excluded "due to the change in game engine barring the player from using the console commands." The Serious Room survives only as an Easter egg inside the Memory Zone.
_source: P2 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · spoiler: none_
[Confirmed: Fandom Endings (EN), Fandom UD wiki (EN)]
