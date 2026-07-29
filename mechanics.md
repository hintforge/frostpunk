# Frostpunk -- Mechanics

**status:** research-integrated
**last_reconciled:** 2026-06-02

Core game-system rules. AI agent reads this for cross-scenario system knowledge. Per-scenario facts go in `sections/`; tech tree specifics in `items/upgrades.md`; law-path strategy in `paths/` and `items/builds.md`.

---

## Heat System

**status:** research-integrated

The Generator is the city's single heat source, radiating heat in a concentric circular radius around itself. Workers and buildings outside the heat radius work slower and accumulate cold-related illness faster. "Movement" in Frostpunk is camera pan/rotate/zoom only -- there is no player avatar and no navigable zones; the city is always viewed top-down.

- The Generator's heat radius and intensity are extended/raised through the Heating tech tab (Generator Power, Range, Efficiency, Overdrive). See `items/upgrades.md` Heating tab for node-by-node costs.
- **Steam Hubs** relay heat to remote districts: a Steam Hub's heat zone equals the Generator's current power level and must be placed on roads. Range and efficiency are upgradeable.
- **Heaters** provide independent per-building heating (a separate mode), upgradeable via Improved Heaters / Advanced Heaters.
  _source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_
- **Exception -- buildings that need no heat to operate:** Hunters' Huts, Beacons, and Storage operate cold. Placing them outside the heat radius frees prime warm real estate near the Generator for housing. (Common-knowledge rule "you always need heat" has documented exceptions.)
  _source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_
- **Overdrive trick (endgame):** run the Generator to 100% stress, then reset to ~65% with a steam core for the final push (e.g. the last day of the Great Storm). The max-upgraded Infirmary is the warmest building in the city.
  _source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 2 · category: mainline · spoiler: late-game_

---

## Hope and Discontent

**status:** research-integrated

Two aggregate city-wide meters. If Discontent reaches maximum or Hope reaches minimum, the population revolts and the run ends. They are not inversely linked -- both can be low simultaneously.

- The **Purpose** law trees (Faith / Order) exist primarily to raise Hope and lower Discontent; their existence and mid-scenario unlock are progression content. See `paths/` for full law effects.
  _source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_
- **Endgame consequence:** the final law of each Purpose branch (New Faith / New Order) **eliminates the Hope meter entirely** and auto-builds an Execution Platform. Under the Order path, the Hope bar is replaced by an **Obedience** bar.
  _source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 2 · category: mainline · spoiler: late-game_
  > see `paths/faith_path.md` and `paths/order_path.md` for the full branch chains and ending consequences.
  > **Cross-system dependency** -- see `dependencies.md` DEP-002: New Faith / New Order terminal laws remove the Hope meter from the game entirely; see `paths/` for the specific crossing-the-line laws that also lock the Saviour ending (PON-002).

---

## Resource Management

**status:** research-integrated

The base game has **five** stored/counted resources: **Coal, Wood, Steel, Steam Cores, and Food** (Raw Food + Rations). **Correction to common listings:** "Iron" is *not* a stored player resource in the base game -- it is only an in-ground deposit type mined into Steel by the Steelworks. Steel is the stored resource.
_source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

**Base gather rate** per person per standard 10-hour workday (Medium difficulty, excluding tech/efficiency/Extended Shift): **24 Coal OR 7 Wood OR 5 Steel OR 0.2 Steam Cores** at a Gathering Post on a pile. Gathering Posts roughly double pile-harvest rate and keep their workers warm.
_source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

### Coal
Production: Gathering Posts on coal piles; **Coal Thumper** (560 coal/workday, creates an infinite pile but needs heavy manpower -- rule of thumb 1 thumper feeds 2 Gathering Posts; **Steam Coal Thumper** = 1120/day feeds 4); **Coal Mine** (240 coal/10h, on a deposit, needs a steam core); **Charcoal Kiln** (converts wood → coal); **Coal Mine Outpost** in A New Home (800/day); **Advanced Coal Mine** is the top sustained source. Consumption sinks: Generator (base 12/h, rising to 24/h at Power Upgrade III; coal cost multiplies ×2/×3/×4 with Range Upgrades I/II/III), Steam Hubs, Heaters, Automatons.
_source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

