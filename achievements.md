# The Stanley Parable -- Achievements

**status:** research-integrated
**last_reconciled:** 2026-06-02
**research_run:** P1 + P2 (2026-06-02)
**stub_source:** Steam (AppID 1703340, via vgtimes.com mirror at Stage 0)
**coverage:** 11 stubs / 11 resolved / 0 deferred / 0 unreachable

All 11 Ultra Deluxe achievements, organized by `trigger_type`. **No achievement is missable** -- Xbox/PSN roadmaps state "Missable achievements: No." The only true gates are real-world time (Commitment, Super Go Outside) and a long prerequisite chain (Test achievement please ignore).

**Hidden-flag note:** across the Steam global-stats page and every third-party tracker, all 11 achievements display full names and descriptions with no "Hidden Achievement" placeholders -- a well-supported inference that all are **non-hidden**, but not confirmed against SteamDB's raw API.

_source: P1 deep-research 2026-06-02 · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_
[Single source -- verify · class: forum] (hidden-flag inference only; trigger conditions are high-confidence)

**Global unlock rates (Steam, logged-out):** Get your first 93.8% · You can't jump 84.2% · Beat the game 73.7% · Welcome back! 68.3% · Door 430 44.2% · 8888888888888888 21.3% · Test achievement 18.6% · Settings World Champion 16.7% · Speed run 9.4% · Super Go Outside 4.5% · Commitment 3.1%.

## Genre vocabulary
- **meta** -- fourth-wall / easter-egg / joke achievements that comment on the achievement system itself or on game systems. Pervasive in this game.

---

## Progression

### Get your first achievement
- **trigger:** awarded automatically alongside whatever achievement you earn first (no separate action). Easiest first: spam Space for *You can't jump*.
- **missable:** no · **ponr-window:** n/a · **prereqs:** any other achievement (it IS your first)
- **vector-binding:** achievements.md (self-referential meta) · **hidden:** no · **genre:** meta
- _ach: get_your_first_achievement · trigger_type: progression · spoiler: none · puzzle-tier: 0 · enemy-tier: 0_

