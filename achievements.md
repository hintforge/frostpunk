# Frostpunk -- Achievements

**status:** research-integrated
**last_reconciled:** 2026-06-03 (P3)
**stub_source:** Steam (via vgtimes.com)
**stub_fetched:** 2026-06-02

## Why this file exists

The corpus's single source of truth for "what achievements does this game have, and what do I need for each one." The reader consults it for any achievement-class question.

**Coverage summary:** 115 stubs total -- **115 resolved** (P1 2026-06-02: 53 base-game; P3 2026-06-03: 62 closures -- 26 DLC, 11 scope-confirmed OTE, 25 base-game trigger gaps. Two previously-deferred items were already partially resolved at P1: Central Heating in Mastery; Builder in DLC.)

**Platform note:** Steam / PC total = 115 achievements. TrueAchievements shows higher per-pack counts (TLA pack 20/405 GS, OTE 20) vs Console Edition (13/195 GS each); triggers are identical across platforms.

**Genre vocabulary:** no `genre:` overlays used in this corpus (Frostpunk achievements map cleanly to the universal `trigger_type` axis).

> Hidden achievements keep their full name + trigger here; the read-time renderer gates the *name* below the appropriate tier per `warning_tiers.md`. All triggers carry `_source: Deep Research handoff 2026-06-02_` (P1 base-game) or `_source: Deep Research P3 handoff 2026-06-03_` (DLC and gap closures) unless noted.

> **Two historically-buggy achievements -- QA note:** "Not great, not terrible" (also counts Dangerous workplaces per a known bug; avoid Dangerous too) and "A for Effort" (was unobtainable at launch; re-verify against current patch before treating as freely earnable).

---

## Progression

Every player reaching the relevant point gets these (no non-default choice required).

| Achievement | Scope | Trigger | Missable | PoNR | Vector binding | Status |
|---|---|---|---|---|---|---|
| Leader | Base | Finish A New Home | no | — | `sections/a_new_home.md` | resolved P1 |
| Refugee | Base | Finish The Refugees | no | — | `sections/the_refugees.md` | resolved P1 |
| Technocrat | Base | Finish The Arks | no | — | `sections/the_arks.md` | resolved P1 |
| Winterhome | Base | Finish The Fall of Winterhome | no | — | `sections/fall_of_winterhome.md` | resolved P1 |
| Built to Serve | Base | Build an Automaton | no | — | `items/upgrades.md` (Factory) | resolved P1 |
| The Scientific Method, vol. 1 _(hidden)_ | Base | Finish the Automaton Project (research line) | no | — | `items/upgrades.md` (Automaton line) | resolved P1 |
| This is New London, Over | DLC: OTE | Contact New London (build Admin + Transport Depot + clear road to Warehouse) | no | — | `sections/on_the_edge.md` | resolved P3 |
| Builder | DLC: TLA | Build the Generator in The Last Autumn scenario (win the scenario) | no | — | `sections/the_last_autumn.md` | resolved P3 |
| First Steps | DLC: OTE | Build a Safe Route (functionally required to finish OTE) | no | — | `sections/on_the_edge.md` | resolved P3 |
| Once More unto the Breach | Base / Multi | Provide an amputee with a prosthesis (prosthesis available via telegraph or expeditions) | no | — | `mechanics.md` (Expeditions) | resolved P3 |

---

## Branch

Getting these requires a non-default choice or excludes another outcome.

