# Frostpunk -- Architecture Manifest

**status:** research-integrated
**last_reconciled:** 2026-06-03 (P3)
**research_run:** P1 ingested 2026-06-02; P2 ingested 2026-06-02; P3 ingested 2026-06-03

This file serves as the corpus manifest and structural anchor. `nav/` was skipped (game-type: on-rails; localization-mechanism: none -- no spatial player navigation in Frostpunk). Zone graph, per-zone gate lists, and localization toolkit are not applicable. Because `nav/` is absent, this file is the home for cross-scenario structural facts (scenario registry, expedition/optional-content registry, scenario-graph unlocks).

## Hintforge manifest

<!-- Read by the reader at session start (see docs/corpus-format.md §3). Bump corpus-core-version only when a change to docs/corpus-format.md would break an older reader; see the Versioning subsection in that doc. game-version-* fields describe the game build the corpus was authored against (player-supplied at setup; required as of v3); they are orthogonal to corpus-core-version (which is the schema axis). -->

```
corpus-core-version: 5
game-version: "latest"
game-version-platform: "PC / Steam"
game-version-as-of: 2026-06-03
vector-extensions: endings, paths
```

## Vector extensions

<!-- Wizard populates from Step 7 conditional-creation decisions. One entry per extension created. Reader uses this list to route topical questions to the right folder. -->

- `endings/` -- scenario victory/defeat conditions and ending branches; indexed by `endings/index.md`
- `paths/` -- law path branches (Faith tree vs Order tree) and their mechanical consequences; indexed by `paths/index.md`

## Game-type label

**on-rails** -- scenarios unfold on a fixed day-count timeline. No spatial zone graph applies. Scenario structure (days, event triggers, key milestones) is documented in `sections/` and populated at P1 ingestion.

## Localization-mechanism class

**none** -- no player avatar navigating zones. The city is always the same top-down view. Expeditions are dispatched, not traversed. No localization toolkit, landmark lists, or map-system prompts needed.

## Scenario registry

Equivalent to the zone/chapter list for on-rails games. One entry per scenario. Scenarios are **isolated** -- no save-state carries between them.

| Scenario | Scope | Approx. length | Unlock | Notes |
|---|---|---|---|---|
| A New Home | Base game -- P1 | ~48 days (storm latest day 43 w/o exploits) | from start | Main campaign; 3 acts; culminates in the Great Storm. City "New London" |
| The Refugees | Base game -- P1 | ~26-30 days | after surviving 20 days of A New Home | Refugee/Lord waves; save 250 people |
| The Arks | Base game -- P1 | ~22-27 days | after surviving 20 days of A New Home | Automaton-focused; 4 Seedling Arks; New Manchester arc. City "Legacy" |
| The Fall of Winterhome | Base game -- P1 | ~22-26 days | from start (free update) | Reconstruction → evacuation via Land Dreadnought |
| Endless Mode | Base game -- P1 | unlimited | from start (free update, patch 1.3.0) | Sandbox; cyclical storms. Sub-modes Serenity / Endurance (+ Builders = DLC) |
| The Last Autumn | DLC (prequel) | ~45 days (Day-37 sea-freeze gate; icebreaker Day 45) | DLC purchase only | Prequel; construction of the Generator at Site 113. No Purpose laws; Administration + Labour books. See `sections/the_last_autumn.md` |
| On The Edge | DLC (post-game) | ~3 acts (~40 days) | DLC purchase only | Post-A New Home outpost management; Settlements diplomacy; no Generator. See `sections/on_the_edge.md` |

**Scenario graph:** A New Home is available from start; The Arks and The Refugees each unlock after **surviving 20 days** in A New Home; The Fall of Winterhome and Endless Mode are available from the start via Select Scenario (added by free updates). No scenario shares state with another. Lore chronology: The Last Autumn → The Fall of Winterhome → A New Home / The Arks / The Refugees (parallel) → On The Edge.
_source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

## Optional content registry

Expedition destinations (Frostland). Each scenario has its **own** Frostland variant map; nodes are not shared identically. A New Home nodes (full list; The Refugees / The Arks variants summarized below):

| Expedition location | Scenario | Unlock condition | Access window | Yield | Notes |
|---|---|---|---|---|---|
| Weather Station | A New Home | scouting | early | 91 coal + 1 core | unlocks Winterhome + Coal Mine |
| Winterhome | A New Home | via Weather Station | mid | story trigger | unlocks 'We're On Our Own'; reveals Snow Cliff + American Camp |
| Snow Cliff | A New Home | via Winterhome | mid | 98 rations, 61 wood, 1 core | reveals Shrouded Cave + Freshwater Springs |
| Freshwater Springs | A New Home | via Snow Cliff | mid | 7 children + 22 workers | reveals Frozen Grove |
| Shrouded Cave | A New Home | via Snow Cliff | mid | 34 children | — |
| Frozen Grove | A New Home | via Freshwater Springs | mid | 258 wood | — |
| Large Convoy | A New Home | scouting | mid | 18 engineers + 26 workers | — |
| Coal Mine (Outpost) | A New Home | scouting | mid | 263 coal, then 800/day | if lost: 202 coal/208 wood/2 cores |
| Tesla City (Outpost) | A New Home | after Winterhome discovered | before storm | 1 core/day (only renewable core source) | **missable** -- rushing Winterhome shortens the window; max 2 Outposts per city |
| Destroyed Steam Core Transports ×2 | The Refugees | starting crater | start | 2 cores each (4 total) | only scenario with cores in ground piles |
| Broken Automaton node | The Arks | scouting (eye-shaped crater) | mid | automaton | Arks crater has **no Outpost Depot** location |