### Beat the game
- **trigger:** complete the **Freedom Ending** (left → stairs → Boss's Office → 2845 → elevator → Mind Control Facility → press OFF → step outside). Must **NOT** hold the Bucket. ~6-8 min.
- **missable:** no · **ponr-window:** n/a · **prereqs:** none
- **vector-binding:** `endings/left_door.md` (Freedom Ending) · **hidden:** no
- _ach: beat_the_game · trigger_type: progression · spoiler: progression · puzzle-tier: 1 · enemy-tier: 0_

> **Cross-system dependency** -- see `dependencies.md` DEP-004: the Reassurance Bucket (post-Sequel item) disqualifies this achievement if held during the Freedom Ending.

---

## Mastery

### Speed run
- **trigger:** complete the **Freedom Ending in under 4:22** (excluding load times). Prep: reach the Boss's Office ~3-4× entering 2845 early so the fireplace auto-opens; reset until you spawn in a short corridor.
- **missable:** no · **ponr-window:** n/a · **prereqs:** ~3-4 Boss's Office visits
- **vector-binding:** `paths/speedrun.md` · **hidden:** no
- _ach: speed_run · trigger_type: mastery · spoiler: progression · puzzle-tier: 1 · enemy-tier: 0_

> **Cross-system dependency** -- see `dependencies.md` DEP-004: the Reassurance Bucket disqualifies this achievement if held during the run.
> **Cross-system dependency** -- see `dependencies.md` SEQ-002: the fireplace auto-open requires ≥3 prior Boss's Office visits as cross-run prep.

### Commitment
- **trigger:** accumulate **24 hours of runtime on a Tuesday (UTC)**; cumulative across multiple Tuesdays; counts while paused/idle; does not count while the console sleeps. Datamined per-frame check (PC): *"…get today's date in UTC and see if it's a Tuesday. If true, then for every 60 minutes it adds up the playing minute. Once that adds up to 1440 or more (24 hours), the achievement unlocks. All checks are done every frame."* Does NOT require midnight-to-midnight. Spoof: set the clock to a UTC Tuesday, run the game.
- **missable:** no · **ponr-window:** n/a · **prereqs:** none
- **vector-binding:** achievements.md · **hidden:** no · **genre:** meta
- _ach: commitment · trigger_type: mastery · spoiler: none · puzzle-tier: 0 · enemy-tier: 0 · confidence: medium (timer behavior was buggy at launch; cumulative-UTC-Tuesday is consensus, may vary by patch/platform)_
[Confirmed: datamining + forum -- but patch-variable]

### Super Go Outside
- **trigger:** don't play for **10 years**, then launch and start a new game. Spoof: close the game, set the system clock +10 (or +11) years, relaunch, start. (The 2013 original had "Go Outside" at 5 years; UD doubled it.)
- **missable:** no · **ponr-window:** n/a · **prereqs:** none (patience)
- **vector-binding:** achievements.md · **hidden:** no · **genre:** meta
- _ach: super_go_outside · trigger_type: mastery · spoiler: none · puzzle-tier: 0 · enemy-tier: 0_

---

## Collection

### Settings World Champion
- **trigger:** set **every slider to every value and cycle every option** in Settings (the finite, enumerable set is documented in `settings.md`), **including the hidden Subtitle/Translation opacity sliders**. The set is the completeness target; per-member detail lives in `settings.md`.
- **missable:** no · **ponr-window:** n/a · **prereqs:** none (can be done from the title screen)
- **vector-binding:** `settings.md` (full slider set) · **hidden:** no · **genre:** meta
- **reward:** unlocks the Settings World Champion room + the **bumpscosity** setting.
- _ach: settings_world_champion · trigger_type: collection · spoiler: none · puzzle-tier: 0 · enemy-tier: 0_

---

## Discovery

### Test achievement please ignore
- **trigger:** flip the lever on the **"Free Achievement" machine** in the TSP2 Expo -- but it only works **after completing the Epilogue**. The name is a Source missing-texture / "test post please ignore" joke. Full chain: 2 different endings → New Content door → Memory Zone ending → Sequel (Expo) ending → collect all 6 figurines → Figurines Ending → reboot ~5× + Settings Person → play the Epilogue → return to the Expo → flip the lever (~2-2.5h).
- **missable:** no · **ponr-window:** n/a · **prereqs:** the entire UD progression chain + Epilogue
- **vector-binding:** `endings/progression_ud.md`, `paths/new_content.md` · **hidden:** no · **genre:** meta
- _ach: test_achievement_please_ignore · trigger_type: discovery · spoiler: late-game · puzzle-tier: 2 · enemy-tier: 0_

### Welcome back!
- **trigger:** gain control of Stanley, fully quit the application, relaunch and begin again.
- **missable:** no · **ponr-window:** n/a · **prereqs:** none
- **vector-binding:** `mechanics.md` (playtime structure) · **hidden:** no · **genre:** meta
- _ach: welcome_back · trigger_type: discovery · spoiler: none · puzzle-tier: 0 · enemy-tier: 0_

### You can't jump
- **trigger:** press Space/jump several times where not interacting. Works in-run (NOT on the title screen); works at any point where Stanley is not interacting with a door or button. The Out of Map desk and the Games Ending segments are reliable spots. Press count varies (some players report a handful, others report more — spam freely).
- **Caution:** rebinding Space in Options can break the trigger — use the default binding.
- **missable:** no · **ponr-window:** n/a · **prereqs:** must be in-run (not title screen)
- **vector-binding:** `controls.md` · **hidden:** no · **genre:** meta
- _ach: you_cant_jump · trigger_type: discovery · spoiler: none · puzzle-tier: 0 · enemy-tier: 0_
- _source: P2 deep-research 2026-06-02 · capture: web_fetch · confidence: high_
[Confirmed: xboxachievements (EN), Steam discussions (EN), Steam Hunters (EN)]

> **Cross-system dependency** -- see `dependencies.md` SEQ-003: the Out of Map Ending's Desk 434 climb is a reliable in-run trigger point for this achievement.

### 8888888888888888
- **trigger:** in the Boss's Office, press **8** on the keypad **sixteen times total** (enter "8888" twice — 8 presses per entry, 2 entries = 16 total presses) instead of 2845. Achievement pops when you hear the voice say "eight." No timing constraint — the keypad accepts the 8s at any point; you can grab this before entering 2845 to continue to the Freedom Ending in the same run.
- **missable:** no · **ponr-window:** n/a · **prereqs:** reach the Boss's Office (left-door path)
- **vector-binding:** `paths/narrator_compliant.md`, `endings/left_door.md` · **hidden:** no · **genre:** meta
- _ach: 8888888888888888 · trigger_type: discovery · spoiler: progression · puzzle-tier: 1 · enemy-tier: 0_
- _source: P2 deep-research 2026-06-02 · capture: web_fetch · confidence: high (16 total presses confirmed)_
[Confirmed: xboxachievements (EN), GameFAQs Grawl FAQ (EN), Steam Hunters (EN)]

### Door 430 ("Click on door 430 five times")
- **trigger:** a multi-step **click-chain**, NOT five clicks. Full sequence (P2-confirmed click counts): Door 430 ×5 → ×20 → ×50 (75 total on 430) → Door 417 ×~20 → Door 437 ×a few → Door 415 ×~10 → return to 437 → copy machine ×1 → climb Desk 419 (box → chair → desk) → Door 416 ×a few → copy machine ×1 → Door 430 ×5 → achievement.
- **prereq caveat:** Do NOT enter the Two Doors Room mid-chain. Bug still present: if New Content replaced Door 416, go to the Boss's Office and back to restore the original mid-chain, or do the chain on a fresh run before the New Content door appears.
- **missable:** no · **ponr-window:** n/a
- **vector-binding:** `paths/door_430.md` · **hidden:** no · **genre:** meta
- _ach: door_430 · trigger_type: discovery · spoiler: progression · puzzle-tier: 1 · enemy-tier: 0_
- _source: P2 deep-research 2026-06-02 · capture: web_fetch · confidence: high (click counts corroborated across 2 sources)_
[Confirmed: PSNProfiles (EN), xboxachievements (EN), ScreenRant (EN), Gamepur (EN)]

> **Cross-system dependency** -- see `dependencies.md` DEP-006: the New Content door replacing Door 416 blocks step 10 of this chain.
> **Cross-system dependency** -- see `dependencies.md` SEQ-004: entering the Two Doors Room mid-chain resets all chain progress.

---

## Resolution table

| Achievement | trigger_type | Status | Primary vector home |
|---|---|---|---|
| Get your first achievement | progression | resolved | achievements.md |
| Beat the game | progression | resolved | endings/left_door.md |
| Speed run | mastery | resolved | paths/speedrun.md |
| Commitment | mastery | resolved | achievements.md |
| Super Go Outside | mastery | resolved | achievements.md |
| Settings World Champion | collection | resolved | settings.md |
| Test achievement please ignore | discovery | resolved | endings/progression_ud.md |
| Welcome back! | discovery | resolved | mechanics.md |
| You can't jump | discovery | resolved | controls.md |
| 8888888888888888 | discovery | resolved | paths/narrator_compliant.md |
| Door 430 | discovery | resolved | paths/door_430.md |

*Branch and Threshold sections omitted -- no achievement classifies into them.*

## Efficient 100% routing
1. **Session #1:** spam Space (*You can't jump* → *Get your first achievement*); set all settings sliders/options incl. hidden ones (*Settings World Champion*); fully quit + relaunch (*Welcome back!*).
2. **Freedom runs:** complete the Freedom Ending (*Beat the game*); on a separate run enter 8888 twice (*8888888888888888*); do 3-4 Boss's Office visits entering 2845 early, then the sub-4:22 Freedom run (*Speed run*).
3. **Door 430 chain** on a fresh run **before** the New Content door exists (avoids the 416 bug).
4. **Progression chain** for *Test achievement*: rack up endings → New Content → Sequel → 6 figurines → Figurines Ending → reboot ×5 + Settings Person → Epilogue → flip the Expo lever.
5. **Time-gates last:** *Commitment* (idle 24h across UTC Tuesday(s), or clock-spoof offline); *Super Go Outside* (clock +10y offline, relaunch).

## Sources
- P1 deep-research handoff (2026-06-02): xboxachievements.com & playstationtrophies.org roadmaps, psnprofiles.com, gamerant.com, gamepur.com, gamepressure.com; Fandom wiki (Achievements); tcrf.net (datamining); steamcommunity.com/stats/1703340; Steam community guides (EN/DE/FR/RU).
