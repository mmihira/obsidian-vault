---
tags:
  - sanctuary/design
  - framework
---

# Constraints

> *"Games are defined not by their freedoms but by their limitations."*

Constraints are what transform free-form interaction into a *game*. Every constraint in Sanctuary serves a design purpose: forcing trade-offs, creating tension, or gating content behind mastery.

---

## Environmental Constraints

### Fog Damage & Boxing-In
- The [[Sanctuary/Combat/Fog System|fog]] deals continuous damage to players inside it
- Fog restores behind the player during exploration, creating the [[Sanctuary/Combat/Fog System#Boxing-In Mechanic|boxing-in mechanic]]
- Risk/reward tension: push deeper for resources vs. maintaining escape routes
- Fog damage **intensifies at night** ([[Sanctuary/World/Day Night Cycle|Day Night Cycle]])

### Crystal Network Barriers
- [[Sanctuary/Crystals/Crystal Power & Networks#Crystal Networks|Crystal networks]] compartmentalise the map into cells
- [[Sanctuary/Crystals/Crystal Power & Networks#Crystal Network Nexus Gate|Nexus gates]] act as hard barriers requiring significant combat investment to break
- [[Sanctuary/Crystals/Crystal Overview|Crystal filament]] impedes movement and protects network cores

### Crystal Wall
- The [[Sanctuary/Map/Crystal Wall|Crystal Wall]] is a massive living barrier blocking northward progression
- A nexus on the far side continuously repairs damage
- Only a narrow weak point can be attacked — the first major tower-defense challenge

### Map Boundaries
- Southern edge blocked, sides bordered by oceans and mountains ([[Sanctuary/Map/Map Overview|Map Overview]])
- Enemy difficulty scales with distance from town
- Natural terrain barriers (fissures, [[Sanctuary/Map/Impassable River|Impassable River]], [[Sanctuary/Map/Mountain Tunnel|Mountain Tunnel]]) funnel exploration

---

## Resource Scarcity

### Food
- Food **does not grow in Sanctuary** ([[Sanctuary/Progression/Food System|Food System]])
- Must be imported via the [[Sanctuary/Economy/Export Import System|exporter]] — initially only 1 day's supply per morning
- Hunger penalties escalate: movement speed → mana consumption → unplayable
- Food scarcity is the primary constraint on exploration range until late game
- Buying from [[Sanctuary/Town/NPC System|townspeople]] is limited; true farming unlocks very late

### Power Cap
- The [[Sanctuary/Crystals/Crystal Power & Networks#Central Command Point|Central Command Point]] caps total power production
- Must be upgraded by supplying accumulated power
- Attack fog clouds target this structure — damage resets current progress
- Creates a ratcheting tension: invest power to level up, or stockpile as a safety buffer

### Crystal Cores
- [[Sanctuary/Crystals/Crystal Growing|Crystal cores]] are **scarce** — extracted only from destroyed nexus gates
- Required to build [[Sanctuary/Crystals/Crystal Growing|projector slots]] for crystal farming
- Every core spent on farming is a core not spent on other infrastructure

### Power Shards
- Obtained by destroying wild [[Sanctuary/Crystals/Crystal Types & Structures|power crystals]] guarded by monsters
- Required to grow power crystals — the backbone of the energy network
- Limited supply creates a gating mechanic on network expansion

---

## Combat Constraints

### Monster Scaling
- Monster frequency and power scales with the number of cultivated [[Sanctuary/Crystals/Crystal Types & Structures#Power Crystals|crystal patches]] ([[Sanctuary/Combat/Combat & Defense|Combat & Defense]])
- Monsters actively **seek out crystal farms** to grow bigger
- Creates the [[Sanctuary/Design/Feedback Loops#The Growth Paradox|Growth Paradox]]: farming makes you stronger *and* enemies harder

### Tower Power Consumption
- [[Sanctuary/Combat/Tower System|Towers]] consume crystal power — the same resource used for farming and building
- Destroy mode is powerful but expensive; Push mode is cheap but temporary
- Defensive infrastructure directly competes with economic infrastructure

### Core Structure Vulnerability
- If the central command point takes enough damage from [[Sanctuary/Combat/Fog System#Fog Network Aggression|attack fog clouds]], current progress **resets**
- If enemies destroy the core structure, it is **game over** ([[Sanctuary/Combat/Combat & Defense|Combat & Defense]])
- The ultimate constraint: there is a real fail state

### Armor Depletion
- [[Sanctuary/Combat/Armor System|Armor]] is **consumable** — it cannot be regenerated once applied
- Application takes time and can be interrupted
- Forces forward planning: armor must be crafted and equipped *before* entering danger

---

## Temporal Constraints

### Day/Night Cycle
- [[Sanctuary/World/Day Night Cycle|Night]] activates [[Sanctuary/Crystals/Crystal Types & Structures#Dark Crystals|dark crystals]], spawning stronger enemies
- Fog becomes more intense and damaging at night
- Exploration at night is significantly more dangerous — creating natural session rhythms

### Sleep Requirements
- Sleep always ends at 6 AM — player cannot control wake time
- Less than 6 hours of sleep imposes penalties
- Full stomach grants sleep bonuses; being famished prevents recovery and XP gain
- Forces a daily checkpoint/reset cycle

### Hunger Timer
- Player must eat 2–3 times daily ([[Sanctuary/Core Loops/Survival|Survival]])
- Hunger is a **ticking clock** that limits how long the player can stay in the field
- Combined with food scarcity, this is the primary constraint on early-game exploration range

---

## Knowledge Constraints

### Skill Gating via Variation Routes
- Some [[Sanctuary/Progression/Skill Perk Tree|skills]] are locked behind successfully routing [[Sanctuary/Combat/Fog System#Variation System|fog variation sources]]
- Variant fog drops are required to advance up the skill tree
- [[Sanctuary/Combat/Spells/Elemental Essence System|Elemental essences]] extracted via the variant system gate spell crafting
- This constraint ensures players engage with fog networks as puzzles, not just obstacles

### Knowledge Gain Throttling
- Unused [[Sanctuary/Progression/Knowledge System|skill points reduce knowledge gain]] — an anti-hoarding mechanic
- Forces players to commit to specialisation rather than banking options
- Mana pool upgrades have exponentially decreasing returns

---

## How Constraints Interact

The power of Sanctuary's constraint system is in how constraints **compound**:

1. **Food + Fog** → You can't explore indefinitely; you must return to town or die
2. **Power Cap + Monster Scaling** → You can't safely grow without upgrading defenses first
3. **Crystal Cores + Tower Power** → Building farms and building towers compete for the same bottleneck resource
4. **Day/Night + Hunger** → Night forces retreat, sleep requires food, food requires exports
5. **Variation Routes + Skill Gating** → Engaging fog as a puzzle (not just a wall) is required for character growth

These intersecting constraints create the **possibility space** within which [[Sanctuary/Design/Meaningful Choice|meaningful choices]] emerge.

---

## Related

- [[Sanctuary/Design/Design Framework|Design Framework]]
- [[Sanctuary/Design/Feedback Loops|Feedback Loops]]
- [[Sanctuary/Design/Meaningful Choice|Meaningful Choice]]