_source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression · missable: yes (Tesla City)_

See `sections/a_new_home.md` for full A New Home expedition detail; `mechanics.md` Expedition System for the scout/Beacon mechanics.

## Support topology

### Save system

Full save-system table: `mechanics.md` §Save system. Survivor-mode requirements: `mechanics.md` §Difficulty Modes. No save-state carries between scenarios -- each is fully independent (see §Scenario registry above).

### Fast-travel network

None -- the city is always the single view; no fast travel between locations.

## Locks and Keys (scenario-level gates)

_source: Deep Research handoff 2026-06-02 (P2) · capture: web_fetch · confidence: high (confirmed rows) / medium (estimated rows) · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

### Technology prerequisites (tech-as-key)

All locked nodes are **visible (greyed)** in the tech-tree UI before their key is researched. No base-game tech requires a Steam Core to research; cores are build-only.

| Lock | Scenario(s) | Key required | Research cost of key | Notes |
|---|---|---|---|---|
| Tier 1 techs | All | Drawing Boards | **50 Wood** | Unlocks all T1 nodes |
| Tier 2 techs | All | Drafting Machines | **75 Wood / 25 Steel** | |
| Tier 3 techs | All | Mechanical Calculators | **100 Wood / 50 Steel** | |
| Tier 4 techs | All | Difference Engine | **125 W / 75 S** (confirmed 2 sources, readonly.wiki) | |
| Tier 5 techs | All | Automatic Prototyping | **150 W / 100 S** (single source -- verify, readonly.wiki) | |
| Sawmill | All | Workshop | **10 Wood** (T0) | |
| Steelworks | All | Workshop | **10 Wood** (T0) | |
| Advanced Steelworks | All | Steam Steelworks | ~50 W / 30 S (T4, estimate) | `[Single source -- verify · class:tier-estimate]` |
| Wall Drill | All | Drawing Boards | ~20 Wood (T1, inferred) | `[Single source -- verify · class:community-forum]`; building needs Steam Core to build |
| Infirmary | All | Medical Post Upgrade | ~30 W / 20 S (T2, estimate) | `[Single source -- verify]`; building needs 1 Steam Core |
| Beacon | All | Workshop | **10 Wood** (T0) | Build: 20 W / 35 S; scout team: 40 W / 5 workers |
| Factory | A New Home: **not available** (not researchable; no fixed scouting path in ANH); Refugees/Winterhome: Drafting Machines (T2) | Drafting Machines | **30 W / 20 S** | Factory blueprints obtainable only via the Lost Dreadnought node in The Arks (a separate scenario). In Refugees/Winterhome, Factory is researchable via Drafting Machines. |
| Heater Efficiency Upgrade | All | Improved Heaters | **60 W / 40 S** (T3; above-tier-baseline like range upgrades) | `[Single source -- verify · class:wiki-NamuWiki]` |
| Advanced Heaters | All | Improved Heaters | **50 W / 30 S** (T4 baseline) | single-source (tier-confirmed, readonly.wiki) |
| Generator Range Upgrade II | All | Range Upgrade I | **60 W / 40 S** | confirmed (2 sources: NamuWiki + readonly.wiki) |

### Law prerequisites (law-as-key)

| Lock | Scenario(s) | Key required | Notes |
|---|---|---|---|
| Adaptation laws | All | None | Available from scenario start |
| Purpose laws (Faith/Order) | A New Home | Londoners crisis (scout Winterhome OR day-15 messenger) | Permanent once first Purpose law signed |
| Purpose laws | The Refugees | None (available from start) | No trigger gate |
| Purpose laws | The Arks | N/A -- never available | Adaptation tree only; Children laws also absent |
| Purpose laws | Fall of Winterhome | None (available from start, none pre-chosen) | |
| Purpose laws | Endless Mode | None (available from start) | |
| Faith Keepers / The Temple | Faith scenarios | Evening Prayers (House of Prayer → Evening Prayers first) | Both branch from Evening Prayers |
| Public Penance → Protector of the Truth | Faith scenarios | Faith Keepers | Full chain confirmed (German wiki) |
| New Faith | Faith scenarios | Protector of the Truth (or Righteous Denunciation branch) | Terminal law; removes Hope meter |
| Pledge of Loyalty | Order scenarios | Propaganda Centre | |
| Forceful Persuasion | Order scenarios | Pledge of Loyalty | "Crossing the line" law |
| New Order | Order scenarios | Forceful Persuasion | Terminal law; replaces Hope with Obedience |
| Locked laws in Book of Laws | All | Preceding law signed | Visible (greyed) before prerequisite; cooldown between signings |

