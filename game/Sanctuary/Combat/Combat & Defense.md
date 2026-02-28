---
tags:
  - sanctuary/combat
  - mechanic
---

# Combat & Defense

## Core Combat

- Fight monsters spawned by crystal patches and power sources
- Build and upgrade defensive [[Sanctuary/Combat/Tower System|towers]] to protect town and crystal farms
- Defend against periodic monster attacks from [[Sanctuary/Crystals/Crystal Power & Networks#Crystal Network Nexus Gate|crystal nexus structures]]
- Clear natural crystal growths to reduce monster threat

## Monster Scaling

- More crystals = more power but more danger
- Attack frequency scales with the number of power-generating crystal patches cultivated
- Rewards players who balance offense (attacking the nexus) with defense (protecting the town)

## Monster–Crystal Farm Interaction

- Monsters will seek out your crystal farm and attempt to suck on your crystals to grow bigger
- Can build towers to protect your crystals
- However towers will consume your crystal resources

## Endgame Tower Defense

- After generating enough power, monsters spawn at map outskirts and come for the town
- Becomes a massive tower defense game requiring towers at specific locations
- Beating progressively powerful waves requires red gem tech
- Fog attack vs monster attack scale differently

## Invasion / Assault System

Late-game assault system triggered by high power output.

### Defense Requirements

#### Tower Scaling

- Tower effectiveness scales primarily with **gem power**
- Early game: basic gems suffice for fog management
- Late game: **high-tier gems required** to damage invasion forces
- Creates demand for advanced crystal farming and rare gem production

#### Spell Scaling

- Combat spells also scale with gem power
- Player's personal combat effectiveness tied to gem quality
- Encourages active defense participation, not just tower reliance

#### Gem Tier Requirements

| Assault Level | Minimum Gem Tier | Source |
| ------------- | ---------------- | ------ |
| 1-3 | Common | Basic farming |
| 4-6 | Uncommon | Pattern farming |
| 7-10 | Rare | Depth excavation |
| 11+ | Legendary | Rift drops, boss rewards |

### Strategic Implications

#### Base Layout Matters

- Enemies path straight to center
- Player must design **kill corridors** with overlapping tower coverage
- Chokepoints become valuable
- Town layout shifts from aesthetic to strategic

#### Resource Allocation Tension

- Spend gems on expansion (more power = harder enemies) **OR**
- Stockpile gems for defense (slower growth but safer)
- High-tier gems are **scarce** — can't do everything

#### The Growth Paradox

- Early game: "I need more power to explore further"
- Late game: "More power makes enemies stronger, but I need it to fight them"

### Fail State

- If enemies reach the town center and destroy the **core structure**: **GAME OVER**
- This is the player's first real loss condition
- Early game is essentially safe (tutorial/learning phase)
- Late game introduces genuine stakes and tension

### Assault Structure

```
┌─────────────────────────────────────────────┐
│            ASSAULT CYCLE                    │
├─────────────────────────────────────────────┤
│ Day 1: Warning signs / scouts spotted       │
│ Day 2: Enemy base appears on map edge       │
│ Day 3: Wave 1 launches                      │
│ Day 4: Wave 2 (stronger)                    │
│ Day 5: Wave 3 (strongest)                   │
│ Day 6: Assault ends if survived             │
│ Days 7-20: Recovery period                  │
│ Day 21: Next assault cycle begins           │
└─────────────────────────────────────────────┘
```

### Design Considerations

- **Telegraphing**: Give players advance warning of incoming assaults — show enemy base location, estimated wave strength, and allow preparation time
- **Catch-Up Mechanics**: If player falls behind, options include mercenary NPCs for hire, desperate measures (sacrifice buildings for burst power), or tactical retreats (lose outer territory to consolidate)
- **Victory Condition**: After repelling enough assaults, locate and assault the **enemy origin point** — destroying it ends the invasion threat (alternate endgame to [[Sanctuary/Progression/Central Rift|The Rift]])

## Related

- [[Sanctuary/Combat/Tower System|Tower System]]
- [[Sanctuary/Combat/Fog System|Fog System]]
- [[Sanctuary/Combat/Armor System|Armor System]]
- [[Sanctuary/Combat/Spells/Spell Progression|Spell Progression]]
- [[Sanctuary/Crystals/Crystal Types & Structures|Crystal Types & Structures]]