- **Edge case (commonly missed) -- "phantom" coal income:** the economy panel lists Gathering Post output based only on worker count, ignoring whether the thumper actually supplies enough coal to the pile. A thumper showing a green surplus can still let the Generator shut off. Rule of thumb: one thumper supports only **2** Gathering Posts.
  _source: Deep Research handoff 2026-06-02 (2 forum sources) · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

### Wood
Production: Gathering Posts on wood crates/piles; **Sawmill** (finite -- harvests nearby frozen trees, must relocate when depleted; Steam Sawmill upgrade); **Wall Drill** (infinite -- extracts wood from the ice wall, needs a steam core; the community-preferred "wall drill rush"). Consumption: all research (tech costs wood ± steel), construction, Charcoal Kilns, the prosthetics line. **Wood is the de-facto research currency** -- the single most important early resource.
_source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

### Steel
Production: **Steelworks ONLY** (60 steel/day base; ~25 wood to build; mines iron deposits; Steam Steelworks & Advanced Steelworks upgrades). **The steel bottleneck:** steel is the only resource with a single building family fixed to finite deposit locations -- no infinite alternative, no conversion path. It is the pacing bottleneck, especially in The Fall of Winterhome (the Dreadnought needs 9000 steel). Community consensus: prioritize Advanced Steelworks before other advanced buildings.
_source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

### Steam Cores -- finite; cannot be created or destroyed
Cores are fully **refunded on deconstruction** (never a permanent loss except via specific story arcs, or repairing a generator at 100% stress) -- they are never "truly lost." Buildings requiring a core to build/operate: Coal Mine, Wall Drill, Hothouse line, Factory, Infirmary, Automatons. **Steel never requires a core. No base-game *tech* requires a core to research** (cores are build-only; the Nexus Balance Mod that adds core research costs is a mod, not vanilla).
_source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

Per-scenario core supply: see each `sections/<scenario>.md`. Summary -- A New Home: scouting + 1 automaton at the Steel Bridge node + Tesla City Outpost (1/day, the only renewable source).
> **Cross-system dependency** -- see `dependencies.md` DEP-001: Tesla City Outpost is the sole renewable Steam Core source in A New Home; it is missable (must be reached before the Great Storm closes the Beacon -- see PON-001). The Refugees: scouting + 2 Destroyed Steam Core Transports (4 total) + cores in starting piles (the only scenario where cores appear in ground piles). The Arks: start 2-3, scouting, new core locations spawn only after you run out. The Fall of Winterhome: scouting; the Dreadnought consumes 10 cores fully upgraded. Endless: effectively unlimited (Rifts map starts with 5).

### Food
Raw Food → Food Rations via **Cookhouse** (2 Raw = 4 Rations standard; **Soup** law = 5; **Sawdust / Food Additives** = 6). Production: **Hunters' Hut / Hangar** (infinite, no steam core, works in cold, needs no heat) and **Hothouse** (infinite, needs steam core + heat; better very early before hunting tech). Both are **disabled during storms** -- stockpile **raw food** rather than rations (more storage-efficient, since Cookhouses keep converting).
_source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

