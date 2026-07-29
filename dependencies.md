# Dependencies -- Frostpunk
<!-- hintforge · stitch pass · last run: 2026-06-03 -->
<!-- Every stitch run re-audits ALL existing edges + adds new ones. The per-edge convergence audit (open each cited source, verify the specific value) applies to every row in this file on every run, not just new candidates. A game patch, DLC, or new ingestion phase can change facts that existing edges cite -- only a full re-audit catches that. See `stitch_and_zipper.md` Phase B "Re-run scope: always full." Inconsistencies (cited source contradicts edge text) land in the `## Corpus inconsistencies` section; the edge row stays in place. -->

## Cross-system edges

| Edge ID | System A | System B | Dependency description | Confidence | Source files |
|---------|----------|----------|------------------------|------------|--------------|
| DEP-001 | Expedition System (Tesla City Outpost) | Resource System (Steam Cores) | Tesla City Outpost in A New Home yields 1 Steam Core/day and is the **only renewable Steam Core source** in the scenario; losing it makes late-game Steam Core-dependent builds critically scarce. | high | `sections/a_new_home.md`, `mechanics.md`, `sections/missables.md`, `architecture_manifest.md` |
| DEP-002 | Law System (Purpose terminal laws) | Hope/Discontent Mechanic | Signing New Faith (Faith terminal law) or New Order (Order terminal law) **removes the Hope meter entirely** and auto-builds an Execution Platform; Hope-based management becomes impossible for the remainder of the run. Under Order, the Hope bar is replaced by an Obedience bar. | high | `paths/faith_path.md`, `paths/order_path.md`, `mechanics.md`, `sections/story_notes.md` |
| DEP-003 | Scenario Event System (Londoners crisis) | Law System (Purpose laws) | In A New Home, Purpose laws (Faith or Order) are locked until the Londoners crisis fires -- triggered by scouting Winterhome OR the day-15 messenger arriving. This event also starts the Great Storm timer. Purpose is unavailable before the trigger. | high | `sections/a_new_home.md`, `architecture_manifest.md`, `paths/faith_path.md`, `paths/order_path.md` |
| DEP-004 | Achievement System (Golden Path) | Law System (Purpose + Adaptation laws) | The Golden Path achievement requires avoiding Purpose "crossing the line" laws (Protector of Truth / Righteous Denunciation for Faith; Pledge of Loyalty / Forceful Persuasion for Order) AND avoiding Triage / Emergency-Shift abilities AND no Needs Crises AND no forbidden deaths throughout the A New Home run. Most Adaptation laws (incl. Soup, Extended Shift) are safe. | high | `endings/a_new_home_endings.md`, `paths/faith_path.md`, `paths/order_path.md`, `paths/adaptation_laws.md`, `items/builds.md`, `achievements.md` |

## PoNR / lockout edges

