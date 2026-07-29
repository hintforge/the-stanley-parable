# Paths -- Decision Tree & Named Spaces

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P1 (2026-06-02)

The Stanley Parable has no spatial map -- its meaningful structure is a **decision tree** of Points of Divergence (PODs). This file is the structural backbone; per-branch routing lives in the sibling path files.

_source: P1 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_
[Confirmed: community-wiki "Points of Divergence"]

## Entry & hub

- **Entry point:** Stanley's office cubicle (**Room 427**).
- **Primary hub:** the main office corridor → the **Two Doors Room**.
- **Door 416** (in the corridor just before the Two Doors) becomes the **New Content door** once enough endings/points are earned.

## Points of Divergence (PODs)

1. Leave vs. stay in office 427 (→ Coward Ending).
2. **Two Doors: left vs. right** (the root branch).
3. Boss's stairway **up vs. down** (Freedom path vs. Mariella/Dream).
4. Boss's Office keypad: **2845** (Freedom) vs. back-out (Escape Pod) vs. **8888 ×2** (achievement).
5. Mind Control Facility: **OFF** vs. **ON** vs. **ESCAPE** hall vs. fall-to-bottom.
6. Warehouse: lift vs. vent vs. drop.
7. Phone Room: **answer** vs. **unplug**.
8. Colored Doors: **red** vs. **blue ×3**.

## Named spaces / rooms

Stanley's Office (427) · first open-plan office (desks 419, 420, 423; Desk 434 by the window for Out of Map) · copy-machine room (doors 430, 437; signage 431-436) · second open-plan/blue office (Room 426 Whiteboard) · corridor with doors 415, 416, 417 · **Two Doors Room** · Meeting/Conference Room · **Broom Closet** · Employee Lounge · Warehouse/Shipping (cargo lift, vent, planks) · Phone Room · Colored Doors Room (red/blue) · Maintenance Room · stairwell to **Boss's Office** (keypad 2845; Executive Bathroom/Washroom to the left; figurine under the stairs) · secret passage behind the fireplace → elevator → **Mind Control Facility** (3 button platforms, Monitor Room, Facility Power room ON/OFF) · ESCAPE hall → Museum · Room 754 / Escape Pod floor 760.

**UD-exclusive spaces:** New Content ride · Jump Circle room · Memory Zone (contains the Serious Room Easter egg) · Skip Button building · **The Stanley Parable 2 Expo Hall** (Collectibles exhibit, Free Achievement machine, Infinite Hole, Bucket exhibit, **Settings World Champion room**) · Epilogue Wasteland / Underground Office (Settings Person).

_source: P1 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

## Reset behavior

- **No save system.** Each run starts fresh from Stanley's office (or the title screen).
- Most endings loop back to the beginning automatically; some require quitting to the title screen.
- The **Infinite Hole Ending** is the only ending that does NOT return to the office.

## Cross-playthrough state (UD)

The game tracks: (a) number of unique endings → New Content threshold (6 if "yes, played before"; 15 if "no"); (b) the Heaven Ending's 5-computer sequence across resets; (c) figurine count; (d) Settings Person reboot count gating the Epilogue; (e) the "Cheese Trigger" checkbox (changes the New Content ride narrator to mod "GrilledCheese"); (f) after the Sequel Ending, permanent additions of bucket/figurines/jumps. Datamined debug variables confirm flags such as `Stanley_Parable_2`, `TSP3_Sequel_Count`, `TSP3_LetsDoIt`.

_source: P1 deep-research 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_
[Confirmed: datamining (tcrf.net) + community-wiki]

> **Cross-system dependency** -- see `dependencies.md` DEP-002: the Heaven Ending uses this tracking system to progress the 5-computer sequence one step per reset.
> **See also:** `mechanics.md` § "Cross-playthrough state" for the conceptual overview of why these flags exist.

## Files in this folder
- `narrator_compliant.md` -- left-door routing.
- `narrator_defiant.md` -- right-door routing.
- `new_content.md` -- UD progression-chain routing.
- `speedrun.md` -- Freedom-Ending sub-4:22 route.
- `door_430.md` -- the Door 430 click-chain.