### Scarcity / bottleneck patterns (per scenario)
- **A New Home:** food during the final storm (#1 death cause); steel mid-game.
- **The Refugees:** housing + medical capacity (waves of sick refugees); food on hard/extreme.
- **The Arks:** workforce (fixed 45 engineers, no new workers) and steam cores; coal at the end (8000-coal win gate).
- **The Fall of Winterhome:** steel (9000 for the Dreadnought) and time.
  _source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

---

## Technology Tree

**status:** research-integrated

Built by a **Workshop** with engineers assigned; organized in **tiers 0-5** (each tier must be unlocked: Tier 1 = Drawing Boards 50 Wood / 5h; Tiers 2-5 = Drafting Machines, Mechanical Calculators, Difference Engine, Automatic Prototyping). Three tabs are shared across all base scenarios -- **Heating; Resources; Food/Health & Shelter** -- plus an **Exploration & Industry** tab. **Research rate:** 5 engineers = 100%, with diminishing returns above (10 eng ≈ 130%, 25 eng ≈ 170%).
_source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

See `items/upgrades.md` for the full node-by-node tree (prerequisites, costs, effects, recommended order).

---

## Book of Laws

**status:** research-integrated

Two parallel law trees: **Adaptation** (available from the start; problem-solving laws) and **Purpose** (unlocks mid-scenario via a story trigger; branches into **Faith** OR **Order** -- mutually exclusive and **permanent** once chosen).
_source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

- **Laws cannot be repealed once signed.** Each law has a cooldown before the next can be enacted.
  _source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_
- **Faith and Order are hard-locked once Purpose is chosen** -- there is no documented edge case to switch trees mid-run.
  _source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

See `paths/adaptation_laws.md`, `paths/faith_path.md`, `paths/order_path.md` for full law lists and consequences; `items/builds.md` for strategic combinations.

---

## Expedition System

**status:** research-integrated

Expeditions are dispatched from a **Beacon** (built; requires Wood + Steel). Scout teams explore the Frostland map and return with resources, survivors, or story-relevant finds. Scout-team count is upgradeable via the Exploration & Industry tech tab (More Scouts / Additional Scouts; Lighter / Boosted Scout Sleds for speed; Automaton Scouts for the Arks).
_source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

- **Each scenario has its own Frostland variant map** -- nodes are not shared identically across scenarios. A New Home's node list (Weather Station, Winterhome, Snow Cliff, etc.) is documented in `architecture_manifest.md` Optional content registry and `sections/a_new_home.md`. The Arks crater is eye-shaped with no Outpost Depot location and a "Broken Automaton" node; The Refugees' crater has two Destroyed Steam Core Transports.
  _source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_
- **Maximum 2 Outposts per city** in A New Home; expeditions/Outposts disabled during storms; Endless has **no Outposts** and its Frostland regenerates after each storm.
  _source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

---

## Scenario Events / Timeline

**status:** research-integrated

Each scenario is a discrete, time-limited run with scripted event chains and a fixed end condition; there is no persistent overworld and no save-state shared between scenarios. Per-scenario timelines, act structures, and event triggers are documented in `sections/<scenario>.md`; ending branches in `endings/`. Cross-scenario summary:

- **A New Home:** ~48 days, 3 acts, culminating in the Great Storm (final 7 days). Weather changes always occur at **7:00**.
- **The Refugees:** ~26-30 days; refugee/Lord waves arrive ~every 2 days.
- **The Arks:** ~22-27 days; New Manchester relief arc ~day 15.
- **The Fall of Winterhome:** ~22-26 days; ~13 days to prepare evacuation after the trigger.
- **Endless:** unlimited; cyclical storms every ~10-15 days by sub-mode.
  _source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

### The Great Storm (A New Home endgame)
The final 7 days of A New Home. Temperature reaches **−150 °C** (a heat level of −13). The storm **disables Hunters, Hothouses, scouting, and the Beacon** (no food production); Coal Mines suffer the **Coal Mine Crisis** (must "air out" or they collapse), but Coal Thumpers keep working. Music changes to "The City Must Survive."
_source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 2 · category: mainline · spoiler: late-game_

---

## Difficulty Modes

**status:** research-integrated

Difficulty is set per-scenario via "Select Scenario" → Scenario Settings (A New Home defaults to Medium with no in-line difficulty choice unless you use Select Scenario). Higher difficulties reduce resource availability and increase event pressure.
_source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

- **Survivor Mode** is Frostpunk's Ironman tier: disables reload-to-undo, retaining only a single rolling autosave for crash recovery. It is required for the per-scenario "Survivor" completion achievements and also for the "Iron Man" difficulty achievements (complete a scenario on Hard in Survivor mode).
  _source: Deep Research handoff 2026-06-02 (P2 result, 3 sources) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

### Save system
_source: Deep Research handoff 2026-06-02 (P2 result, confirmed) · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

| Aspect | Behavior |
|---|---|
| Autosave | Mid-scenario on day transition (~00:00) and on quit; crash protection, not save-scumming |
| Manual save | Yes on Easy / Medium / Hard; multiple named slots, Steam-cloud synced |
| Quicksave | Yes — a separate quicksave slot exists (Easy/Medium/Hard only) |
| No save-state between scenarios | Each scenario is fully independent; no carry-over |
| Survivor mode | Single rolling autosave only; disables all reload-to-undo |
| Exit mid-scenario | Autosaves on quit |
| Endless Mode | Same save behavior as scenarios |

**Known issue:** save-corruption / CTD around late game (day 30+, 500+ population) on certain patches. Backing up the Steam `userdata\...\323190\remote\saves` folder is advised for long Survivor or Marathon/Ultramarathon runs. [Confirmed: 2 · class:community-forum]
