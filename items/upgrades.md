# Frostpunk -- Technology Tree (Upgrades)

**status:** research-integrated
**last_reconciled:** 2026-06-03 (P3)

Full Technology Tree for Frostpunk, base game. Built by a **Workshop** with engineers assigned; organized in **tiers 0-5** (each tier unlocked in sequence: Tier 1 = Drawing Boards 50 Wood / 5h; Tiers 2-5 = Drafting Machines, Mechanical Calculators, Difference Engine, Automatic Prototyping). **Research rate:** 5 engineers = 100%, diminishing returns above (10 eng ≈ 130%, 25 eng ≈ 170%). **No base-game tech requires a Steam Core to research** -- cores are build-only.

Three tabs are shared across all base scenarios (Heating; Resources; Food/Health & Shelter), plus Exploration & Industry. Endless Mode uses the A New Home tree minus Stereoscopic Lenses and Outpost Depot.

> **P3 cost-resolution note (2026-06-03):** Research costs follow a tier-based schedule independently confirmed by English + Korean wikis (readonly.wiki / NamuWiki mirror). Schedule: T0/Basic = 10 Wood; T1 = 20W/10S; T2 = 30W/20S; T3 = 40W/25S; T4 = 50W/30S; T5 = 120W/80S (exceptions: Advanced Coal Mine and Coal Thumper Injectors = 60W/35S; range/heater upgrades exceed their tier baseline). Tier-unlock techs: Drawing Boards 50W (T1) · Drafting Machines 75W/25S (T2) · Mechanical Calculators 100W/50S (T3) · Difference Engine **125W/75S** (T4, confirmed 2 sources) · Automatic Prototyping **150W/100S** (T5, single source). Rows formerly flagged [Hypothesis] or [research cost unconfirmed] are resolved below; remaining single-source entries are noted.
> **BUILD COST ≠ RESEARCH COST.** Wikis frequently print the building's build cost (e.g., Steam Steelworks "40W/15S", Bunkhouse "20W/10S"). These are NOT research costs. All costs below are research-only.

_All nodes below: source: Deep Research P3 handoff 2026-06-03 (readonly.wiki / NamuWiki + English sources) · capture: web_fetch · confidence: high unless flagged · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

---

## Heating tab

**status:** research-integrated

| Node | Prereq | Tier | Research cost | Confidence | Effect |
|---|---|---|---|---|---|
| Steam Hub | none | 0 | **10 Wood** | confirmed (2 sources) | Builds Steam Hubs (heat zone = Generator level, on roads) |
| Steam Hub Range Upgrade | Steam Hub | 2 | **30 W / 20 S** | confirmed | +50% range, 2× coal |
| Steam Hub Efficiency Upgrade | Range Upgrade | 4 | **50 W / 30 S** | confirmed | −33% Steam Hub coal |
| Generator Power Upgrade I | none | 1 | **20 W / 10 S** | confirmed | +1 heat level (coal 6→12/h) |
| Generator Power Upgrade II | Power I | 3 | **40 W / 25 S** | confirmed | +1 (→18/h) |
| Generator Power Upgrade III | Power II | 5 | **120 W / 80 S** | confirmed | +1 (→24/h) |
| Generator Efficiency Upgrade I | Power I | 2 | **30 W / 20 S** | confirmed | −10% generator coal |
| Generator Efficiency Upgrade II | Efficiency I | 4 | **50 W / 30 S** | confirmed | −10% more (−20% total) |
| Overdrive Couplings | Power I | 2 | **30 W / 20 S** | confirmed | Overdrive +2 instead of +1 |
| Generator Safety Bypass | Overdrive Couplings | 5 | **120 W / 80 S** | confirmed | Overdrive stress +25% slower / −25% faster |
| Generator Range Upgrade I | none | 1 | **20 W / 10 S** | confirmed | +3 tiles range, 2× coal |
| Generator Range Upgrade II | Range I | 3 | **60 W / 40 S** | confirmed (2 sources; above T3 baseline -- range upgrades exceed tier) | +3 tiles, 3× coal |
| Generator Range Upgrade III | Range II | 5 | **120 W / 80 S** | confirmed | +3 tiles, 4× coal |
| Heaters | none | 0-1 | **10 Wood** | confirmed | Independent building heating mode (+1) |
| Improved Heaters | Heaters | 2 | **30 W / 20 S** | confirmed | +2 |
| Heater Efficiency Upgrade | Improved Heaters | 3 | **60 W / 40 S** | single-source · verify (readonly.wiki; above T3 baseline like range upgrades) | reduces heater coal |
| Advanced Heaters | Improved Heaters | 4 | **50 W / 30 S** | single-source (T4 baseline; readonly.wiki) | +3 |

