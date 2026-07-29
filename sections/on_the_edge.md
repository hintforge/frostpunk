# On The Edge -- Scenario Reference

**status:** research-integrated
**last_reconciled:** 2026-06-03 (P3)
**dlc:** On The Edge
**scope:** DLC post-game -- manage Outpost 11 after the events of A New Home

---

## Overview

Post-game scenario set after A New Home. The player leads Outpost 11, established beside a discovered Army Warehouse full of steel and steam cores. New London demands shipments of steel and cores in exchange for raw food (the only food source available), but short-changes the outpost, leading to independence and inter-settlement diplomacy with three discovered trading settlements.

Independently accessible -- completing A New Home is NOT required to play On The Edge (only owning the DLC is required). Narratively follows A New Home and references The Last Autumn's convicts.

_source: Deep Research P3 handoff 2026-06-03 (5+ sources: fandom OTE, PSNProfiles, Hey Poor Player, Gamer Terra, Speculiction) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none · dlc: on_the_edge_

### Starting conditions

| Difficulty | Workers | Engineers | Coal | Wood | Steel | Raw Food | Steam Cores |
|---|---|---|---|---|---|---|---|
| Easy | 50 | 15 | 120 | 60 | 30 | 60 | 0 |
| Medium | 50 | 15 | 60 | 30 | 10 | 40 | 0 |
| Hard | 50 | 15 | 30 | 20 | 10 | 30 | 0 |
| Extreme | 50 | 15 | 0 | 0 | 0 | 30 | 0 |

0 Automatons, 0 Children at start. Raw Food **cannot be gathered locally** -- trade is the only source.

_source: Deep Research P3 handoff 2026-06-03 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none · dlc: on_the_edge_

---

## Unique mechanics

_source: Deep Research P3 handoff 2026-06-03 (fandom, PSNProfiles, Neoseeker) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression · dlc: on_the_edge_

- **No Generator** -- heat comes from researched **Braziers** (small radius, no automaton recharge, ~3 coal/h). Automatons are buildable but functionally useless (no automaton-recharge infrastructure).
- **Army Warehouse** -- infinite Steel + Steam Cores; upgraded via new techs (Handcarts +20% output, Wooden Support ability). Replaces Steelworks / Wall-Drill tech branch.
- **Settlements + Favours + Relations** -- up to 3 trading settlements discovered via scouting: **Hot Springs** (south, raw food), **Shipwreck Camp** (east, wood), **Children's Mine** (west, coal). Each has Favour (Low → Average → High, auto-rises over time) and Relations (distrustful → neutral → loyal) driven by trades, improvements, requests, and events.
- **Safe Routes + Construction Teams** -- new unit type builds Trading Depots and Safe Routes connecting settlements.
- **Diplomacy / Trade** -- request goods, develop settlements, or trade resources; final-act loyal allies auto-send Coal / Workers / Food shipments.
- **Law signing blocked under New London rule** -- New London signs laws by edict (Emergency Shift, Extended Shift, Food Additives/Soup, Public House/Fighting Arena, Radical Treatment, Cemetery/Corpse Disposal via favour requests). Full law control returns only after declaring independence.

### Law books

- **Adaptation laws**: present, but NO signing until independence is declared.
- **Purpose laws (Faith/Order)**: ABSENT (like The Arks).

### Technology tree

- **Heating tab**: Generator line replaced by Braziers branch (Radiator Extensions, Improved Blowers, Efficient / Advanced Burners).
- **Resources tab**: Steelworks / Wall-Drill line replaced by Army Warehouse development techs (Handcarts, Wooden Support); Outpost Depot and Stereoscopic Lenses unavailable.
- Other tabs: same as base game.

_source: Deep Research P3 handoff 2026-06-03 (game-vault tech tree, Neoseeker, PSNProfiles) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression · dlc: on_the_edge_

### Resource supply model

Raw Food: trade-only (cannot be gathered). Wood: sharply limited. Steel + Steam Cores: effectively infinite from the Warehouse. No new resource types vs base game, but supply model is inverted.

### Unique buildings

Outpost Administration, Transport Depot, Trading Depots (one per settlement), Braziers, Army Warehouse, Safe Routes.
_source: Deep Research P3 handoff 2026-06-03 (fandom Quests, Neoseeker) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none · dlc: on_the_edge_

---

## Milestone sequence

_source: Deep Research P3 handoff 2026-06-03 (fandom Quests, PSNProfiles, Steam discussions) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression · dlc: on_the_edge_

1. **Establish the operation (Day 1).** Rebuild Transport Depot, build Outpost Administration, clear road to Warehouse. Exit: New London auto-contacts you (achievement "This is New London, Over"); New London sends children + clerks shortly after. PoNR: No.

2. **Send the first shipment (≤ Day 7, 18:00).** Gather + send 100 Steel and 2 Steam Cores. **Hard gate:** missing the deadline triggers a "Last chance to send the shipment" 24h warning; if still unsent → instant game over. **Delaying to the last minute grants Emergency Shift + Extended Shift laws for free via New London edict.** PoNR: **YES** (loss if unsent). `spoiler: progression`
   > **Cross-system dependency** -- see `dependencies.md` PON-005: missing the Day-7 shipment deadline is the run's earliest hard PoNR; 24h last-chance then instant game over.

