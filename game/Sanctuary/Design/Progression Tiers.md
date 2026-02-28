---
tags:
  - sanctuary/design
  - framework
  - reference
---

# Progression Tiers

> A consolidated reference for all tier systems in Sanctuary. Each tier table lives in its source note — this note collects them in one place for cross-system analysis.

Sanctuary layers multiple tier systems that interlock: clearing a fog tier unlocks crystal types that enable gem tiers that gate assault levels that require depth floors. Understanding how tiers map across systems reveals the game's macro-progression structure.

---

## Fog Network Tiers

Source: [[Sanctuary/Combat/Fog System#Network Difficulty Tiers|Fog System]]

| Tier | Distance from Town | Characteristics |
| ---- | ------------------ | --------------- |
| 1 | Close | Slow fog regen, passive defenders, single emitter |
| 2 | Medium | Moderate regen, some aggressive clouds, environmental hazards |
| 3 | Far | Fast regen, aggressive defenders, multiple emitters |
| 4 | Remote | Emitters relocate, coordinated cloud attacks, elite rewards |

**Design note:** Clearing Tier N networks reveals Tier N+1 locations ([[Sanctuary/Core Loops/Progression Systems|Progression Systems]]). Each tier demands qualitatively different strategies, not just higher stats.

---

## Core Depths Floor Tiers

Source: [[Sanctuary/Progression/Core Depths|Core Depths]]

| Floor Range | Difficulty | Rewards |
| ----------- | ---------- | ------- |
| 1–10 | Easy | Common resources, tutorials |
| 11–25 | Medium | Rare shards, pattern blueprints |
| 26–50 | Hard | Power shards, unique cores |
| 51+ | Extreme | Legendary items, endgame content |

**Design note:** Higher floors gate materials for advanced [[Sanctuary/Crystals/Crystal Growing|crystal patterns]] and [[Sanctuary/Combat/Combat & Defense|invasion defense]]. The Stardew-mine-style persistence creates a long-horizon goal.

---

## Crystal Type Hierarchy

Source: [[Sanctuary/Crystals/Crystal Types & Structures|Crystal Types & Structures]]

### By Colour (Power Level)
| Colour | Tier |
| ------ | ---- |
| Blue | Base |
| Green | Mid |
| Red | High |
| Gold | Max |

### By Function
| Type | Role | Key Mechanic |
| ---- | ---- | ------------ |
| Power Crystals | Network energy | Tiered Blue → Gold, can level up with maintenance |
| Raw Crystals | Farm resource | Harvested for gems, primary farm output |
| Dark Crystals | Night threat | Spawn powerful enemies at nighttime |
| Crystal Catalyst | Liquid resource | Hexagonal areas, harvested via siphon spell |

### Special Types
| Type | Property |
| ---- | -------- |
| Teleporter Crystal | Slow growth, hard shards |
| Black Crystal | Grows from human death |

---

## Projector Tiers

Source: [[Sanctuary/Crystals/Crystal Growing|Crystal Growing]]

| Tier | Bed Slots | Special Features |
| ---- | --------- | ---------------- |
| Basic | 4 | Standard growth |
| Advanced | 9 | Pattern bonuses |
| Master | 16 | Geometry arrangements, rare crystals |

**Design note:** Projector tier gates access to the [[Sanctuary/Design/Meaningful Choice#Crystal Geometry Specialisation|crystal geometry system]], which in turn gates rare resources for endgame.

---

## Crystal Farming Difficulty

Source: [[Sanctuary/Crystals/Crystal Growing|Crystal Growing]]

| Type | Difficulty | Primary Use |
| ---- | ---------- | ----------- |
| Common | Easy | Currency, basic potions |
| Elemental | Medium | Magical ammunition |
| Power | Hard | Network expansion |
| Rare/Named | Pattern-dependent | Special crafting, quests |

---

## Gem / Assault Tier Requirements

Source: [[Sanctuary/Combat/Combat & Defense|Combat & Defense]]

| Assault Level | Min Gem Tier | Source |
| ------------- | ------------ | ------ |
| 1–3 | Common | Basic farming |
| 4–6 | Uncommon | Pattern farming |
| 7–10 | Rare | Depth excavation |
| 11+ | Legendary | Rift drops, boss rewards |

**Design note:** This table is the clearest expression of how tiers gate each other. You cannot survive Assault 7+ without Rare gems, which require Core Depths floors 26–50, which require clearing Tier 3+ fog networks.

---

## Resource Abundance Tiers

Source: [[Sanctuary/Crystals/Crystal Growing|Crystal Growing]]

| Resource | Acquisition | Abundance | Primary Use |
| -------- | ----------- | --------- | ----------- |
| Crystal Shards | Breaking crystals | Common | Planting, basic crafting |
| Crystal Catalyst | Harvesting in fog zones | Abundant | Watering crystals |
| Crystal Cores | Extracting from nexus | Scarce | Building projector slots |
| Power Shards | Destroying wild power crystals | Limited | Growing power crystals |
| Magic Essence | Harvesting mature crystals | Variable | Potions, advanced crafting |
| Raw Gems | Breaking mature crystals | Variable | Currency, ammunition |

**Design note:** The scarcity gradient (Common → Scarce) maps directly to progression depth. Abundant resources enable moment-to-moment play; scarce resources gate strategic decisions. See [[Sanctuary/Design/Constraints#Resource Scarcity|Resource Scarcity]].

---

## Control Center Power Caps

Source: [[Sanctuary/Crystals/Crystal Power & Networks#Central Command Point|Crystal Power & Networks]]

- The [[Sanctuary/Crystals/Crystal Power & Networks#Central Command Point|Central Command Point]] caps total power production
- Must be upgraded by supplying accumulated power
- Each upgrade increases the power ceiling, unlocking new network tiers
- Attack fog clouds target this structure — damage resets current progress toward the next level

**Design note:** The power cap is the **master gate** for macro-progression. All other tier systems ultimately bottleneck through the control center's level.

---

## Elemental Essence Sources

Source: [[Sanctuary/Combat/Spells/Elemental Essence System|Elemental Essence System]]

| Essence | Source | Location |
| ------- | ------ | -------- |
| Fire | Magma/Lava Geysers | Volcanic regions |
| Frost | Glacial/Cryo Geysers | Frozen tundra |
| Storm | Thunder/Lightning Geysers | Mountain peaks |
| Temporal | Chronos/Time Geysers | Ancient ruins (rare) |
| Gravity | Void/Singularity Geysers | Spatial anomalies (very rare) |
| Arcane | Prismatic/Arcane Geysers | Ley line convergences (rare) |

---

## Cross-System Tier Map

```
Fog Tier 1 ──► Blue Crystals ──► Common Gems ──► Assault 1-3
    │                                                  │
    ▼                                                  ▼
Fog Tier 2 ──► Green Crystals ──► Uncommon Gems ──► Assault 4-6
    │                                                  │
    ▼                                                  ▼
Fog Tier 3 ──► Red Crystals ──► Rare Gems ──► Assault 7-10
    │               │                              │
    ▼               ▼                              ▼
Fog Tier 4 ──► Gold Crystals ──► Legendary Gems ──► Assault 11+
                    │                                  │
                    ▼                                  ▼
            Core Depths 51+ ────────────► Central Rift
```

Each horizontal band represents a **progression plateau** — a period where the player has unlocked a new tier of systems and must master them before pushing to the next.

---

## Related

- [[Sanctuary/Design/Design Framework|Design Framework]]
- [[Sanctuary/Design/Constraints|Constraints]]
- [[Sanctuary/Design/Meaningful Choice|Meaningful Choice]]
- [[Sanctuary/Design/Learning Patterns|Learning Patterns]]