> Note: Heater Efficiency Upgrade was previously hypothesized at ~30W/20S; P3 research (readonly.wiki) returns 60W/40S -- above the T3 baseline, consistent with the range-upgrade pattern. Verify against a second source or in-game screenshot before treating as confirmed.

---

## Resources tab

**status:** research-integrated

| Node | Prereq | Tier | Research cost | Confidence | Effect |
|---|---|---|---|---|---|
| Faster Gathering | none | 0 | **10 Wood** | confirmed (2 sources) | +gather rate |
| Resource Depot Upgrade | Faster Gathering | 1 | **20 W / 10 S** | confirmed | bigger depot |
| Large Resource Depot | Resource Depot Upgrade | 2 | **30 W / 20 S** | single-source (tier-derived; ⚠️ some wikis print 75 Steel -- that is the BUILD cost) | largest depot |
| Coal Thumper | none | 1 | **10 Wood** | confirmed | Builds Coal Thumper (560/day) |
| Steam Coal Thumper | Coal Thumper | 3 | **30 W / 20 S** | confirmed | 1120/day |
| Coal Mining | none | 1 | **20 W / 10 S** | confirmed (2 sources: readonly.wiki + English) | Builds Coal Mine (240/10h) |
| Coal Mining Optimisation / Rationalisation | Coal Mining | 2 / 3 | Rationalisation **50 W / 30 S** (T3) | confirmed | +10% each |
| Steam Coal Mine | Coal Mining | 3 | **40 W / 25 S** | confirmed | upgrade (strong) |
| Advanced Coal Mine | Steam Coal Mine | 5 | **60 W / 35 S** (T5 exception) | confirmed | best sustained coal |
| Charcoal Kiln | none | 1 | **20 W / 10 S** | single-source (T1 tier-derived; game-vault) | wood→coal |
| Sawmill | none | 0 | **10 Wood** | confirmed | finite wood |
| Steam Sawmill | Sawmill | 2 | **30 W / 20 S** | single-source (T2 tier-derived) | upgrade |
| Sawmill Upgrade | Sawmill | 1 | **20 W / 10 S** | single-source (T1 tier-derived) | +efficiency |
| Sawmill Range Extension | Sawmill Upgrade | 4 | **50 W / 30 S** | single-source (T4 tier-derived) | +range |
| Wall Drill | none | 1 | **20 W / 10 S** | confirmed (2 sources: Steam thread derivation + readonly.wiki); building needs 1 Steam Core to build | infinite wood |
| Steam Wall Drill | Wall Drill | 3 | **40 W / 25 S** | single-source (T3 tier-derived; ⚠️ fandom "20W/40S/2 Cores" is the Advanced Wall Drill BUILD cost -- do not conflate) | upgrade |
| Advanced Wall Drill | Steam Wall Drill | 5 | **120 W / 80 S** | single-source (T5 tier-derived) | upgrade |
| Steelworks | none | 0 | **10 Wood** | confirmed | only steel source (60/day) |
| Steam Steelworks | Steelworks | 2 | **30 W / 20 S** | single-source (T2 tier-derived; ⚠️ fandom "40W/15S" is the BUILD cost) | upgrade |
| Advanced Steelworks | Steam Steelworks | 4 | **50 W / 30 S** | single-source (T4 tier-derived; ⚠️ fandom "80W/40S" is the BUILD cost) | upgrade |

---

## Food, Health & Shelter tab

**status:** research-integrated