_source: Deep Research handoff 2026-06-02 (P2, 4 sources incl. German wiki for Faith chain) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

### Building prerequisites (building-as-key)

| Lock (building) | Key required | Notes |
|---|---|---|
| Technology tree access | Workshop built + Engineers assigned | |
| Scout teams | Beacon built | Scout = 40 wood / 5 workers |
| Outpost teams | Outpost Depot researched (T2; needs Beacon) | Team = 40 wood / 20 steel / 10 workers; max 2 Outposts in A New Home |
| Steam Hub heat relay | Steam Hub tech | Extends generator heat zone |
| Infirmary (building) | Infirmary tech + 1 Steam Core | |
| Factory | Factory tech (or scouted plans in The Arks) + 1 Steam Core | Automaton = 100 wood / 100 steel / 50 coal / 1 core |
| Hothouse / Coal Mine / Wall Drill | Respective tech + 1 Steam Core to build | |

Key dependency chain: **Workshop → Technology Tree → (Drawing Boards → higher tiers); Beacon → Scouting/Outposts; Steam Hub → heat relay extension.** [Confirmed: 4 sources]

### Expedition prerequisites (expedition-as-key)

| Gate | Key / Requirement | Notes |
|---|---|---|
| Scouting access | Beacon built | Research: 10 W; Build: 20 W / 35 S |
| Scout team count | More Scouts / Additional Scouts techs | Base: 1 team |
| Scout speed | Lighter Scout Sleds / Boosted Scout Sleds; Faster Outpost Teams | Scouts halve travel time to already-visited nodes |
| Outpost limit (A New Home) | Max 2 Outposts per city | The Arks, Endless Mode: no Outposts |
| Tesla City route (A New Home) | Winterhome discovered first | Eastern scouting route only opens after Winterhome |
| Lost Dreadnought (The Arks) | Scout must reach node | Yields Factory blueprints; Factory not otherwise researchable in The Arks |

**Outpost yields (A New Home):** Winterhome 150 wood/day; Coal Mine 800 coal/day; Fishing Village 100 raw food/day; Tesla City 1 steam core/day; Icebound Dreadnought 100 steel. Most other scouting nodes are partially randomized per playthrough.
_source: Deep Research handoff 2026-06-02 (P2, 4 sources; Coal Mine yield: Official Frostpunk Wiki) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

### Scenario-unlock prerequisites (scenario-as-key)

| Scenario | Unlock condition |
|---|---|
| A New Home | From start |
| The Fall of Winterhome | From start (free update) |
| Endless Mode | From start (free update) |
| The Refugees | Survive 20 days of A New Home |
| The Arks | Survive 20 days of A New Home |
| The Last Autumn | DLC purchase only (The Last Autumn DLC); also unlocks Builders endless mode |
| On The Edge | DLC purchase only (On The Edge DLC); narratively post-A New Home but NOT gated behind completing it |

No achievement-gated scenario unlocks exist. [Confirmed: 4 sources + P3 fandom/PSNProfiles]
_source: Deep Research handoff 2026-06-02 (P2, 4 sources) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

### Missable-trigger gates (point-of-no-return summary)

See `sections/missables.md` for the full aggregated catalog. Summary of hard-deadline PoNR gates:
- **Tesla City Outpost** (A New Home): before storm or permanently lost.
- **Day-15 Winterhome messenger** (A New Home): Winterhome must be scouted before ~10:00 day 15.
- **Steel Bridge automaton** (Fall of Winterhome): taking it permanently blocks Iron Deposit steel.
- **"Crossing the line" Purpose laws** (all Purpose scenarios): block the Golden Path permanently.
- **Radical Treatment "A Frightened Patient"**: refusing amputation kills the patient.
- **Lost Dreadnought** (The Arks): must reach node or Factory plans unobtainable.
- **The Lie** (Fall of Winterhome): triggers blackmail arc, may force killing an engineer.
- **A New Home storm latest day 43**; The Arks win-gate objectives and Winterhome generator final 48 hours are hard endgame deadlines.
- **The Last Autumn Worker/Engineer choice** (post-first-strike): permanent PoNR -- locks one Labour law branch permanently. `dlc:the_last_autumn`
- **The Last Autumn Day-37 sea-freeze**: Docks unusable; logistics locked; must have all 4 construction stages done to leave early. `dlc:the_last_autumn`
- **On The Edge first shipment** (≤ Day 7 18:00): miss it → 24h last chance; miss that → instant game over. `dlc:on_the_edge`
- **On The Edge independence**: irreversible; law signing enabled; triggers law-path locking. `dlc:on_the_edge`
- **On The Edge final Save/Let Fall binary choice** (12h timer): permanently locks ending branch. `dlc:on_the_edge`
_source: Deep Research handoffs 2026-06-02 (P2, confirmed) and 2026-06-03 (P3, confirmed) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_
