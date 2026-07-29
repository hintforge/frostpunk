# A New Home -- Walkthrough

**status:** research-integrated
**last_reconciled:** 2026-06-02 (P2)

The main campaign (~48 days). Found and lead New London; survive the **Great Storm**. Available from the start. Surviving 20 days here unlocks The Arks and The Refugees.

## Act structure
Three acts:
- **Act 1 -- early survival (days 1-~14):** establish heat, coal, wood, food, housing.
- **Act 2 -- the Londoners crisis (~day 14-15):** triggered by scouting Winterhome **OR** by the day-15 messenger. Forces the **Faith / Order** Purpose choice.
- **Act 3 -- the Great Storm (final 7 days):** the endgame survival test.

Storm timing is **action-gated**: Londoners begin ~day 14.5 or when Winterhome is scouted; the storm follows a fixed offset. The **latest the storm can hit without exploits is day 43**; it can arrive much earlier if you rush Winterhome or clear the Londoners early. **Weather changes always occur at 7:00.**
_source: Deep Research handoff 2026-06-02 (4 sources, 2 languages) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

## The Great Storm (endgame)
Final 7 days. Temperature reaches **−150 °C** (heat level −13). Disables Hunters, Hothouses, scouting, and the Beacon; **Coal Mines suffer the Coal Mine Crisis** (must "air out" or collapse), but **Coal Thumpers keep working.** Music changes to "The City Must Survive."
_source: Deep Research handoff 2026-06-02 (4 sources) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 2 · category: mainline · spoiler: late-game_

**Pre-storm prep:** complete Generator Power III + Range III + Overdrive Couplings + Advanced Heaters + Safety Bypass; max-upgraded Infirmary is the warmest building. See `items/builds.md`.
> **Cross-system dependency** -- see `dependencies.md` SEQ-002: Great Storm onset triggers the Coal Mine Crisis (all Coal Mines must be aired out or collapse); Coal Thumpers remain the only large-scale coal source during the storm.
_source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 2 · category: mainline · spoiler: late-game_

## Frostland expeditions
Key nodes and yields (full registry in `architecture_manifest.md`):
- **Weather Station** → unlocks Winterhome + Coal Mine; yields 91 coal + 1 steam core.
- **Winterhome** → unlocks the 'We're On Our Own' Purpose-law trigger; reveals Snow Cliff + American Camp.
- **Snow Cliff** → 98 rations, 61 wood, 1 steam core; reveals Shrouded Cave + Freshwater Springs.
- **Freshwater Springs** → 7 children + 22 workers; reveals Frozen Grove.
- **Shrouded Cave** → 34 children. **Frozen Grove** → 258 wood. **Large Convoy** → 18 engineers + 26 workers.
- **Coal Mine (Outpost)** → 263 coal on completion, then 800/day; if lost, 202 coal / 208 wood / 2 cores.
- **Tesla City (Outpost)** → 1 steam core/day, the **only renewable core source**. Unlocks only after Winterhome is discovered.
  _source: Deep Research handoff 2026-06-02 (5 sources) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

**Maximum 2 Outposts per city.** Realistic core supply: ~20 without Tesla City, ~30-35 stretched with it.
_source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

### Missable: Tesla City Outpost
Must be reached **before the storm**; rushing Winterhome shortens the window. `missable: yes`
_source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression · missable: yes_
> **Cross-system dependency** -- see `dependencies.md` DEP-001, PON-001: Tesla City is the only renewable Steam Core source (1/day); the Great Storm permanently closes the Beacon and the access window.

### Missable: day-15 Winterhome messenger
The day-15 messenger **dies on arrival** unless you scout Winterhome first to prevent it -- otherwise it voids the "save everyone" trophies. `missable: yes`
_source: Deep Research handoff 2026-06-02 · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression · missable: yes_

## Story note (gated)
- Discovering Winterhome's fate (the **cannibalism chronicle**) drops Hope sharply and spawns the **Londoners faction.** See `sections/story_notes.md`.
  _source: Deep Research handoff 2026-06-02 (4 sources) · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 3 · category: lore · spoiler: story_

## Ordered milestone sequence (P2)

Ordered key gates from scenario start to Great Storm. Entry edge / exit edge / PoNR per gate.

1. **Day 1 setup** *(spoiler: none)* — Start: 50 workers, 15 engineers, 15 children, no resources. First Adaptation law (Emergency Shift or Child Labour). Entry: scenario start. Exit: working economy by night 1.
   _source: Deep Research handoff 2026-06-02 (P2, 4 sources) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

2. **Workshop** *(none)* — Day 1; ~10 wood + engineers. Exit: technology tree unlocked. PoNR: no.

3. **First cold wave** *(none)* — Day 5, 07:00, temperature ~−30 °C. Weather always changes at 07:00. Entry: generator + initial heat plan.
   _source: Deep Research handoff 2026-06-02 (P2, 3 sources) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

