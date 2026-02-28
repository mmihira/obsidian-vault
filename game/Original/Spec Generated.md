<!-- mtoc-start -->

* [Additonal deisgn](#additonal-deisgn)
* [Crystal Networks: Core Loop Specification](#crystal-networks-core-loop-specification)
  * [Overview](#overview)
  * [1. Territory Control: The Fog Network System](#1-territory-control-the-fog-network-system)
    * [1.1 Network Structure](#11-network-structure)
    * [1.2 Fog Behavior](#12-fog-behavior)
    * [1.3 The Boxing-In Mechanic](#13-the-boxing-in-mechanic)
    * [1.4 Network Destruction](#14-network-destruction)
    * [1.5 Network Tapping (Alternative)](#15-network-tapping-alternative)
    * [1.6 Network Difficulty Scaling](#16-network-difficulty-scaling)
  * [2. Tower Defense: Cloud Management](#2-tower-defense-cloud-management)
    * [2.1 Tower Functions](#21-tower-functions)
    * [2.2 Tower Placement Strategy](#22-tower-placement-strategy)
    * [2.3 Angry Cloud Response](#23-angry-cloud-response)
    * [2.4 Tower Upgrades](#24-tower-upgrades)
  * [3. Exploration Tools](#3-exploration-tools)
    * [3.1 Fog Repulsor Spell](#31-fog-repulsor-spell)
    * [3.2 Repulsor Resource Management](#32-repulsor-resource-management)
    * [3.3 Death and Recovery](#33-death-and-recovery)
  * [4. Crystal Farming System](#4-crystal-farming-system)
    * [4.1 Resource Hierarchy](#41-resource-hierarchy)
    * [4.2 Core Projectors](#42-core-projectors)
      * [Projector Tiers](#projector-tiers)
      * [Projector Upgrades](#projector-upgrades)
    * [4.3 The Spraying Mechanic](#43-the-spraying-mechanic)
    * [4.4 Crystal Growth Stages](#44-crystal-growth-stages)
    * [4.5 Geometry & Arrangement System](#45-geometry--arrangement-system)
    * [4.6 Crystal Variety & Uses](#46-crystal-variety--uses)
  * [5. Power Network System](#5-power-network-system)
    * [5.1 The Player's Crystal Network](#51-the-players-crystal-network)
    * [5.2 Power as Reach](#52-power-as-reach)
    * [5.3 Power Visualization](#53-power-visualization)
  * [6. Survival Systems](#6-survival-systems)
    * [6.1 Hunger](#61-hunger)
    * [6.2 Mana Management](#62-mana-management)
    * [6.3 Day/Night Cycle](#63-daynight-cycle)
    * [6.4 Sleep Mechanic](#64-sleep-mechanic)
  * [7. Town Building & NPC Progression](#7-town-building--npc-progression)
    * [7.1 Building System](#71-building-system)
    * [7.2 NPC Attraction & Roles](#72-npc-attraction--roles)
    * [7.3 Town Advancement](#73-town-advancement)
    * [7.4 Resource Management](#74-resource-management)
    * [7.5 Projector Placement Conflict Resolution](#75-projector-placement-conflict-resolution)
  * [8. Macro Progression Systems](#8-macro-progression-systems)
    * [8.1 Network Tier Progression](#81-network-tier-progression)
    * [8.2 Core Depth Excavation (Dungeon System)](#82-core-depth-excavation-dungeon-system)
      * [Depth Structure](#depth-structure)
    * [8.3 The Central Rift (Long-Horizon Goal)](#83-the-central-rift-long-horizon-goal)
    * [8.4 Progression Visualization](#84-progression-visualization)
    * [9.4 Defense Requirements](#94-defense-requirements)
      * [Tower Scaling](#tower-scaling)
      * [Spell Scaling](#spell-scaling)
      * [Gem Tier Requirements (Example)](#gem-tier-requirements-example)
    * [9.5 Strategic Implications](#95-strategic-implications)
      * [Base Layout Matters](#base-layout-matters)
      * [Resource Allocation Tension](#resource-allocation-tension)
      * [The Growth Paradox](#the-growth-paradox)
    * [9.6 Fail State](#96-fail-state)
    * [9.7 Assault Structure Example](#97-assault-structure-example)
    * [9.8 Design Considerations](#98-design-considerations)
      * [Telegraphing](#telegraphing)
      * [Catch-Up Mechanics](#catch-up-mechanics)
      * [Victory Condition?](#victory-condition)
  * [10. Core Loop Summary](#10-core-loop-summary)
    * [10.1 Moment-to-Moment (Minutes)](#101-moment-to-moment-minutes)
    * [10.2 Session Loop (Hours)](#102-session-loop-hours)
    * [10.3 Campaign Loop (Days/Weeks)](#103-campaign-loop-daysweeks)
    * [10.4 The Virtuous Spiral](#104-the-virtuous-spiral)
  * [11. Open Design Questions](#11-open-design-questions)
  * [Appendix: Terminology Reference](#appendix-terminology-reference)

<!-- mtoc-end -->



# Additonal deisgn

- Fog network will send out attack fog clouds if their aggression level exceeds a threshold.
- Agression is determined by how many attack towers and extractors are effecting the fog network

The fog clouds will route towards your centeral command point/nexus, and attack it
The strenght of the attack fog clouuds is determined by the source fognetwork level, you current
power maximum, and also how close you are to reaching the next level

And if they do enough damage will reset the current progress (i.e they steal all your power)
The central command point is upgraded by supplying power to it
The central command point must be upgraded to increase your power production maximums
Remember that power production is sources from either tapping fog networks or takin gover their main emiitter

fog clouds are only really blocked  by hard terraibn, i.e buildings etc will just slow their flow down
most fog clouuds won't target towers, they will just head towards the central command point and attack it

the player though can control whhere the attack is coming from by choosing which fognetworks they choose to threaen
however late game, there will be some fog networks whihc are aggressive outright, if discovered,
also the fog variation network can modify fogNetworks which may impart an agressive nature to them

At the early game we introduce some smaller cloud networks just for the player to quickly become accusomted to the mechanics

# Crystal Networks: Core Loop Specification

## Overview

A survival farming game where players expand their territory by dismantling hostile crystal fog networks, harvesting their cores to fuel a growing crystal farming operation, and building a thriving town powered by crystal energy.

---

## 1. Territory Control: The Fog Network System

### 1.1 Network Structure

- The world map is divided into **cells**, each controlled by a crystal fog network
- Each network contains:
  - A central **fog emitter** (the "boss" objective)
  - **Wild crystals** that can be harvested for catalyst
  - **Angry cloud defenders** that protect the inner zones

### 1.2 Fog Behavior

- Crystal formations continuously generate fog clouds
- Fog clouds in the outer circles rotate anti or clockwise randomly
- When the player destroys fog clouds, the fog clouds will regenerate after a short time at their inital spawn position
- Fog clouds near the center are largely stationary and repsawn much quicker

### 1.3 The Boxing-In Mechanic

- As players venture deeper into a network, fog restores behind them
- Players can become **surrounded** by restored fog
- **Fog deals damage** to players caught within it
- Prolonged exposure results in **death**
- This creates a risk/reward tension: push deeper for resources vs. maintaining escape routes

### 1.4 Network Destruction

- Destroying the central **fog emitter** permanently clears the network
- Cleared networks grant:
  - Permanent **crystal power boost** to the player's network
  - Access to all resources within the cell
  - Potential **dungeon access** (core depth excavation)

### 1.5 Network Tapping (Alternative)

- Some networks can be **tapped** instead of destroyed
- Tapped networks provide **ongoing power income**
- Trade-off: network remains semi-active (reduced fog, some danger persists)
- Requires maintenance or periodic defense
- Mid-game option before player is strong enough for full clearance

### 1.6 Network Difficulty Scaling

| Tier | Distance from Town | Characteristics                                               |
| ---- | ------------------ | ------------------------------------------------------------- |
| 1    | Close              | Slow fog regen, passive defenders, single emitter             |
| 2    | Medium             | Moderate regen, some aggressive clouds, environmental hazards |
| 3    | Far                | Fast regen, aggressive defenders, multiple emitters           |
| 4    | Remote             | Emitters relocate, coordinated cloud attacks, elite rewards   |

---

## 2. Tower Defense: Cloud Management

### 2.1 Tower Functions

Towers are the player's primary tool for holding territory within fog networks.

| Mode        | Power Cost | Effect                                 | Use Case                                     |
| ----------- | ---------- | -------------------------------------- | -------------------------------------------- |
| **Destroy** | High       | Permanently eliminates clouds in range | Establishing safe corridors                  |
| **Push**    | Low        | Repels clouds without destroying       | Temporary exploration, resource conservation |

### 2.2 Tower Placement Strategy

- Towers placed near network edges: safe, low yield
- Towers placed near center: high yield, triggers **angry cloud response**
- Players must balance aggression with defensive coverage

### 2.3 Angry Cloud Response

- Networks detect towers placed close to the emitter
- **Aggressive clouds** spawn and actively attack:
  - Thrust fog projectiles at the player
  - Attempt to overwhelm and destroy towers
  - Coordinate to box the player in
- Creates dynamic combat during network assault

### 2.4 Tower Upgrades

Towers can be upgraded to improve efficiency:

- **Range** – larger coverage area
- **Power efficiency** – reduced energy consumption
- **Destruction rate** – faster cloud elimination
- **Durability** – resistance to angry cloud attacks
- **Auto-targeting** – prioritizes threatening clouds

---

## 3. Exploration Tools

### 3.1 Fog Repulsor Spell

The player's key exploration ability:

- **Placeable** anywhere in the world
- Creates a **temporary safe zone** that pushes fog back
- Duration and radius upgradeable
- **Dual purpose**:
  - Scouting ahead to locate emitters and resources
  - Emergency escape when boxed in

### 3.2 Repulsor Resource Management

- Consumes **mana** or a craftable resource
- Cooldown or consumable limit prevents spam
- Strategic decision: scout aggressively or save for emergencies

### 3.3 Death and Recovery

- **Respawn location**: Town or nearest safe point
- **Potential death penalties** (choose one or combine):
  - Lose carried (unbanked) resources
  - Corpse run: dropped loot remains in fog, ticking clock to recover
  - Temporary stat debuff
- Fog damage is **gradual**, allowing a scramble window before death

---

## 4. Crystal Farming System

### 4.1 Resource Hierarchy

| Resource             | Acquisition                           | Abundance | Primary Use                 |
| -------------------- | ------------------------------------- | --------- | --------------------------- |
| **Crystal Shards**   | Breaking wild/farmed crystals         | Common    | Planting, basic crafting    |
| **Crystal Catalyst** | Harvesting wild crystals in fog zones | Abundant  | "Watering" growing crystals |
| **Crystal Cores**    | Extracting from wild crystal nexus    | Scarce    | Building projector slots    |
| **Power Shards**     | Destroying wild power crystals        | Limited   | Growing power crystals      |
| **Magic Essence**    | Harvesting mature crystals            | Variable  | Potions, advanced crafting  |
| **Raw Gems**         | Breaking mature crystals              | Variable  | Currency, ammunition        |

### 4.2 Core Projectors

The foundation of crystal farming:

- **Built by player**, placed in world
- Consume **crystal cores** to create **crystal beds**
- Each bed slot requires one core
- Beds allow planting of crystal shards

#### Projector Tiers

| Tier     | Bed Slots | Special Features                     |
| -------- | --------- | ------------------------------------ |
| Basic    | 4         | Standard growth                      |
| Advanced | 9         | Unlocks pattern bonuses              |
| Master   | 16        | Geometry arrangements, rare crystals |

#### Projector Upgrades

- **Yield increase** – more resources per harvest
- **Growth speed** – reduced maturation time
- **Auto-harvest** – automatically collects mature crystals
- **Catalyst efficiency** – less spraying required

### 4.3 The Spraying Mechanic

- Player selects **spraying spell**
- Circular **area indicator** shows affected region
- Crystals lacking catalyst appear **dull/colorless**
- Spraying restores **luminosity** progressively
- Fully sprayed crystals emit **visual/audio feedback** (glow, chime, particles)
- Spell upgrades increase spray radius
- Continuous spraying consumes catalyst (but catalyst is abundant)

### 4.4 Crystal Growth Stages

| Stage     | Visual                           | Interaction          |
| --------- | -------------------------------- | -------------------- |
| Planted   | Small dull shard                 | Requires catalyst    |
| Growing   | Increasing glow, texture changes | Continue spraying    |
| Mature    | Full luminosity, distinct form   | Ready for harvest    |
| Overgrown | Pulsing, unstable                | Bonus yield or risk? |

### 4.5 Geometry & Arrangement System

Advanced farming involves spatial puzzles:

- **Basic**: Any arrangement works
- **Intermediate**: Adjacent crystal types affect growth (synergy bonuses)
- **Advanced**: Specific patterns unlock rare crystal growth
  - Triangle formations
  - Ring arrangements
  - Spiral configurations
- **Mastery**: Hybrid patterns combining multiple rare types

### 4.6 Crystal Variety & Uses

| Crystal Type | Growth Difficulty            | Primary Use              |
| ------------ | ---------------------------- | ------------------------ |
| Common       | Easy                         | Currency, basic potions  |
| Elemental    | Medium                       | Magical ammunition       |
| Power        | Hard (requires power shards) | Network expansion        |
| Rare/Named   | Pattern-dependent            | Special crafting, quests |

---

## 5. Power Network System

### 5.1 The Player's Crystal Network

- Town contains an initial **power source**
- Player expands network by:
  - Destroying fog emitters (permanent power boost)
  - Tapping networks (ongoing power income)
  - Growing and harvesting power crystals

### 5.2 Power as Reach

Crystal power determines:

- **Tower range** – how far towers can project
- **Tower efficiency** – power cost of operations
- **Repulsor duration** – how long exploration spells last
- **Network boundary** – visible edge of player influence on map

### 5.3 Power Visualization

- Player's territory shown as **glowing network tendrils** on map
- Early game: small circle around town
- Late game: branching reach across multiple cleared cells
- Provides tangible visual progression

---

## 6. Survival Systems

### 6.1 Hunger

- Player must eat **2-3 times daily**
- Hunger affects:
  - Movement speed
  - Stamina regeneration
  - Possibly spell effectiveness
- Food sources: foraging, farming, cooking, purchasing

### 6.2 Mana Management

- Mana powers spells and abilities
- Regeneration is **slow naturally**
- **Crystal-crafted potions** restore mana quickly
- Creates demand for crystal farming output

### 6.3 Day/Night Cycle

- **Daytime**: Standard enemy difficulty
- **Nighttime**:
  - **Dark crystals** activate
  - Stronger enemies spawn
  - Fog may spread faster
  - Higher risk, potentially higher reward

### 6.4 Sleep Mechanic

- Sleeping restores health and provides buffs
- **Quality modifiers**:
  - Sleep while hungry → penalties (reduced stamina, debuffs)
  - Sleep well-fed → bonuses (regeneration, luck)
  - Sleep duration affects bonus strength
- Bed quality upgrades possible

---

## 7. Town Building & NPC Progression

### 7.1 Building System

- Construct buildings to provide services and attract NPCs
- Building types:
  - **Functional**: Storage, crafting stations, defenses
  - **Residential**: NPC housing
  - **Commercial**: Shops, services
  - **Magical**: Crystal processing, power amplifiers

### 7.2 NPC Attraction & Roles

| NPC Type  | Attraction Condition | Services Provided                          |
| --------- | -------------------- | ------------------------------------------ |
| Merchant  | Build shop           | Buying/selling, introduces core projectors |
| Alchemist | Build lab            | Potion crafting, catalyst processing       |
| Smith     | Build forge          | Tool/weapon upgrades                       |
| Scholar   | Build library        | Research, pattern recipes                  |
| Guard     | Build barracks       | Town defense, expeditions                  |

### 7.3 Town Advancement

- Town has a **renown/level** system
- Advancement unlocks:
  - New building types
  - Higher-tier NPCs
  - Expanded services
  - Quest lines

### 7.4 Resource Management

- **Supply lines**: Connect cleared networks to town
- **Storage capacity**: Limits on held resources
- **Upkeep costs**: Some buildings consume resources

### 7.5 Projector Placement Conflict Resolution

Since projectors can be placed anywhere but NPCs need specific plots:

- **Option A**: Show ghost outlines of reserved NPC building locations
- **Option B**: Projectors are relocatable (costs resources)
- **Option C**: Distinct town zone vs. farming zone boundaries
- **Option D**: NPCs negotiate/request relocation when needed

---

## 8. Macro Progression Systems

### 8.1 Network Tier Progression

- World contains networks of escalating difficulty
- Clearing Tier N networks reveals locations of Tier N+1
- Higher tiers yield:
  - More power per emitter
  - Rarer crystal types
  - Unique cores for special projectors

### 8.2 Core Depth Excavation (Dungeon System)

Cleared networks unlock **dungeon access**:

- Each destroyed emitter reveals an entrance to **core depths**
- Depths have **multiple floors** with increasing difficulty
- Progression through floors provides:
  - Rare crafting materials
  - Unique crystal shards
  - Lore/story elements
  - Permanent upgrades

#### Depth Structure

| Floor Range | Difficulty | Rewards                          |
| ----------- | ---------- | -------------------------------- |
| 1-10        | Easy       | Common resources, tutorials      |
| 11-25       | Medium     | Rare shards, pattern blueprints  |
| 26-50       | Hard       | Power shards, unique cores       |
| 51+         | Extreme    | Legendary items, endgame content |

### 8.3 The Central Rift (Long-Horizon Goal)

- A single **mega-dungeon** located on the map
- Requires keys crafted from specific crystals/cores to descend
- Represents the ultimate challenge
- Contains:
  - Deepest lore
  - Most powerful rewards
  - Potential "ending" or prestige reset

### 8.4 Progression Visualization

- **Map**: Networks cleared, tendrils of power visible
- **Town**: Growing from single shelter to thriving settlement
- **Farm**: Expanding projector arrays, complex patterns
- **Depths**: Floor counter, achievements displayed

---

### 9.4 Defense Requirements

#### Tower Scaling

- Tower effectiveness scales primarily with **gem power**
- Early game: basic gems suffice for fog management
- Late game: **high-tier gems required** to damage invasion forces
- Creates demand for advanced crystal farming and rare gem production

#### Spell Scaling

- Combat spells also scale with gem power
- Player's personal combat effectiveness tied to gem quality
- Encourages active defense participation, not just tower reliance

#### Gem Tier Requirements (Example)

| Assault Level | Minimum Gem Tier | Source                   |
| ------------- | ---------------- | ------------------------ |
| 1-3           | Common           | Basic farming            |
| 4-6           | Uncommon         | Pattern farming          |
| 7-10          | Rare             | Depth excavation         |
| 11+           | Legendary        | Rift drops, boss rewards |

### 9.5 Strategic Implications

#### Base Layout Matters

- Enemies path straight to center
- Player must design **kill corridors** with overlapping tower coverage
- Chokepoints become valuable
- Town layout shifts from aesthetic to strategic

#### Resource Allocation Tension

- Spend gems on expansion (more power = harder enemies) OR
- Stockpile gems for defense (slower growth but safer)
- High-tier gems are **scarce**—can't do everything

#### The Growth Paradox

Early game: "I need more power to explore further"
Late game: "More power makes enemies stronger, but I need it to fight them"

### 9.6 Fail State

- If enemies reach the town center and destroy the **core structure**: **GAME OVER**
- This is the player's first real loss condition
- Early game is essentially safe (tutorial/learning phase)
- Late game introduces genuine stakes and tension

### 9.7 Assault Structure Example

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

### 9.8 Design Considerations

#### Telegraphing

- Give players **advance warning** of incoming assaults
- Show enemy base location on map
- Display estimated wave strength
- Allow preparation time

#### Catch-Up Mechanics

- If player falls behind power curve, options:
  - Mercenary NPCs for hire (temporary defense boost)
  - Desperate measures (sacrifice buildings for burst power)
  - Tactical retreats (lose outer territory to consolidate)

#### Victory Condition?

- Does repelling enough assaults lead to a final confrontation?
- Possible: after X assaults, locate and assault the **enemy origin point**
- Destroying the origin ends the invasion threat (alternate endgame to the Rift)

---

## 10. Core Loop Summary

### 10.1 Moment-to-Moment (Minutes)

```
Spray crystals → Harvest mature crops → Manage hunger/mana → Tend farm
```

### 10.2 Session Loop (Hours)

```
Plan network assault → Deploy towers → Push toward emitter →
Harvest wild resources → Destroy emitter → Bank resources →
Expand farm with new cores → Upgrade equipment
```

### 10.3 Campaign Loop (Days/Weeks)

```
Clear network tier → Gain power → Reach new tier →
Descend depths for rare materials → Advance town →
Unlock new crystal types → Tackle harder content →
Progress toward Central Rift
```

### 10.4 The Virtuous Spiral

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

---

## 11. Open Design Questions

1. **Corpse Run vs. Resource Loss**: Which death penalty fits the intended difficulty curve?

2. **Tap vs. Destroy**: What makes a network tappable? Player choice or network type?

3. **Night Incentives**: What rewards justify the risk of nighttime exploration?

4. **Pattern Discovery**: How do players learn geometry recipes? Experimentation, NPCs, or loot?

5. **Power Ceiling**: Is there a maximum power level, or does scaling continue infinitely?

6. **Multiplayer Potential**: Could networks be contested between players, or is this strictly single-player?

7. **Seasonal Events**: Do fog networks behave differently during in-game seasons or events?

8. **Invasion Trigger Visibility**: Should players know the power threshold that triggers invasions, or is it a surprise?

9. **Sandbagging Prevention**: How strictly should historical max power be tracked? What if players intentionally avoid growth?

10. **Assault Frequency Tuning**: How long between assaults? Too short = exhausting. Too long = forgettable.

11. **Partial Failure States**: Can players lose outer buildings/territory without full game over? Comeback potential?

12. **Enemy Variety**: Do invasion forces have different unit types requiring different defenses, or is it purely a power check?

13. **Endgame Resolution**: Does defeating the invasion source provide a "win" state, or does the game continue indefinitely?

---

## Appendix: Terminology Reference

| Term                     | Definition                                                          |
| ------------------------ | ------------------------------------------------------------------- |
| **Fog Network**          | A hostile cell controlled by crystal formations that produce fog    |
| **Fog Emitter**          | The central "boss" structure that powers a network                  |
| **Crystal Bed**          | A plantable slot created by core projectors                         |
| **Core Projector**       | Player-built structure that creates crystal beds                    |
| **Catalyst**             | Abundant resource used to "water" growing crystals                  |
| **Power Crystal**        | Special crystals that expand the player's network reach             |
| **Angry Clouds**         | Aggressive fog defenders that attack players near emitters          |
| **Core Depths**          | Dungeon floors accessible beneath cleared networks                  |
| **The Rift**             | Endgame mega-dungeon requiring special keys                         |
| **Invasion**             | Late-game assault system triggered by high power output             |
| **Historical Max Power** | The highest power level ever achieved; determines invasion scaling  |
| **Assault**              | A series of enemy waves launched from an outskirt base              |
| **Gem Power**            | Stat derived from gem quality that scales tower/spell effectiveness |
