---
tags:
  - sanctuary/combat
  - sanctuary/combat/fog
  - mechanic
  - obstacle
---

# Fog System

## Fog Clouds

- Some crystal networks produce a structure which emits fog clouds
- The fog is the **main constraint** to player exploration
- Acts as a map barrier which must be overcome to access crystal network resources

### Fog Cloud Behaviour

- Fog clouds have a damage radius
- They slowly drift within the area controlled by the crystal network cell
- Fog clouds can be destroyed:
  - By player spells
  - By [[Sanctuary/Combat/Tower System#Anti-Fog Tower|anti-fog tower]]
- The crystal network will periodically refresh destroyed fog clouds
- Fog cloud damage, intensity, and frequency **increases during the night**
- Some crystal structures impose benefits to fog clouds making them harder to destroy — player needs magic spells to remove these structures
- Continuously eliminating fog clouds will slowly raise the aggression level of the crystal network

## Fog Network Aggression

- Fog networks have an **aggression level** that increases based on how many attack towers and extractors are affecting the network
- When aggression exceeds a threshold, the network sends out **attack fog clouds**
- Attack fog clouds route towards the player's **central command point / nexus** and assault it
- Attack cloud strength is determined by:
  - The source fog network's level
  - The player's current power maximum
  - How close the player is to reaching the next power level
- If attack clouds deal enough damage, they **reset current progress** (steal all accumulated power)
- The player controls which direction attacks come from by choosing which fog networks to threaten
- Late game: some fog networks are **inherently aggressive** once discovered
- The [[Sanctuary/Combat/Fog System#Variation System|variation system]] can modify fog networks, potentially imparting aggressive behaviour
- Early game introduces smaller, tutorial-sized cloud networks for the player to learn these mechanics

### Attack Fog Cloud Behaviour

- Attack fog clouds are only blocked by **hard terrain** (buildings slow their flow but don't stop it)
- Most attack fog clouds ignore towers and head straight for the central command point
- The player can shape attack corridors through strategic tower/extractor placement

## Cloud Difficulty Scaling

- Higher-level clouds will **seek the player out** and overload certain cloud structures
- Clouds correspond to gem level — higher damage and much tougher
- **Tornado/gust mechanic** — a large mass of clouds is emitted at the player from some source, requiring specific strategies to overcome

### Network Difficulty Tiers

| Tier | Distance from Town | Characteristics |
| ---- | ------------------ | --------------- |
| 1 | Close | Slow fog regen, passive defenders, single emitter |
| 2 | Medium | Moderate regen, some aggressive clouds, environmental hazards |
| 3 | Far | Fast regen, aggressive defenders, multiple emitters |
| 4 | Remote | Emitters relocate, coordinated cloud attacks, elite rewards |

## Variation System

- A source of variation on the map spreads through natural means and slowly converts fogs to drop different items / behave differently
- The player can eventually control these sources to graduate the behaviour
- The drops are required to advance up the [[Sanctuary/Progression/Skill Perk Tree|skill tree]]
- Some skills are gated behind the player being able to route successfully

### Variation Routers

- Probably exist at the intersection of hexagons
- Only affect networks adjacent to them
- Not all hexagon intersections have routers; some are yet to be upgraded/discovered

### Variation Sources

- Have starting power which degrades
- Variations can combine in different ways to produce different effects

### Gambling Mechanic

- Randomly modify some source on the map
- Adds a source, or randomly introduces a negative modifier

## Traversal

- Can destroy the fog, but it comes back
- Methods to prevent fog return:
  - **Anti-fog tower** — destroys fogs that come close, prevents new spawns
  - **Spell** — prevents clouds from respawning in an area, slowly pushes clouds back
  - **Building** — similar to the spell but lasts much longer, requires a power cell (produced from a factory using crystal power)
- Player pushes forward, finds an area to farm, deploys the spell, farms, then tries to get back

### Armour Options

- Player armour which grants passive cloud resist
- See [[Sanctuary/Combat/Armor System|Armor System]]

## Boxing-In Mechanic

- As players venture deeper into a network, fog restores behind them
- Players can become **surrounded** by restored fog
- **Fog deals damage** to players caught within it — prolonged exposure results in death
- This creates a risk/reward tension: push deeper for resources vs. maintaining escape routes
- Fog damage is **gradual**, allowing a scramble window before death

## Death and Recovery

- **Respawn location**: Town or nearest safe point
- **Potential death penalties** (choose one or combine):
  - Lose carried (unbanked) resources
  - Corpse run: dropped loot remains in fog with a ticking clock to recover
  - Temporary stat debuff

## Related

- [[Sanctuary/Combat/Tower System|Tower System]]
- [[Sanctuary/Core Loops/Exploration & Expansion|Exploration & Expansion]]
- [[Sanctuary/Crystals/Crystal Power & Networks|Crystal Power & Networks]]
- [[Sanctuary/Progression/Skill Perk Tree|Skill Perk Tree]]
- [[Sanctuary/Core Loops/Progression Systems|Progression Systems]]