| Achievement | Scope | Trigger | Missable | PoNR | Vector binding | Status |
|---|---|---|---|---|---|---|
| The Saviour | Base | Finish A New Home on the humane path (no Purpose "crossing the line" laws) | yes | crossing-the-line law signing | `endings/a_new_home_endings.md` | resolved P1 |
| The Iron Saviour | Base | Finish A New Home having signed New Faith or New Order | yes | depends on Purpose endgame | `endings/a_new_home_endings.md` | resolved P1 |
| Everybody Lived for Once | Base | The Arks: save both cities (New Manchester + own) | yes | by deadline | `endings/arks_endings.md` | resolved P1 |
| The Union | Base | The Refugees: accept all Lords, reach optimal reconciliation ending | yes | end of run | `endings/refugees_endings.md` | resolved P1 |
| United _(hidden)_ | Base | A New Home: nobody leaves for London | yes | Londoners departure event | `sections/a_new_home.md` | resolved P1 |
| Banksy _(hidden)_ | Base | A New Home: resolve Londoners' graffiti peacefully (guards/faith keepers, no punishment) | yes | the graffiti event | `sections/a_new_home.md` | resolved P1 |
| Negotiator _(hidden)_ | Base | A New Home: resolve Londoners' thievery peacefully (Hope ≥ ~50%) | yes | the thievery event | `sections/a_new_home.md` | resolved P1 |
| My Turn to Speak _(hidden)_ | Base | A New Home: let Londoners speak, then have the last word | yes | the confrontation event | `sections/a_new_home.md` | resolved P1 |
| Politician | Base | Stay in power after a political threat | yes | the threat event | `sections/a_new_home.md` | resolved P1 |
| The Scientific Method, vol. 2 _(hidden)_ | Base | Improve Radical Treatment (law-branch choice) | yes | Radical Treatment line | `paths/adaptation_laws.md` | resolved P1 |
| All Along the Watchtower | DLC: TLA | Build Generator with only convicts and engineers left at end (side with Engineers after first strike; minimize worker recruitment) | yes | post-first-strike choice (PoNR) | `sections/the_last_autumn.md` | resolved P3 |
| Arise Ye Workers | DLC: TLA | Build Generator with only workers left at end (side with Workers after first strike; minimize engineer recruitment) | yes | post-first-strike choice (PoNR) | `sections/the_last_autumn.md` | resolved P3 |
| It Was Me All Along | DLC: TLA | Find generator parts meant for Winterhome (Lost Crates) and keep them; do not return to base before meeting the convoy | yes | yes (return to base locks out return) | `sections/the_last_autumn.md` | resolved P3 |
| Unforgiven _(hidden)_ | DLC: OTE | Let New London fall (final binary choice) | yes | yes (final choice PoNR) | `endings/on_the_edge_endings.md` | resolved P3 |
| We Are In This Together _(hidden)_ | DLC: OTE | Save New London (final binary choice) | yes | yes (final choice PoNR) | `endings/on_the_edge_endings.md` | resolved P3 |
| Social Activist | DLC: OTE | Make all other settlements loyal at scenario end (excludes Slave Driver) | yes | end of run | `sections/on_the_edge.md` | resolved P3 |
| Slave Driver | DLC: OTE | Make all other settlements distrustful at scenario end (excludes Social Activist) | yes | end of run | `sections/on_the_edge.md` | resolved P3 |
| Endless Social Activist | Endless | Make all 3 settlements loyal in Endless mode | yes | end of run | `sections/endless_mode.md` | resolved P3 |
| Endless Slave Driver | Endless | Make all 3 settlements distrustful in Endless mode (4 negative actions each; unlocks 1 day after full distrustful) | yes | end of run | `sections/endless_mode.md` | resolved P3 |

---

## Mastery

Skill or self-imposed restriction beyond normal play.