| Edge ID | Trigger | Locked out | Notes | Source files |
|---------|---------|------------|-------|--------------|
| PON-001 | Great Storm onset (A New Home) | Tesla City Outpost access -- Beacon disabled, all scouting terminated | Tesla City must be reached and Outpost set up **before the storm**; rushing Winterhome discovery shortens the access window by advancing the storm timer. Once the storm begins the Beacon is disabled and the outpost cannot be established. | `sections/a_new_home.md`, `sections/missables.md`, `architecture_manifest.md` |
| PON-002 | Signing a Purpose "crossing the line" law (A New Home) | Saviour ending + Golden Path achievement -- permanently blocked | Crossing-the-line laws: Protector of Truth / Righteous Denunciation (Faith); Pledge of Loyalty / Forceful Persuasion (Order). Signing any of these is irreversible. | `paths/faith_path.md`, `paths/order_path.md`, `endings/a_new_home_endings.md`, `achievements.md` |
| PON-003 | Taking the Steel Bridge automaton (Fall of Winterhome) | Iron Deposit steel outpost -- permanently blocked | The Iron Deposit is the primary steel supply needed to gather 9,000 Steel for the full Dreadnought. Taking the bridge automaton severs iron delivery, making the full Dreadnought near-impossible. | `sections/fall_of_winterhome.md`, `items/builds.md`, `endings/winterhome_endings.md`, `sections/missables.md` |
| PON-004 | Lost Dreadnought node not scouted (The Arks) | Factory blueprints -- unobtainable; Automaton production blocked; win condition blocked | The Factory is NOT researchable in The Arks; blueprints come only from the Lost Dreadnought scouting node. Without the Factory, Automatons cannot be built and the "Autonomous City" win condition cannot be met. | `sections/the_arks.md`, `sections/missables.md`, `items/upgrades.md`, `architecture_manifest.md` |
| PON-005 | On The Edge: Day-7 18:00 first shipment deadline missed | Run ends (instant game over) after a 24h last-chance window | Must send 100 Steel + 2 Steam Cores to New London by Day 7 18:00. Missing the deadline triggers a 24h last-chance warning; if still unsent, the run ends immediately. | `sections/on_the_edge.md`, `endings/on_the_edge_endings.md`, `sections/missables.md`, `architecture_manifest.md` |
| PON-006 | On The Edge: independence declared | Law signing unlocked (irreversible) | Under New London rule all law-signing is blocked (New London signs laws by edict). Declaring independence is the only way to gain full Book of Laws access; once triggered it is irreversible and law-path choices then lock as in the base game. | `sections/on_the_edge.md`, `endings/on_the_edge_endings.md` |
| PON-007 | The Last Autumn: Day-37 sea freeze | Docks + Fishing Harbour + Telegraph logistics permanently locked | Sea freezes Day 37; coal supply reduced to Charcoal Kilns only; wood to Sawmills only; steel from the Shipwreck only. If all 4 Generator construction stages are done by Day 37, early departure is available (achievement: I'll Be Home for Christmas). | `sections/the_last_autumn.md`, `sections/missables.md`, `architecture_manifest.md`, `endings/the_last_autumn_endings.md` |
| PON-008 | The Last Autumn: Worker/Engineer choice post-first-strike | Opposing Labour law branch permanently locked; one achievement gate closed per-run | Siding with Engineers → Factory Inspectorate (gates "All Along the Watchtower": convicts + engineers only). Siding with Workers → Labour Union (gates "Arise Ye Workers": workers only). The force-signed law and exclusivity are permanent. | `sections/the_last_autumn.md`, `sections/missables.md`, `achievements.md` |

## Missable / sequencing dependencies

| Edge ID | Action | Window | Consequence | Source files |
|---------|--------|--------|-------------|--------------|
| SEQ-001 | Research Advanced Steelworks (Fall of Winterhome) | Early in the scenario, before steel becomes the bottleneck | Advanced Steelworks is the priority research because the full Dreadnought retrofit costs **9,000 Steel** -- the only resource with a single building family fixed to finite deposit locations. Delaying it makes the full Dreadnought and the "Full Dreadnought" achievement unachievable in the time available. | `sections/fall_of_winterhome.md`, `items/upgrades.md`, `items/builds.md`, `endings/winterhome_endings.md`, `mechanics.md` |
| SEQ-002 | Great Storm onset (A New Home) | Final 7 days | All Coal Mines enter the **Coal Mine Crisis** and must be manually "aired out" or they collapse. Coal Thumpers remain operational and become the primary coal source during the storm. Pre-storm coal stockpiling (raw food in parallel) is the counter-strategy. | `sections/a_new_home.md`, `mechanics.md` |
| SEQ-003 | New Manchester 3rd relief shipment (The Arks) | Before scenario deadline | Sending the 3rd shipment consumes **6,000 Coal** from the city's stockpile; the own-city win gate simultaneously requires **8,000 Coal** (plus 500 Food Rations, 5 Houses, disbanding expeditions) by the same deadline. Both use the same coal reserve -- total coal needed to complete both is ≥14,000 Coal. | `sections/the_arks.md`, `endings/arks_endings.md` |

## Stitch run log

| Date | Scope | Edges written | Edges proposed (pending) | Inconsistencies surfaced | Model |
|------|-------|---------------|--------------------------|--------------------------|-------|
| 2026-06-03 | full | 15 (DEP-001–004, PON-001–008, SEQ-001–003) | 0 | 1 | sonnet-class |

<!-- Inconsistencies surfaced: count from the per-edge convergence audit (stitch_and_zipper.md Phase B). Counts must be derived by reading this file, not recalled. A non-zero count requires an explicit chat call-out and at least one populated row in the Corpus inconsistencies section below. -->

## Corpus inconsistencies

Stitch's per-edge convergence audit (see [`../../hintforge/stitch_and_zipper.md`](../../hintforge/stitch_and_zipper.md) Phase B) populates this section when a candidate edge's cited sources contradict each other. Each row records the contradiction; resolving it is the user's call (or a follow-up doctor / ingestion run). Edges blocked on an unresolved entry are NOT written to the tables above until the inconsistency is closed.

| Detected | Files | Conflicting values | Suspected authoritative source | Status |
|----------|-------|--------------------|--------------------------------|--------|
| 2026-06-03 | `architecture_manifest.md` (§Technology prerequisites, Factory row), `items/upgrades.md` (§Exploration & Industry, Factory entry) | `architecture_manifest.md` had "A New Home: scouting only" (ambiguous). `items/upgrades.md` and research inboxes p1+p2: Factory NOT available in A New Home at all. | `items/upgrades.md` | resolved 2026-06-03 -- `architecture_manifest.md` Factory row Scenario column corrected to "not available (not researchable; no fixed scouting path in ANH)" |