3. **Continue shipments to New London.** Repeat 100 Steel + 2 Steam Cores shipments while in contact. New London returns Raw Food. PoNR: No.

4. **We need food.** Once New London only returns raw food for shipments: establish a Trading Depot at Hot Springs, form a Construction Team, find a stable Frostland food source. PoNR: No.

5. **Hot Springs contact (~Day 9–13).** Ask Hot Springs for help -- the food lifeline. Build a Safe Route and Trading Depot there. PoNR: No.

6. **Independence / split from New London.** New London demands the Hot Springs food supply; citizens riot against the clerks. Whatever is decided, New London cuts communications -- **after a short delay the full Book of Laws becomes available.** PoNR: **YES** (irreversible; law-path choices then lock as in base game). `spoiler: story`
   > **Cross-system dependency** -- see `dependencies.md` PON-006: declaring independence is the only way to unlock the Book of Laws in OTE; under New London rule, law signing is blocked (New London signs laws by edict instead).

7. **Confrontation (19-day timer).** Scout Frostland for the other settlements (Shipwreck Camp, Children's Mine) and wait for New London's response. PoNR: No.

8. **Build Trading Depots at Shipwreck Camp and Children's Mine** (after scouting each). Develop settlements via improvements (drives Relations toward loyal or distrustful). "First Steps" achievement on first Safe Route. PoNR: No.

9. **Build all Safe Routes.** Achievement "All Your Base Are Connect To Us." Enables full settlement support network. PoNR: No.

10. **Decide the fate of New London (12h timer).** The "punitive expedition" turns out to be refugees fleeing a New London disaster; New London asks for rescue. Consult Shipwreck Camp, Hot Springs, Children's Mine, then answer. PoNR: **YES** (binary final choice). `spoiler: late-game`

11a. **Save New London (5-day timer).** Send Coal, Workers, building materials (Steel + Steam Cores), Food. Loyal allies auto-send Coal / Workers / Food, leaving only steel + cores to you. Achievement "We Are In This Together." PoNR endpoint. `spoiler: late-game`

11b. **Let New London fall (5-day timer).** Prepare for refugee waves: 5 working Infirmaries, +20 Bunkhouses / Houses (built after the decision; tent upgrades count), 200 Food Rations, all housing Cold-or-warmer, no homeless. Achievement "Unforgiven." PoNR endpoint. `spoiler: late-game`

---

## Missables

_source: Deep Research P3 handoff 2026-06-03 (fandom, PSNProfiles, Steam guides) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression · dlc: on_the_edge · missable: yes_

- **Emergency Shift + Extended Shift (free laws)** -- only granted if you delay the first shipment to ~Day 7–8 18:00. Missed if you ship early. Not directly achievement-linked.
- **"I Feel Lucky" (achievement, hidden)** -- take the risky choice at Tesla City (search for resources), Steel Bridge (Stop them / Chase them away), AND escort survivors at Victims Colony. Scouts dying does NOT void it. Deadline: while sites are scoutable. `spoiler: progression`
- **"You Had To Do It" (achievement, hidden)** -- rename Outpost 11 to "New London." Can be done anytime before scenario end. `spoiler: none`
- **Settlement-improvement achievements** (Green Thumb, Defender of the Oppressed, Guardian, Contractor) -- require completing all improvements at each settlement before scenario end; favour mismanagement can soft-lock these in a run. `spoiler: progression`
- **"Social Activist" vs "Slave Driver"** -- mutually exclusive in a single run (all settlements loyal vs all distrustful); awarded only at scenario end.
- **"Frostland Explorer"** -- explore all Frostland sites including safe-route sites; must not miss any during the run.
- **Law-path locks** post-independence -- choosing e.g. Child Shelters vs Child Labor permanently locks the other. Deadline: independence.
- **"We Are In This Together" vs "Unforgiven"** -- mutually exclusive per run (Save vs Let Fall New London). Both are hard PoNR: **YES.**

See also `sections/missables.md` for the cross-scenario aggregated list.

---

## Locks & Keys (delta from base game)

_source: Deep Research P3 handoff 2026-06-03 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none · dlc: on_the_edge_

| Item | Prerequisite (delta) | Type |
|---|---|---|
| Any player-signed law | Declare independence from New London | Law system unlock |
| New London edict laws (Emergency/Extended Shift, etc.) | Contact New London / delay shipments / favour requests | Law (edict -- automatic) |
| Braziers branch | Replaces Generator / Steam-Hub heating entirely | Tech |
| Army Warehouse upgrades (Handcarts, Wooden Support) | Replace Steelworks / Wall-Drill branch | Tech |
| Trading Depot at a settlement | Scout that settlement + Construction Team | Building |
| Safe Routes | Construction Team | Building |
| Save / Let-Fall final quests | Complete Confrontation + consult all settlements | Scenario branch |

---

## Sources

- frostpunk.fandom.com (On The Edge, New London (Settlement), Quests)
- PSNProfiles, Neoseeker (walkthrough + trophy guides)
- frostpunk.game-vault.net (tech tree)
- Hey Poor Player, Gamer Terra, Speculiction, Twin Cities Geek (overview reviews)
- Steam Community guides (achievement triggers)
- TrueAchievements, Exophase (achievement details)

P3 Deep Research handoff, 2026-06-03.
