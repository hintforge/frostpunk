# Frostpunk artifacts

Self-contained player tools built from this guide's corpus. Download one, open it in any
browser, keep it beside the game. Nothing is installed, nothing phones home, and nothing leaves
your machine — your plan is saved in your own browser and exports to a JSON file you control.

## `city_planner.html` — generator-ring city planner

Plan the ring layout around the generator, including space for buildings you have not
unlocked yet.

Frostpunk builds on a **radial grid**, so a building's footprint is *angular × radial* tiles —
width along the curve, then depth straight out from the generator. That means space around the
generator is not an area budget, it is an **angular budget per ring**, and the budget grows as
you move outward because the circumference does. The planner models exactly that: pick a
building, click where you want it, and watch the ring's angular tiles fill up.

**What it answers that the wiki does not:**

- **Reach cost.** The wiki prices the House tech at 40 Wood / 25 Steel. That is not what a House
  costs you — you must first buy Bunkhouse, and before either, the Drawing Boards / Drafting
  Machines / Mechanical Calculators tier unlocks. The real bill is **285 Wood / 110 Steel**, or
  7.1× the sticker price. The planner computes this chain for every tech-gated building and
  totals the deduplicated research bill for your whole plan.
- **Will it fit.** Each ring shows angular tiles used against its circumference, and refuses to
  place a building where one will not fit.
- **What the range upgrade buys.** Move the generator range dial and the heat boundary moves with
  it, telling you how many more rings come fully inside.
- **What is still locked.** Buildings you have not researched are placeable as *reserved space* —
  drawn hatched, so you can hold the ground now and see what it will cost to earn it.

**Research is built in.** Every tech carries its Workshop tab — Heating, Resources, Food/Health &
Shelter, Exploration & Industry — plus the Book of Laws for law-gated buildings. Filter the
building list by tree, and tick off what you have already researched in the Research tab; ticking
a node auto-ticks its prerequisites, and the map, the list and the totals all follow.

### Where the numbers come from

| Data | Source |
|---|---|
| Footprints, build costs, insulation, unlock requirements | Official Frostpunk Wiki *Buildings* table |
| Research costs, prerequisites, tiers | this guide's [`items/upgrades.md`](../items/upgrades.md) |
| Generator range (+3 tiles per upgrade) | this guide's [`items/upgrades.md`](../items/upgrades.md), confidence *confirmed* |
| Ring capacity, base heat radius, Steam Hub radius | **derived** — see below |

### The honest part

Ring capacity, the base heat radius and the Steam Hub radius are **published nowhere** — not on
the wiki, not in the game's UI. The planner derives them (ring capacity is the circumference in
tiles at the ring's mid-radius) and calibrates against the only community measurement that
exists, which is itself internally inconsistent. Against the one trustworthy figure in it — ring 1
holds 10 buildings — the model lands exactly; on outer rings it runs up to **~13% pessimistic**.

The wiki also states plainly that buildings "may slightly shrink or grow in size to accommodate
their surroundings", so no planner can be tile-exact. **If the game fits more than the planner
says, the game is right** — every derived number is editable in the Model tab.

Not modelled: roads and road adjacency, shelter population capacity (no sourced figures exist),
coal burn per ring, and the two DLC scenarios *The Last Autumn* and *On The Edge* (both replace
the generator heating line with Braziers, so the ring model does not apply).

### Controls

| To do this | Do this |
|---|---|
| Place a building | Click it in the list, then click where you want it on a ring |
| Move it | Drag it around the ring, or across into another ring |
| Remove it | Right-click it, or select it and press Delete |
| Rotate a two-footprint building | Select it, then **Rotate** |
| Narrow to one research tree | Click a chip above the building list |
| Stop placing | Esc |

Your plan is kept in browser storage and survives a reload. **Export** writes it to JSON;
**Import** reads it back, so a layout is portable between machines.