| Achievement | Scope | Trigger | Missable | PoNR | Vector binding | Status |
|---|---|---|---|---|---|---|
| Iron Man (New Home) | Base | Finish A New Home in Iron Man mode (Hard, no reloads) | yes | whole run | `mechanics.md` (Difficulty) | resolved P1 |
| Iron Man (Refugees) | Base | Finish The Refugees in Iron Man mode | yes | whole run | `mechanics.md` (Difficulty) | resolved P1 |
| Iron Man (The Arks) | Base | Finish The Arks in Iron Man mode | yes | whole run | `mechanics.md` (Difficulty) | resolved P1 |
| Iron Man (Fall of Winterhome) | Base | Finish Winterhome in Iron Man mode | yes | whole run | `mechanics.md` (Difficulty) | resolved P1 |
| New Home Survivor | Base | Finish A New Home in Survivor Mode | yes | whole run | `mechanics.md` (Difficulty) | resolved P1 |
| Refugees Survivor | Base | Finish The Refugees in Survivor Mode | yes | whole run | `mechanics.md` (Difficulty) | resolved P1 |
| The Arks Survivor | Base | Finish The Arks in Survivor Mode | yes | whole run | `mechanics.md` (Difficulty) | resolved P1 |
| The Winterhome Survivor | Base | Finish Winterhome in Survivor Mode | yes | whole run | `mechanics.md` (Difficulty) | resolved P1 |
| Golden Path _(hidden)_ | Base | Finish A New Home without severe laws/harsh abilities, no Needs Crisis, no forbidden deaths (Soup/Extended Shift safe; Triage/Emergency-Shift forbidden) | yes | whole run | `endings/a_new_home_endings.md`, `items/builds.md` | resolved P1 |
| Sprinter _(hidden)_ | Base | The Arks: find New Manchester before Day 15 | yes | Day 15 | `endings/arks_endings.md`, `sections/missables.md` | resolved P1 |
| Vegetarian | Base | Finish a scenario using only Hothouses (food). **Unreachable in The Arks** (no food choice). | yes | end of run | `sections/the_arks.md` (unreachable note) | resolved P1 |
| Carnivore | Base | Finish a scenario using only Hunters (food). **Unreachable in The Arks.** | yes | end of run | `sections/the_arks.md` | resolved P1 |
| Worse than London | Base | Finish without building a House or Bunkhouse (all tents) | yes | end of run | `items/upgrades.md` (housing) | resolved P1 |
| Better than London | Base | Finish without building a Tent | yes | end of run | `items/upgrades.md` (housing) | resolved P1 |
| Tis but a Scratch | Base | Finish without building an Infirmary or House of Healing | yes | end of run | `items/upgrades.md` (health) | resolved P1 |
| Bad at Politics | Base | Keep all your promises in a run | yes | end of run | `sections/a_new_home.md` | resolved P1 |
| Marathon Hard | Endless | Survive the Marathon (50-day Endurance) duration on Hard | yes | run end | `sections/endless_mode.md` | resolved P1 |
| Ultramarathon Hard | Endless | Survive the Ultramarathon (100-day Endurance) on Hard | yes | run end | `sections/endless_mode.md` | resolved P1 |
| Marathon Extreme | Endless | Survive the Marathon duration on Extreme | yes | run end | `sections/endless_mode.md` | resolved P1 |
| Ultramarathon Extreme | Endless | Survive the Ultramarathon duration on Extreme | yes | run end | `sections/endless_mode.md` | resolved P1 |
| The Last Autumn Survivor | DLC: TLA | Build the Generator in Survivor mode | yes | whole run | `sections/the_last_autumn.md` | resolved P3 |
| Iron Man (The Last Autumn) | DLC: TLA | Build the Generator on Hard difficulty | yes | whole run | `sections/the_last_autumn.md` | resolved P3 |
| Iron Man (On The Edge) | DLC: OTE | Finish On The Edge on Hard difficulty | yes | whole run | `sections/on_the_edge.md` | resolved P3 |
| On the Edge Survivor | DLC: OTE | Finish On The Edge in Survivor mode | yes | whole run | `sections/on_the_edge.md` | resolved P3 |
| Perfectionist | DLC: TLA | Build Generator with all 3 upgrades and zero construction faults (failed disaster choices cause permanent faults) | yes | no (but faults are permanent per choice) | `sections/the_last_autumn.md` | resolved P3 |
| I'll Be Home for Christmas | DLC: TLA | Build the Generator (all 4 stages) before the Day-37 last shipment (sea freeze) | yes | yes (Day 37) | `sections/the_last_autumn.md` | resolved P3 |
| Bonus Pater Familias | DLC: TLA | Build the Generator without anyone dying | yes | no | `sections/the_last_autumn.md` | resolved P3 |
| No Crunch | DLC: TLA | Build Generator using neither Two Shifts nor Extended Shifts (must sign one but not use it) | no | no | `sections/the_last_autumn.md` | resolved P3 |
| Ducks in a Row | DLC: TLA | Build Generator without any pause >24h between part construction stages | no | no | `sections/the_last_autumn.md` | resolved P3 |
| Not great, not terrible | DLC: TLA | Build Generator employing people in neither Safe nor Deadly workplaces. **Bug:** also avoid Dangerous (the bug counts it as out-of-bounds; verify against current patch) | no | no | `sections/the_last_autumn.md` | resolved P3 (bug-noted) |
| Fisher King | DLC: TLA | Build the Generator without setting up any Foragers' Camps (Foragers' Quarters and scouting allowed) | no | no | `sections/the_last_autumn.md` | resolved P3 |
| Emissions Reduction | DLC: TLA | Build Generator using no Coal-consuming buildings (Foundry coal is allowed; no Ventilation Plants, no Bath House) | no | no | `sections/the_last_autumn.md` | resolved P3 |
| Unskilled Labour | Base / Multi | Finish a scenario without constructing any Steam or Advanced buildings (standard houses, infirmaries, etc. are allowed) | yes | end of run | `mechanics.md` | resolved P3 |
| Charcoaled | Base / Multi | Finish a scenario with Charcoal Kilns as the only coal-providing buildings (piles, gathering, outposts allowed) | no | no | `mechanics.md` | resolved P3 |
| Satellites | Base / Multi | Finish a scenario without ever expanding the Generator's range (don't research any Range Upgrade). Not possible in TLA/OTE (no generator range line) | yes | no | `items/upgrades.md` (Heating) | resolved P3 |
| Central Heating | Base / Multi | Finish a scenario without building a single Steam Hub. **Not possible in TLA/OTE** (no Generator to hub-extend). | no | no | `items/upgrades.md` (Heating) | resolved P1 |
| Notting Hollow | Base / Endless | Have over 600 population living in Houses only (no Tents or Bunkhouses) | no | no | `items/upgrades.md` (housing) | resolved P3 |
| By the Sweat of their Brow | Endless | Survive 75 days in Endless without building any Automatons (Serenity-friendly) | no | no | `sections/endless_mode.md` | resolved P3 |

