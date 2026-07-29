# Frostpunk -- Limitations & Blocked Sources

Sources I found that look useful but couldn't fully fetch -- paywalls, Cloudflare, age gates, video-only content, etc. URLs preserved so the player (or another contributor) can open them in a real browser.

## How to read this file
- Each entry: topic, URL, block type, what I could glean, best alternative I did get to.
- Each per-topic file (in `items/`, `sections/`, `paths/`, `endings/`) also lists its own blocked sources at the bottom -- the player rarely needs to come hunting here.
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

### Steam Community achievements page -- achievement list
- Source: https://steamcommunity.com/stats/323190/achievements
- Block type: cloudflare (probable -- not directly fetched during Stage 0)
- Why I think it has the answer: canonical Steam achievement list with global unlock percentages
- What I could glean before the block: achievement names confirmed via vgtimes.com mirror
- Best alternative I did get to: https://vgtimes.com/games/frostpunk/achievements-and-trophies/ (rung 3 of achievement source ladder)

### Achievement triggers not captured at P1 -- base game
- **RESOLVED by P3 (2026-06-03).** All 25 gaps closed via Deep Research P3 handoff (fandom Achievements + TrueAchievements + Steam guides). "Central Heating" was already resolved at P1; "Builder" is TLA DLC scope. All triggers now in `achievements.md`.

### Achievement base-vs-DLC scope unconfirmed (rows 101-110, 114)
- **RESOLVED by P3 (2026-06-03).** All 11 confirmed as On The Edge DLC: Guardian, First Steps, Contractor, Frostland Explorer, I Feel Lucky, All Your Base Are Connect To Us, Social Activist, Slave Driver, Unforgiven, We Are In This Together (all OTE); I See Friends Holding Hands (Endless mode, OTE Settlements enabled). Triggers now in `achievements.md`.

### Technology-tree research costs -- partially resolved (P3 2026-06-03)
- Source: readonly.wiki (NamuWiki mirror, Korean) + English sources (game-vault, fandom-archive, Steam thread)
- **Most costs resolved at P3.** Tier-based schedule confirmed: T1=20W/10S, T2=30W/20S, T3=40W/25S, T4=50W/30S, T5=120W/80S; exceptions noted.
- **Remaining single-source entries** (threshold: a second English source printing "research cost" for the node, or datamined game file): Heater Efficiency Upgrade (60W/40S -- contradicts prior hypothesis; priority), Large Resource Depot, Charcoal Kiln, Steam/Advanced Sawmill line, Steam/Advanced Wall Drill line, Steam/Advanced Steelworks (build-cost conflation risk high), Automatic Prototyping (150W/100S), Infirmary, Infirmary Mechanisation, Bunkhouse, House, Hunters' Gear.
- ⚠️ **Build-cost conflation remains the #1 hazard.** Fandom pages for Steam Steelworks, Advanced Steelworks, Bunkhouse, House, Advanced Wall Drill print build costs only. Corpus now notes each conflict inline.
- Block type: search-snippet-only / build-cost-only (wikis print build costs; research costs not stated). Threshold to fully close: datamined game-file values.

### Single-source fan theory -- Winterhome survivor → New London
- Source: community-wiki (single source)
- Block type: search-snippet-only / unverifiable in-game
- The claim that the Winterhome scout/survivor becomes the figure who triggers the Londoners crisis in A New Home is a fan theory, never confirmed in-game. Flagged `[Single source -- verify]` in `sections/fall_of_winterhome.md` and `sections/story_notes.md`.

## Always-blocked categories

- **In-game UI elements:** Frostpunk's technology tree node costs and exact worker-count thresholds may not be fully documented in text guides. The in-game UI is the authoritative source; P1 researcher should transcribe from a comprehensive Let's Play or wiki screenshot source.
- **Randomized elements:** The Frostland (expedition map) has some randomization in resource cache contents. Per-save variance won't be captured in the corpus; claims about expedition yields will carry confidence ranges.
