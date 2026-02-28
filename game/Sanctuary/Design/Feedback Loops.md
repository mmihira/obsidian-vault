---
tags:
  - sanctuary/design
  - framework
---

# Feedback Loops

> *"A game is a series of interesting decisions."* — Sid Meier

Feedback loops are the engine of Sanctuary's pacing. **Positive loops** (virtuous spirals) reward investment and accelerate growth. **Negative loops** (balancing mechanics) prevent runaway dominance and keep the game challenging. The interplay between them is what makes Sanctuary feel dynamic.

---

## Positive Loops (Virtuous Spirals)

### Core Loop Spiral

The fundamental virtuous spiral from [[Sanctuary/Core Loops/Core Game Loops|Core Game Loops]]:

```
┌─────────────────────────────────────────────────────────┐
│                                                         │
│   Clear Networks ──► Gain Power ──► Extend Reach ───┐   │
│         ▲                                           │   │
│         │                                           ▼   │
│   Grow Crystals ◄── Build Projectors ◄── Get Cores ◄┘   │
│         │                                               │
│         ▼                                               │
│   Craft Potions ──► Survive Longer ──► Explore More ───►│
│                                                         │
└─────────────────────────────────────────────────────────┘
```

Each station in this loop feeds the next. More networks cleared → more cores → more projectors → more crystals → more potions → longer exploration → more networks cleared.

### Crystal Farming Growth
- [[Sanctuary/Crystals/Crystal Growing|Crystal farms]] produce gems and essence
- Gems fund [[Sanctuary/Economy/Export Import System|exports]] → imports → better equipment
- Essence powers [[Sanctuary/Town/Production Chains|production chains]] → advanced crafting
- Advanced projectors ([[Sanctuary/Crystals/Crystal Growing|Basic → Advanced → Master]]) unlock geometry arrangements → rare crystal types → even better yields

