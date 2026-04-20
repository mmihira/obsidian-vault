---
tags:
  - sanctuary/crystals
  - sanctuary/crystals/farming
  - mechanic
---

# Crystal Growing

## Overview

- Crystal shard is analogous to **seeds**
- Crystal catalyst is analogous to **water**

## Resource Hierarchy

| Resource             | Acquisition                           | Abundance | Primary Use                 |
| -------------------- | ------------------------------------- | --------- | --------------------------- |
| **Crystal Shards**   | Breaking wild/farmed crystals         | Common    | Planting, basic crafting    |
| **Crystal Catalyst** | Harvesting wild crystals in fog zones | Abundant  | "Watering" growing crystals |
| **Power Shards**     | Destroying wild power crystals        | Limited   | Growing power crystals      |
| **Magic Essence**    | Harvesting mature crystals            | Variable  | Potions, advanced crafting  |
| **Raw Gems**         | Breaking mature crystals              | Variable  | Currency, ammunition        |
|                      |                                       |           |                             |

## Constraints

- **Time** 
	- Crystal take time to fully grow
- Crystal Projectors
	- Need projects to act as beds
- Power
	- Every crystal projector take some amount of power
- Crystal catalyst
	- Must have enough crystal catalsyt to feed the crystals
- Crystal shards
	  - Shards are required as seeds

## Spraying Mechanic

- Player chooses the spraying spell
- Indicator of affected area (circular)
- Crystals lacking catalyst appear dull without colour
- As they get sprayed, their luminosity changes; once fully sprayed they make a satisfying sound and particle effect animation
- Player can upgrade the spell to spray a progressively larger area
- Spraying continuously consumes crystal catalyst (however catalyst is relatively abundant)

### Power Crystal Shards

- Crystal power shards are used to grow power crystals
- Power shards are of limited quantity and must be obtained by destroying wild power crystals

## Core Projector

- Core projectors project crystal beds onto the ground, which can be used to grow crystals by planting crystal shards
- Relatively cheap to build
- Player can change the layout configuration
- Different tiers of core projectors exist with increased bed counts
- Core projectors **continuously consume power** while active — this is the primary cap on how many beds the player can run simultaneously
- Core projectors are upgradeable with modifiers:
  - **Yield increase** — more resources per harvest
  - **Growth speed** — reduced maturation time
  - **Auto-harvest** — automatically collects mature crystals
  - **Catalyst efficiency** — less spraying required
  - **Power efficiency** — reduces the projector's power draw

### Power as a Scaling Cap

- Each active projector draws power from the sanctuary's power network
- Higher-tier projectors draw more power but offer more bed slots and features
- The player's total crystal farming capacity is effectively bounded by their power production
- Upgrading power infrastructure is the progression path to scaling up crystal output

### Projector Tiers

| Tier     | Bed Slots | Power Draw | Special Features                      |
| -------- | --------- | ---------- | ------------------------------------- |
| Basic    | 4         | Low        | Standard growth                       |
| Advanced | 9         | Medium     | Unlocks pattern bonuses               |
| Master   | 16        | High       | Geometry arrangements, rare crystals  |
- Initially introduced via the merchant NPC who has a core machine deployed for making potions
- Player can place core projectors mostly anywhere (though conflict with NPC building locations is a concern)

## Crystal Growth Stages

| Stage | Visual | Interaction |
| ----- | ------ | ----------- |
| Planted | Small dull shard | Requires catalyst |
| Growing | Increasing glow, texture changes | Continue spraying |
| Mature | Full luminosity, distinct form | Ready for harvest |
| Overgrown | Pulsing, unstable | Bonus yield or risk? |

## Geometry & Arrangement System

Advanced farming involves spatial puzzles:

- **Basic**: Any arrangement works
- **Intermediate**: Adjacent crystal types affect growth (synergy bonuses)
- **Advanced**: Specific patterns unlock rare crystal growth
  - Triangle formations
  - Ring arrangements
  - Spiral configurations
- **Mastery**: Hybrid patterns combining multiple rare types

## Variety

- Customisable layout/variety/schedule
- Player can grow crystals of increasing rarity as the game progresses
- Geometry/arrangement of crystals unlocks certain crystal growth (see above)

### Crystal Types

| Crystal Type | Growth Difficulty | Primary Use |
| ------------ | ----------------- | ----------- |
| Common | Easy | Currency, basic potions |
| Elemental | Medium | Magical ammunition |
| Power | Hard (requires power shards) | Network expansion |
| Rare/Named | Pattern-dependent | Special crafting, quests |

## Value

- Breaking/harvesting crystals is easy
- Crystals can be sold to the overworld for money
- Certain crystals will be used as magical ammo

## NPC Crystal Patches

- Some NPCs will mine their own crystal patch to produce stuff for the player
- Early in the game, the player is tasked with protecting NPC crystal patches

## Related

- [[Sanctuary/Crystals/Crystal Overview|Crystal Overview]]
- [[Sanctuary/Crystals/Crystal Types & Structures|Crystal Types & Structures]]
- [[Sanctuary/Crystals/Crystal Interaction|Crystal Interaction]]
- [[Sanctuary/Town/NPC System|NPC System]]
- [[Sanctuary/Economy/Items & Resources|Items & Resources]]