| Node | Prereq | Tier | Research cost | Confidence | Effect |
|---|---|---|---|---|---|
| Hothouse | none (New Home / Refugees / Arks / Winterhome) | 1 | **20 W / 10 S** | confirmed | core-powered infinite food |
| Hothouse Insulation / II | Hothouse | 2 / 4 | Insulation **30 W / 20 S** | confirmed | less heat demand |
| Industrial Hothouse | Hothouse | 3 | **40 W / 25 S** | confirmed | upgrade |
| Hunters' Gear | none (not in Arks) | 1 | **10 Wood** | single-source (basic T0/T1 tech; tier-derived) | builds Hunters' Hut |
| Hunting Tactics | Hunters' Gear | 2 | **30 W / 20 S** | confirmed (2 sources: readonly.wiki + English) | +efficiency |
| Flying Hunters | Hunters' Gear | 2 | **30 W / 20 S** | confirmed (2 sources: readonly.wiki) | Hangar |
| Flying Hunters' Gear | Flying Hunters | 4 | **50 W / 30 S** | confirmed | upgrade |
| Medical Post Upgrade | none | 1 | **20 W / 10 S** | confirmed | +capacity |
| Healthcare Insulation | Medical Post Upgrade | 2 | **30 W / 20 S** | confirmed (2 sources: readonly.wiki) | less heat demand |
| Healthcare Insulation II | Healthcare Insulation | 5 | **120 W / 80 S** | confirmed (2 sources: readonly.wiki + dcinside) | greater heat reduction |
| Infirmary | Medical Post Upgrade | 2 | **30 W / 20 S** | single-source (T2 tier-derived; note: building needs 1 Steam Core to BUILD -- not research) | cures gravely ill |
| Infirmary Mechanisation | Infirmary | 3 | **40 W / 25 S** | single-source (T3 tier-derived) | +efficiency |
| Infirmary Checklists | Infirmary Mechanisation | 4 | **50 W / 30 S** | confirmed (2 sources: readonly.wiki) | further efficiency |
| Bunkhouse | none | 1 | **20 W / 10 S** | single-source (T1 tier-derived; ⚠️ build cost is also 20W/10S -- coincidental, do NOT conflate) | housing |
| House | Bunkhouse | 3 | **40 W / 25 S** | single-source (T3 tier-derived; ⚠️ build cost is also 40W/25S -- coincidental) | better housing |
| House Redesign | House | 4 | **50 W / 30 S** | confirmed (2 sources: readonly.wiki) | +capacity |
| House Insulation | House Redesign | 5 | **120 W / 80 S** | confirmed (2 sources: readonly.wiki + dcinside) | less heat demand |

---

## Exploration & Industry tab

**status:** research-integrated

| Node | Prereq | Research cost | Confidence | Effect |
|---|---|---|---|---|
| Beacon | none | **10 Wood** (T0; build: 20W/35S; scout team: 40W/5 workers) | confirmed | enables scouting |
| Automaton Scouts | Beacon | **20 Wood** (T1, wood-only; Arks-exclusive) | confirmed (2 sources: readonly.wiki) | automaton expeditions |
| More Scouts | Beacon | **20 Wood** (T1, wood-only) | confirmed (2 sources: readonly.wiki) | +1 scout team |
| Additional Scouts | More Scouts | **50 W / 30 S** (T4) | confirmed (2 sources: readonly.wiki) | +more scout teams |
| Lighter Scout Sleds | More Scouts | **30 Wood** (T2, wood-only) | confirmed (2 sources: readonly.wiki) | +scout speed |
| Boosted Scout Sleds | Lighter Scout Sleds | **120 W / 80 S** (T5) | confirmed (2 sources: readonly.wiki) | +further scout speed |
| Outpost Depot | Beacon (not in Endless / Arks) | **30 W / 20 S** (T2; A New Home/Refugees/Winterhome only) | confirmed (2 sources: readonly.wiki) | enables Outposts |
| Factory | see notes | **30 W / 20 S** (T2; build: 30W/15S/1 core; NOT researchable in A New Home -- plans only via Lost Dreadnought in The Arks) | confirmed | builds Automatons |
| Streamlined Automatons | Factory | **40 W / 25 S** (T3) | confirmed (2 sources: readonly.wiki) | −20W/−20S per automaton |
| Automaton Redesign | Streamlined | **120 W / 80 S** (T5) | confirmed (2 sources: readonly.wiki) | −30W/−30S per automaton |
| Automaton Integration I / II / III | Factory | 40/25, 50/30, 120/80 | confirmed | +automaton efficiency |
| Medical Automatons | Integration | **50 W / 30 S** (T4) | confirmed (2 sources: readonly.wiki) | automatons in medical |
| Engineer Automatons | Integration | **50 W / 30 S** (T4) | confirmed (2 sources: readonly.wiki) | automatons in workshop |
| Stereoscopic Lenses | Beacon (not Endless) | **10 W / 100 S** | confirmed | scout-found tech reveal |