### Power Network Expansion
- Clearing [[Sanctuary/Crystals/Crystal Power & Networks#Crystal Networks|crystal networks]] provides power
- Power extends [[Sanctuary/Crystals/Crystal Power & Networks#Power as Reach|tower range and repulsor duration]]
- Greater reach → access to further networks → more power
- Visual feedback: **glowing network tendrils** spread across the map ([[Sanctuary/Crystals/Crystal Power & Networks#Power Visualization|Power Visualization]])

### Combat Gem Scaling
- Higher-tier gems → more powerful [[Sanctuary/Combat/Spells/Spell Progression|spells]] and [[Sanctuary/Combat/Tower System|towers]]
- Better combat capability → ability to clear harder networks
- Harder networks → rarer gem drops
- Gem tier ladder: Common → Uncommon → Rare → Legendary ([[Sanctuary/Combat/Combat & Defense|Combat & Defense]])

### Town & NPC Self-Sustaining Growth
- [[Sanctuary/Town/NPC System|NPCs]] build homes → then businesses → then provide benefits
- Player keeps the [[Sanctuary/Town/NPC System|cooking pot]] filled → NPCs gather materials → NPCs self-sustain
- Self-sustaining NPCs free up player time → more exploration → more town renown → more settlers
- [[Sanctuary/Town/Town Progression|Town Renown]] attracts new settlers → more buildings → more services

### Export Capacity Loop
- [[Sanctuary/Economy/Export Import System|Export terminal]] ships gems → funds upgrades
- Exporter has its own upgrade tree → increased capacity and corporation benefits
- More capacity → more gems shipped → faster upgrades
- [[Sanctuary/Economy/Portal System|Portal]] strengthens with gems → larger item transfers → further acceleration

### Network Tier Unlocking
- Clearing Tier N networks reveals Tier N+1 locations ([[Sanctuary/Core Loops/Progression Systems|Progression Systems]])
- Higher tiers yield more power, rarer crystals, unique cores
- More power → ability to tackle the next tier
- Creates a staircase of escalating capability

---

## Negative Loops (Balancing Mechanics)

### Fog Aggression Scaling
- [[Sanctuary/Combat/Fog System#Fog Network Aggression|Fog aggression]] increases based on attack towers and extractors affecting a network
- Pushing too aggressively triggers **attack fog clouds** targeting the [[Sanctuary/Crystals/Crystal Power & Networks#Central Command Point|central command point]]
- Attack strength scales with source network level *and* player's current power maximum
- Forces the player to choose *which direction* attacks come from — strategic corridor management

### Invasion / Assault System
- [[Sanctuary/Combat/Combat & Defense|Assault cycle]]: 21-day rhythm with 5 days of escalating waves
- Monster waves scale with total power output
- Late game: enough power triggers waves from **map outskirts** ([[Sanctuary/Core Loops/Exploration & Expansion|Exploration & Expansion]])
- Assault telegraphing provides advance warning but demands preparation
- Assault tier requirements gate progression behind gem quality:

| Assault Level | Min Gem Tier | Source |
| ------------- | ------------ | ------ |
| 1–3 | Common | Basic farming |
| 4–6 | Uncommon | Pattern farming |
| 7–10 | Rare | Depth excavation |
| 11+ | Legendary | Rift drops, boss rewards |

### Monster Scaling with Crystal Farms
- Monster frequency scales with number of cultivated [[Sanctuary/Crystals/Crystal Types & Structures#Power Crystals|crystal patches]]
- Monsters **seek out crystal farms** to grow bigger ([[Sanctuary/Combat/Combat & Defense|Combat & Defense]])
- At the [[Sanctuary/Map/Crystal Wall|Crystal Wall]], monster attack frequency scales with cultivated patches
- Creates a direct mechanical link: economic growth = military threat

### The Growth Paradox

> **The central strategic tension of Sanctuary.**

The Growth Paradox emerges from the intersection of positive and negative loops:

- **More crystals** = more power = more reach = more resources (positive)
- **More crystals** = more monsters = stronger assaults = higher risk (negative)
- **Gems spent on expansion** make enemies harder; **gems stockpiled** slow growth but are safer
- **High-tier gems are scarce** — every gem spent on towers is a gem not spent on exports

The player must constantly navigate this tension. There is no "safe" strategy — only strategies with *different risk profiles*. This is what gives Sanctuary its strategic depth and prevents the late game from becoming a passive snowball.

### Anti-Hoarding Mechanics
- Unused [[Sanctuary/Progression/Knowledge System|skill points reduce knowledge gain]] — must commit to specialisation
- Mana pool upgrades have **exponentially decreasing returns** — diminishing value from pure stat investment
- [[Sanctuary/Progression/Food System|Food]] cannot be stockpiled efficiently — daily import dependency

---

## Loop Interactions

```
  POSITIVE LOOPS                    NEGATIVE LOOPS
  ─────────────                     ──────────────
  Crystal farming ──────────┐  ┌── Monster scaling
  Power expansion ──────────┤  ├── Fog aggression
  Town growth ──────────────┤  ├── Assault waves
  Export capacity ──────────┤  ├── Resource competition
                            ▼  ▼
                    ┌───────────────┐
                    │ GROWTH        │
                    │ PARADOX       │
                    │               │
                    │ Every gain    │
                    │ creates a     │
                    │ new threat    │
                    └───────────────┘
```

The Growth Paradox is not a single mechanic — it is the **emergent property** of all positive and negative loops intersecting. This is Sanctuary's answer to the classic problem of late-game stagnation: the world *always* pushes back proportionally.

---

## Related

- [[Sanctuary/Design/Design Framework|Design Framework]]
- [[Sanctuary/Design/Constraints|Constraints]]
- [[Sanctuary/Design/Meaningful Choice|Meaningful Choice]]
- [[Sanctuary/Core Loops/Core Game Loops|Core Game Loops]]