---

## Collection

Complete a finite, enumerable set in full.

| Achievement | Scope | Trigger | Missable | PoNR | Vector binding | Status |
|---|---|---|---|---|---|---|
| Conservationist | Base | The Arks: save all 4 Seedling Arks | yes | by storm | `endings/arks_endings.md` | resolved P1 |
| Compassionate _(hidden)_ | Base | A New Home: accept all refugee groups | yes | last refugee group | `sections/a_new_home.md` | resolved P1 |
| Lost Souls _(hidden)_ | Base | A New Home: save every person in the Frostland (~691 pop) | yes | before storm | `sections/a_new_home.md` | resolved P1 |
| Search and Rescue | Base | Rescue all arrivals in The Refugees | yes | last arrival | `sections/the_refugees.md` | resolved P1 |
| All children on board | Base | Winterhome: evacuate all children | yes | Dreadnought launch | `endings/winterhome_endings.md` | resolved P1 |
| Full Dreadnought | Base | Winterhome: fully upgrade **and** fill the Dreadnought | yes | Dreadnought launch | `endings/winterhome_endings.md` | resolved P1 |
| Power Overwhelming | Base | Fully upgrade the Generator (power + range + overdrive -- all research nodes) | no | — | `items/upgrades.md` (Heating) | resolved P1 |
| Master Archivist | Endless | Collect all Relics in Endless mode (require scouting + building Archives) | yes | run end | `sections/endless_mode.md` | resolved P1 |
| Advanced Designs | Base / Multi | Have an Advanced Coal Mine, Advanced Wall Drill, and Advanced Steelworks working simultaneously | no | — | `items/upgrades.md` | resolved P3 |
| Bald Mountain | DLC: OTE | Cut down all trees in Outpost 11 (cliff trees don't count) | no | — | `sections/on_the_edge.md` | resolved P3 |
| Green Thumb | DLC: OTE | Complete all improvements in Hot Springs settlement | yes | before scenario end | `sections/on_the_edge.md` | resolved P3 |
| Defender of the Oppressed | DLC: OTE | Complete all improvements in Shipwreck Camp settlement | yes | before scenario end | `sections/on_the_edge.md` | resolved P3 |
| Guardian | DLC: OTE | Complete all improvements in Children's Mine settlement | yes | before scenario end | `sections/on_the_edge.md` | resolved P3 |
| Contractor | DLC: OTE | Develop all three settlements to the highest level | yes | before scenario end | `sections/on_the_edge.md` | resolved P3 |
| All Your Base Are Connect To Us _(hidden)_ | DLC: OTE | Build all Safe Routes (all 3 settlements connected) | yes | before scenario end | `sections/on_the_edge.md` | resolved P3 |
| Frostland Explorer | DLC: OTE | Explore all Frostland sites in On The Edge (including safe-route sites; requires Safe Routes) | yes | before scenario end | `sections/on_the_edge.md` | resolved P3 |
| Hyde Park Corner | Endless | Have a Town Square of each size in Endless mode | no | — | `sections/endless_mode.md` | resolved P3 |
| Walk on the Grass | Endless | Have a Garden of each size in Endless mode | no | — | `sections/endless_mode.md` | resolved P3 |
| There was no Waldo | Endless | Explore all Frostland sites between storms in Endless mode (every named variant; cumulative across multiple runs) | no | — | `sections/endless_mode.md` | resolved P3 |
| A Tomb for Memories | Endless | Build the Archives building in Endless mode (requires obtaining a relic from scouting first) | no | — | `sections/endless_mode.md` | resolved P3 |

---

## Threshold

Cumulative count, no finite-set ceiling.

| Achievement | Scope | Trigger | Missable | PoNR | Vector binding | Status |
|---|---|---|---|---|---|---|
| Expats | Base | Set up 2 Outposts in one playthrough. **Unreachable in The Arks / Winterhome** (no Outpost Depot). | no | — | `mechanics.md` (Expeditions) | resolved P1 |
| Oxbridge | Base | Have 4 Workshops researching simultaneously | no | — | `mechanics.md` (Tech Tree) | resolved P1 |
| Shai Hulud Summoner | Base | Have 4 Coal Thumpers working at once | no | — | `mechanics.md` (Coal) | resolved P1 |
| Urban Planner | Base | 300 people in one Steam Hub heat zone | no | — | `mechanics.md` (Heat) | resolved P1 |
| Bread and Games | Base | 200+ pop, all with Public House + Fighting Arena access | no | — | `paths/adaptation_laws.md` | resolved P1 |
| Autonomous City | Base | 200+ pop, automatons in more than half of workplaces | no | — | `items/upgrades.md` (Automatons) | resolved P1 |
| Promised Land | Base | Reach max Hope with no Discontent | no | — | `mechanics.md` (Hope/Discontent) | resolved P1 |
| Marathon Medium | Endless | Survive the Marathon (50-day Endurance) duration on Medium | yes | run end | `sections/endless_mode.md` | resolved P1 |
| Ultramarathon Medium | Endless | Survive the Ultramarathon (100-day Endurance) on Medium | yes | run end | `sections/endless_mode.md` | resolved P1 |
| On the Waterfront | DLC: TLA | Have 4 Advanced Docks and 12 Reloading Stations working simultaneously | no | — | `sections/the_last_autumn.md` | resolved P3 |
| Messrs Gabriel | DLC: TLA | Use the Telegraph Station 20 or more times | no | — | `sections/the_last_autumn.md` | resolved P3 |
| City of Steam | Base / Multi | Have 15 Automatons working simultaneously (best in Arks or ANH with full Factory line) | no | — | `items/upgrades.md` (Automatons) | resolved P3 |
| City of Man | Base / Multi | Have more than 650 people in the city at once (best achieved in A New Home or The Refugees) | no | — | `mechanics.md` (Population) | resolved P3 |
| Hyperefficient | Base / Multi | Have a workplace with efficiency above 200% (easiest via Builders DLC Rush Construction) | no | — | `mechanics.md` / `sections/endless_mode.md` | resolved P3 |
| Full House | Endless | Have over 700 population in Endless mode (Serenity or Settlements enabled) | no | — | `sections/endless_mode.md` | resolved P3 |
| Let There Be Light | Endless | Build 10 Street Lamps in Endless mode | no | — | `sections/endless_mode.md` | resolved P3 |
| Backup Plan | Endless | Stockpile 35,000 Coal and 10,000 Food Rations (Endless mode only) | no | — | `sections/endless_mode.md` | resolved P3 |
| Rise of the Machines | Base / Multi | Have 20 working Automatons simultaneously (hidden; needs 21+ Steam Cores total) | no | — | `items/upgrades.md` (Automatons) | resolved P3 |

---

## Discovery

Found only by deliberate exploration of non-obvious mechanics or obscure hints. Most carry the platform's hidden flag.

| Achievement | Scope | Trigger | Missable | PoNR | Vector binding | Status |
|---|---|---|---|---|---|---|
| Hi Marek! _(hidden)_ | Endless (Serenity) | Lose in Serenity mode by overdriving the generator until it explodes | no | — | `sections/endless_mode.md` | resolved P3 |
| Unknown Ship _(hidden)_ | Base: Refugees | Find the unknown ship in the Frostland (hidden scouting node in The Refugees) | yes | before scenario end | `sections/the_refugees.md` | resolved P3 |
| I Feel Lucky _(hidden)_ | DLC: OTE | Always take the risky choice at all three Frostland events: Tesla City (search for resources), Steel Bridge (Stop them / Chase them away), AND escort survivors at Victims Colony. Scouts dying does NOT void it. | yes | while sites are scoutable | `sections/on_the_edge.md` | resolved P3 |
| You Had To Do It _(hidden)_ | DLC: OTE | Rename Outpost 11 to "New London" (can be done at any point before scenario end) | yes | before scenario end | `sections/on_the_edge.md` | resolved P3 |
| I See Friends Holding Hands | Endless (Settlements) | Have an ally settlement send Emergency Aid to another settlement (non-obvious inter-settlement interaction) | no | — | `sections/endless_mode.md` | resolved P3 |
| Please, Sir, I Want Some More _(hidden)_ | Base: ANH | After signing Child Labour, give child workers extra rations (hidden follow-on action) | yes | while Child Labour is in effect | `paths/adaptation_laws.md` | resolved P3 |

---

## Builders DLC (Endless mode)

Achievements tied to the Builders endless sub-mode (requires The Last Autumn DLC). Start with a destroyed Generator; blizzards reset construction progress.

| Achievement | Trigger | Missable | PoNR | Vector binding | Status |
|---|---|---|---|---|---|
| A for Effort | Build a Generator with ALL construction faults in Builders mode (historically buggy; re-verify vs current patch) | no | — | `sections/endless_mode.md` | resolved P3 (bug-noted) |
| One More Day Syndrome | Build the Generator and then reach Day 100 in Builders mode | no | — | `sections/endless_mode.md` | resolved P3 |
| Winter Ready | Build the Generator before the weather changes in Builders mode | no | — | `sections/endless_mode.md` | resolved P3 |
| Weathering the Storm | Build the Generator in Builders mode with no storm damage | no | — | `sections/endless_mode.md` | resolved P3 |

---

## Sources

- https://vgtimes.com/games/frostpunk/achievements-and-trophies/ (fetched 2026-06-02 -- rung 3; stub source)
- https://steamcommunity.com/stats/323190/achievements (canonical; not directly fetched)
- frostpunk.fandom.com (Achievements page + per-scenario pages)
- TrueAchievements (individual achievement pages -- trigger details, PC/Console pack comparison)
- Exophase.com (trigger corroboration)
- Steam Community achievement guides ("Achievements by Map"; "Organised by Scenario"; Solo guide)
- namu.wiki (KR); readonly.wiki (mirror)
- PSNProfiles (TLA, OTE trophy guides)
- Deep Research handoffs: P1 2026-06-02 · P3 2026-06-03