A single **Automaton** costs **100 Steel, 100 Wood, 50 Coal, and 1 Steam Core** to build (official Frostpunk Wiki, The Arks).

---

## Tier-unlock nodes

| Node | Tier unlocked | Research cost | Confidence |
|---|---|---|---|
| Drawing Boards | T1 | **50 Wood** | confirmed |
| Drafting Machines | T2 | **75 W / 25 S** | confirmed |
| Mechanical Calculators | T3 | **100 W / 50 S** | confirmed |
| Difference Engine | T4 | **125 W / 75 S** | confirmed (2 sources: readonly.wiki) |
| Automatic Prototyping | T5 | **150 W / 100 S** | single-source · verify (readonly.wiki; no English wiki confirmation) |

---

## Scenario-specific tech notes

**status:** research-integrated

- **The Arks** -- Hunters' tech line is unavailable (no Hunters; food is Hothouse-only). Automaton tech (Factory → Engineer Automatons) is the win-condition priority.
- **The Fall of Winterhome** -- reconstruction-driven; the steel line (Advanced Steelworks) is the gating research because the Dreadnought needs 9000 steel.
- **Endless Mode** -- A New Home tree minus Stereoscopic Lenses and Outpost Depot (no Outposts in Endless).
- **The Last Autumn** (DLC) -- Heating tab uses Heaters/Braziers only (no Generator upgrade line). Resources/Food-Health tabs are modified (adds Docks, Reloading Stations, Fishing Harbour, Foragers). Exploration & Industry replaced by **Generator Construction** tab (Profiles Manufacture, Foundry, Machine Shop, Ventilation Plant). See `sections/the_last_autumn.md`.
- **On The Edge** (DLC) -- Heating tab Generator line replaced by Braziers branch. Resources tab Steelworks/Wall-Drill line replaced by Army Warehouse upgrades (Handcarts, Wooden Support). Outpost Depot and Stereoscopic Lenses unavailable. See `sections/on_the_edge.md`.
  _source: Deep Research P3 handoff 2026-06-03 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

---

## Remaining single-source entries (verify threshold)

Threshold to upgrade any "single-source (tier-derived)" to "confirmed": one English primary source printing the word "research" for that specific node, or a datamined game-file value. These nodes rest on tier-derivation from the readonly.wiki schedule or game-vault tier data:
- Heater Efficiency Upgrade (60W/40S -- also contradicts prior hypothesis; priority verify)
- Large Resource Depot (30W/20S)
- Charcoal Kiln (20W/10S)
- Steam Sawmill, Sawmill Upgrade, Sawmill Range Extension
- Steam Wall Drill, Advanced Wall Drill
- Steam Steelworks, Advanced Steelworks (confirmed tier-derived; build-cost conflation risk high)
- Automatic Prototyping (150W/100S)
- Infirmary, Infirmary Mechanisation, Bunkhouse, House
- Hunters' Gear

---

## Recommended research order (mainstream convergence)

- **Early:** Sawmill or Wall Drill, Coal Mining, Beacon, a heating upgrade.
- **Mid:** Steelworks line, Steam Hubs, Hothouse/Hunters, Factory.
- **Late:** Generator Power III + Range III, Advanced Heaters, Safety Bypass, advanced resource buildings.
  _source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

See `items/builds.md` for scenario-specific priority orders.

---

## Sources

- frostpunk.fandom.com (individual tech pages); frostpunk-archive.fandom.com (cost stubs)
- readonly.wiki (mirror of NamuWiki) and thewiki.kr / dcinside -- Korean tech research-cost listings (primary non-English source)
- frostpunk.game-vault.net -- full Technology Tree (tier/prerequisite structure)
- Nexus Mods datamined vanilla baselines (post-patch 1.x); TheGamer, stopgame.ru
- Deep Research handoffs, 2026-06-02 (P1/P2) and 2026-06-03 (P3).
