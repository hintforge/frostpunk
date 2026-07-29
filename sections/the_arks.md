# The Arks -- Walkthrough

**status:** research-integrated
**last_reconciled:** 2026-06-02 (P2)

A separate base-game scenario (~22-27 days), city nicknamed "Legacy." Unlocks after surviving 20 days of A New Home. **Objective: keep the 4 Seedling Arks above freezing** while meeting your city's completion gate. An automaton-heavy scenario.

## Starting conditions & key mechanic
Start with **45 technicians (engineers), 1 automaton, 4 Seedling Arks, and 3 Steam Cores.** **No new survivors are found** (except one worker via an event) -- workforce caps at 46. Seedlings freeze if temperature drops too low (game over if any Ark falls below "chilly"); **research Heaters / Steam Hubs before the 2nd temperature drop.** Purpose laws and Children laws are absent; Adaptation tree only.
_source: Deep Research handoff 2026-06-02 (P2, 4 sources, 2 languages) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

Steam cores: start **3**, plus scouting; **new core locations spawn only after you run out** (deliberate game-design trigger). If the depletion event fires too late, some cores cannot be retrieved before the storm.
_source: Deep Research handoff 2026-06-02 (P2, 3 sources) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

## Build priority
First tech **Faster Gathering → Beacon**; then rush **Factory plans → Engineer Automatons.** Research throughput, not heat, is the win condition. No Hunters available (food via Hothouse only) -- sign **Food Additives early** (sawdust meals count for stockpile + the New Manchester shipment).
_source: Deep Research handoff 2026-06-02 (3 sources) · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

## New Manchester relief arc + win gate (endgame -- gated)
~day 15. Optional escalating shipments to a sister-city; your own win gate is 8000 Coal / 500 Rations / 5 houses / disband expeditions by deadline. Full detail (shipment amounts, both-cities best ending): `endings/arks_endings.md`.
_source: Deep Research handoff 2026-06-02 (4 sources) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 3 · category: mainline · spoiler: story_

## Frostland
The Arks crater is eye-shaped, has **no Outpost Depot location**, and yields a "Broken Automaton" node. (Outposts and Hunters' tech are both unavailable here.)
_source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

## Achievement note
**Vegetarian** is impossible here (no Hunters available = no food "choice"). See `achievements.md`.
_source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

## Ordered milestone sequence (P2)

1. **Day 1 setup** *(none)* — 45 technicians, 1 automaton, 4 Seedling Arks, 3 Steam Cores. Heat-the-Arks is the continuous fail condition.

2. **Workshop + Beacon rush** *(none)* — Research Faster Gathering → Beacon; build Beacon ~day 2. Exit: scouting available.

3. **Heat the Arks (ongoing fail condition)** *(progression)* — Research Heaters / Steam Hubs before the 2nd temperature drop. Arks must stay at ≥ "chilly" at all times.
   _source: Deep Research handoff 2026-06-02 (P2, 3 sources) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

4. **Lost Dreadnought -- Factory plans** *(progression)* — The Factory is NOT researchable in this scenario; blueprints only via the Lost Dreadnought node. Keep scouts moving toward it. PoNR: **YES** (must reach node before scenario end). `missable: yes` → `sections/missables.md`
   _source: Deep Research handoff 2026-06-02 (P2, 4 sources) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression · missable: yes_
   > **Cross-system dependency** -- see `dependencies.md` PON-004: without scouting the Lost Dreadnought, Factory blueprints are unobtainable, blocking all Automaton production and the win condition.

5. **Build the Factory** *(progression)* — Costs 30 wood / 15 steel / 1 Steam Core. PoNR: no.

6. **Autonomous City quest -- 5 Automatons** *(progression)* — Each Automaton costs 100 wood, 100 steel, 50 coal, and 1 Steam Core (reduced by Streamlined Automatons / Automaton Redesign). Build all 5 to satisfy citizens.
   _source: Deep Research handoff 2026-06-02 (P2, 4 sources) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

7. **Broken Automaton scouting event** *(progression)* — Repairing a found automaton yields a second free one (Automaton Scouts is exclusive to The Arks). Missable if not scouted.
   _source: Deep Research handoff 2026-06-02 (P2, 2 sources) · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

8. **New Manchester arc (~day 15)** *(progression)* — A messenger arrives. Optional 3-stage relief: (1) 600 wood + 600 steel + 1 automaton; (2) 2000 food rations + 2 automatons; (3) 6000 coal + 4 automatons (7 automatons total sent). Must keep ≥6 automatons working in the city for citizens. Shipments take 1 day. Optional but missable if objective-deadline pressure forces skipping. Full ending detail: `endings/arks_endings.md`.
   > **Cross-system dependency** -- see `dependencies.md` SEQ-003: the 3rd shipment requires 6,000 Coal from the city stockpile; your own win gate simultaneously requires 8,000 Coal by the same deadline.
   _source: Deep Research handoff 2026-06-02 (P2, 4 sources) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

9. **Storm-prep hard deadline** *(progression)* — Build 5 Houses; disband all expeditions/outposts; gather **8000 Coal**; gather **500 Food Rations**. PoNR: **YES** (endgame).
   _source: Deep Research handoff 2026-06-02 (P2, 3 sources) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

10. **Ending -- text evaluation** *(late-game)* — Scenario ends the moment objectives are met; the player does NOT play through the storm (text evaluation screen). No Outposts exist in The Arks (eye-shaped crater, no Outpost Depot site). PoNR: **YES**.
    _source: Deep Research handoff 2026-06-02 (P2, 4 sources) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 2 · category: mainline · spoiler: late-game_

## See also
- Builds: `items/builds.md` (The Arks) · Endings: `endings/arks_endings.md` · Tech: `items/upgrades.md` (Automaton line)

---

## Sources
- frostpunk.fandom.com (The Arks); namu.wiki (KR); Steam Community guides. Deep Research handoff, 2026-06-02.
