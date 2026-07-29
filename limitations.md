# The Stanley Parable -- Limitations & Blocked Sources

Sources I found that look useful but couldn't fully fetch -- paywalls, Cloudflare, age gates, video-only content, etc. URLs preserved so the player (or another contributor) can open them in a real browser.

## How to read this file
- Each entry: topic, URL, block type, what I could glean, best alternative I did get to.
- Each per-topic file (in `endings/`, `paths/`, `items/`, `sections/`) also lists its own blocked sources at the bottom -- the player rarely needs to come hunting here.
- This file is the catch-all for sources that didn't fit a specific topic.

## Block types
- **paywall** -- content gated behind a subscription or article limit
- **cloudflare** -- Cloudflare bot challenge / 403 / 503 from WebFetch
- **video-only** -- YouTube or other video where the answer is shown visually; no readable text equivalent
- **age-gate** -- content blocked behind age verification
- **cookie-wall** -- popup or consent flow that broke the fetch
- **search-snippet-only** -- search engine returned a snippet but the page itself wasn't reachable
- **dead-link** -- URL was in another source but no longer resolves

## Entries

### Steam achievement completion percentages -- achievements
- Source: https://steamcommunity.com/stats/1703340/achievements
- Block type: cloudflare (Stage 0 did not attempt direct fetch; rung 3 mirror used instead)
- Why I think it has the answer: Global completion % for all 11 achievements
- What I could glean before the block: Achievement names confirmed via vgtimes.com mirror
- Best alternative I did get to: vgtimes.com (rung 3) -- names confirmed, % not surfaced

### Per-achievement Steam "hidden" flag -- achievements (P1)
- Source: SteamDB raw achievement API for AppID 1703340
- Block type: search-snippet-only (raw per-achievement boolean could not be fetched)
- Resolution: P1 inferred **all 11 achievements are non-hidden** because every one displays a full name + description with no "Hidden Achievement" placeholder across the Steam global-stats page and every third-party tracker. Treated as a well-supported inference, not a raw-flag confirmation. Confidence: medium. See `achievements.md`.

### Accessible-ending count discrepancy -- endings (P1)
- The Fandom wiki's **45** (46 franchise minus the console-only Serious Ending) is canonical and matches the brief.
- Some non-English guides count **41 or 43** by tallying bucket-variants and the Epilogue differently (e.g. showgamer.com, ru). [Contradicted across sources] -- the 45 figure is best-sourced and adopted corpus-wide.

### Per-ending point values for the New Content threshold -- paths/new_content.md (P2)
- Source: https://thestanleyparable.fandom.com/wiki/Have_you_played_The_Stanley_Parable_before%3F
- Block type: cloudflare (automated fetch returned 403 during P2 research)
- Why I think it has the answer: This Fandom article is the specific page that documents exactly how many ending-points each ending grants, explaining how quickly a player accumulates toward the 6 or 15 point threshold
- What I could glean before the block: The 6/15 thresholds themselves are confirmed from the New Content Ending and Paywall Ending articles. The per-ending point values are not in those articles.
- Best alternative: The 6 vs. 15 threshold is firmly established; the per-ending breakdown is the unresolved gap. A player who wants to minimize runs before the New Content door appears should open this Fandom page directly in a browser.

### speedrun.com leaderboard WR -- paths/speedrun.md (P2)
- Source: https://www.speedrun.com/tspud (Freedom IL, Glitchless category)
- Block type: cloudflare (automated fetch blocked during P2 research)
- What I could glean: Confirmed mid-pack time ToranPetto 4m 29s 317ms (ranked 7th). Actual #1 WR not fetched. Known to be faster than 4:22.
- Recommendation: open the leaderboard directly in a browser for current verified leader.

## Always-blocked categories

- **"Commitment" achievement trigger:** Playing for a full UTC Tuesday is a real-world time constraint -- not directly observable via automated fetch. P1 resolved the mechanism via community datamining (per-frame UTC-Tuesday check, 24 cumulative hours, counts while paused). Behavior was buggy at launch and may vary by patch/platform -- confidence medium. See `achievements.md`.
- **"Super Go Outside" achievement trigger:** Not playing for ten years is a real-world time constraint -- unresearchable by direct observation. P1 resolved the trigger (10 years; clock-spoofable) via community reports.
- **Pause/Menu key and auto-walk default key:** P1 could not directly quote a source confirming **Esc** as pause or any default **auto-walk** key (auto-walk became a 1.07 toggle). Both are standard-default inferences flagged at medium/low confidence in `controls.md`.