4. **Beacon** *(none)* — Day 2–3. Research: 10 wood. Build: 20 wood / 35 steel. Scout team: 40 wood + 5 workers. Exit: expedition system. PoNR: no.

5. **Adaptation available; Purpose locked** *(progression)* — Purpose (Faith/Order) is unavailable until the Londoners trigger. No PoNR yet.
   _source: Deep Research handoff 2026-06-02 (P2, 4 sources) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

6. **Convoy + "Search for Other Cities" arc** *(progression)* — Days 1–14. Scout stray convoy survivors, then locate Winterhome. Route choices are partial PoNR.
   _source: Deep Research handoff 2026-06-02 (P2, 3 sources) · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

7. **Winterhome discovery + Purpose unlock (Act 2 start)** *(progression)* — ~Day 14–15. Scouting Winterhome OR the day-15 messenger fires the Londoners crisis and unlocks Faith/Order (permanent). The storm timer starts from this event. Best practice: do NOT scout Winterhome before day 14 / early day 15 -- scouting it early pulls the storm closer. If Winterhome is not scouted before ~10:00 on day 15, the messenger dies on arrival (Hope drop + corpse-disposal). PoNR: **YES** (Faith/Order permanent; messenger death is a no-restore-messenger run concern).
   _source: Deep Research handoff 2026-06-02 (P2, 5 sources) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_
   > **Cross-system dependency** -- see `dependencies.md` DEP-003: Winterhome discovery triggers the Londoners crisis AND starts the Great Storm timer; Purpose laws (Faith/Order) are unavailable before this event.

8. **Tesla City window** *(progression)* — Eastern scouting route opens only after Winterhome discovered. Yields 1 Steam Core/day (the only renewable core source). **Missable before the storm.** Tesla City and Gloomy Cave have random outcomes that can kill the scout party -- save before scouting. PoNR: **YES** (missable). → `sections/missables.md`
   _source: Deep Research handoff 2026-06-02 (P2, 4 sources) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression · missable: yes_

9. **The Londoners faction conflict** *(progression)* — Hope drops sharply on Winterhome discovery; citizens join the Londoners. Raise Hope (~50%+) to reduce membership; subplots include Prey on Discontent (speeches), vandalism, and theft. Reducing Londoners to zero before they leave (without force) is achievement-relevant. Partial PoNR.
   _source: Deep Research handoff 2026-06-02 (P2, 4 sources) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

10. **"Crossing the line" Purpose laws** *(story)* — Signing Pledge of Loyalty / Forceful Persuasion (Order) or Protector of the Truth / Righteous Denunciation (Faith) blocks the Golden Path permanently and changes the music. PoNR: **YES**. → `paths/`, `sections/missables.md`
    _source: Deep Research handoff 2026-06-02 (P2, 4 sources) · capture: web_fetch · confidence: high · enemy-tier: 0 · puzzle-tier: 3 · category: mainline · spoiler: story · missable: yes_

11. **Refugees from Frostland (Act 3 start)** *(progression)* — After the Londoners are resolved, refugee groups arrive warning of the storm. Accept or refuse. PoNR: no.
    _source: Deep Research handoff 2026-06-02 (P2, 3 sources) · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

12. **"What looms ahead" storm-prep quest** *(none)* — Research Beacon: Stereoscopic Lens; gather a week of food per citizen; research Overdrive Couplings and Generator Power Upgrade III. PoNR: no.
    _source: Deep Research handoff 2026-06-02 (P2, 3 sources) · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 0 · category: mainline · spoiler: none_

13. **Rescue survivors -- Snow Burrows, Ice Crevasse, Deep Hollow** *(progression)* — Triggered by "What looms ahead." Dispatch scouts to these three nodes before the storm locks the Beacon. Partial PoNR: survivors become unreachable once the storm closes scouting. `missable: yes`
    _source: Deep Research handoff 2026-06-02 (P2, 2 sources) · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression · missable: yes_

14. **Recall all scouts and outpost teams** *(none)* — Before the storm closes the Beacon. No PoNR for this action itself; failing to recall leaves resources/workers stranded.

15. **The Great Storm (final 7 days)** *(late-game)* — See "The Great Storm" section above. Latest without exploits: day 43. PoNR: **YES** (endgame).

16. **Storm subplots** *(progression)* — **Fear of the Storm** (panic event, city-wide Hope pressure); **Desperate Father** (a father and daughter venture outside -- can result in a death). Both are partial-PoNR events once the storm starts.
    _source: Deep Research handoff 2026-06-02 (P2, 2 sources) · capture: web_fetch · confidence: medium · enemy-tier: 0 · puzzle-tier: 1 · category: mainline · spoiler: progression_

## See also
- Builds: `items/builds.md` (A New Home) · Endings: `endings/a_new_home_endings.md` · Law paths: `paths/`
- Steam-core sourcing & resource bottlenecks: `mechanics.md`

---

## Sources
- frostpunk.fandom.com; thegamer.com; steamcommunity.com; stopgame.ru (RU); namu.wiki (KR). Deep Research handoff, 2026-06-02.
