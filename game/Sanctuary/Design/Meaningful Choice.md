---
tags:
  - sanctuary/design
  - framework
---

# Meaningful Choice

> *"A game is a series of meaningful choices."* — Sid Meier

A choice is meaningful when it has **clear trade-offs**, **no obviously dominant option**, and **consequences that persist**. Sanctuary structures its core decisions around resource scarcity, risk management, and irreversible commitment.

---

## Decision Matrices

### Tap vs. Destroy Networks

When encountering a [[Sanctuary/Crystals/Crystal Power & Networks#Crystal Networks|crystal network]], the player chooses:

| | **Tap** | **Destroy** |
|---|---------|-------------|
| **Power Income** | Ongoing, moderate | One-time large yield + crystal cores |
| **Danger** | Reduced fog, some danger persists | Network fully cleared |
| **Maintenance** | Requires periodic defense | None after clearance |
| **When Optimal** | Mid-game, when not strong enough for full clearance | Late game, or when cores are critical |
| **Unlocks** | Steady power for expansion | [[Sanctuary/Progression/Core Depths|Core Depths]] dungeon entrance |

See [[Sanctuary/Crystals/Crystal Power & Networks#Network Tapping (Alternative to Destruction)|Network Tapping]].

**Design intent:** This prevents a single "always destroy" strategy and rewards reading the current game state.

---

### Expand vs. Defend (Resource Allocation Tension)

The player's crystal power, gems, and cores must be allocated between growth and survival:

| | **Expand** | **Defend** |
|---|-----------|------------|
| **Spend crystals on** | Projectors, farms, relays | [[Sanctuary/Combat/Tower System|Towers]], armor, potions |
| **Risk** | Weak defense → assault damage → progress reset | Slow growth → fall behind the scaling curve |
| **Feedback loop** | [[Sanctuary/Design/Feedback Loops#Crystal Farming Growth|Crystal farming growth]] accelerates | [[Sanctuary/Design/Feedback Loops#Fog Aggression Scaling|Fog aggression]] stays manageable |
| **Fail condition** | Core structure destroyed ([[Sanctuary/Combat/Combat & Defense|game over]]) | Stagnation; unable to reach higher tiers |

**The Growth Paradox in action:** Neither pure expansion nor pure defense is viable. The optimal path requires continuously balancing both — and the balance point *shifts* as monster scaling responds to the player's choices.

---

### Tower Mode: Destroy vs. Push

[[Sanctuary/Combat/Tower System|Towers]] operate in two modes:

| | **Destroy Mode** | **Push Mode** |
|---|-----------------|---------------|
| **Power Cost** | High | Low |
| **Effect** | Permanently eliminates fog clouds | Temporarily repels fog clouds |
| **When Optimal** | Committed expansion into a network | Temporary safe corridor for farming/exploration |
| **Risk** | High power drain reduces other capabilities | Fog returns — no permanent progress |

**Design intent:** Prevents towers from being a one-size-fits-all solution. The player must read the situation: am I committing to this area, or just passing through?

---

### Crystal Geometry Specialisation

[[Sanctuary/Crystals/Crystal Growing|Crystal farming]] rewards specific arrangements:

| Geometry Tier | Arrangement | Reward |
| ------------- | ----------- | ------ |
| Basic | Any placement | Standard growth |
| Intermediate | Adjacency synergy | Bonus yields |
| Advanced | Triangles, rings, spirals | Rare crystal types |
| Mastery | Hybrid patterns | Unique resources, quest items |

**The choice:** Specialising in advanced geometry requires [[Sanctuary/Crystals/Crystal Growing|Master-tier projectors]] (16 bed slots) and deep knowledge of pattern mechanics. The player must decide:
- **Breadth** — many Basic/Advanced projectors for volume
- **Depth** — fewer Master projectors for rare resources

Rare crystals from advanced geometry gate [[Sanctuary/Progression/Core Depths|Core Depths]] materials and endgame crafting, so this choice has long-term consequences.

---

### Active vs. Passive Defense

The [[Sanctuary/Combat/Combat & Defense|assault system]] can be managed through different defensive postures:

| | **Active Defense** | **Passive Defense** |
|---|-------------------|---------------------|
| **Approach** | Player-controlled spells and positioning | Tower networks and NPC mercenaries |
| **Resource Cost** | Mana potions, armor, player time | Crystal power, gems, building materials |
| **Advantage** | Flexible, responsive | Autonomous, frees player for other tasks |
| **Risk** | Player death loses carried resources | Tower failure can cascade |

**Design intent:** Neither approach is sufficient alone. The 21-day assault cycle demands a mix — and the mix changes as assault tiers increase.

---

### Endgame Path: Rift vs. Invasion Origin

The ultimate fork in [[Sanctuary/Progression/Central Rift|Sanctuary's endgame]]:

| | **The Rift** | **Invasion Origin** |
|---|-------------|---------------------|
| **Type** | Mega-dungeon descent | Surface assault on enemy source |
| **Prereq** | Keys crafted from [[Sanctuary/Progression/Core Depths|Core Depths]] materials + high-tier fog network materials | Repelling successive assault waves |
| **Gameplay** | Exploration, lore, boss encounters | Tower defense, army coordination |
| **Reward** | Deepest lore, most powerful items | Eliminate the assault threat entirely |
| **Replayability** | Each descent requires a new key | One-time climactic battle |
| **Prestige** | Potential prestige reset | Campaign resolution |

**Design intent:** Two endgame paths serve different player archetypes — explorers/lore-seekers vs. builders/strategists. Both are valid "endings" with distinct rewards, preventing a single optimal route.

---

## The Growth Paradox as Central Tension

All of the above decisions orbit a single strategic question:

> **How aggressively should I grow, given that growth itself creates danger?**

This is the [[Sanctuary/Design/Feedback Loops#The Growth Paradox|Growth Paradox]] — and it is *by design* the question the player must answer differently in every session, at every tier, with every resource decision. It cannot be "solved" because the variables (monster scaling, resource distribution, network layout) change continuously.

A game where growth is purely beneficial becomes boring once the player snowballs. A game where growth is purely punished feels stagnant. Sanctuary's insight is that growth should be **simultaneously rewarding and threatening** — and the player's skill lies in navigating that tension.

---

## Related

- [[Sanctuary/Design/Design Framework|Design Framework]]
- [[Sanctuary/Design/Constraints|Constraints]]
- [[Sanctuary/Design/Feedback Loops|Feedback Loops]]
- [[Sanctuary/Design/Progression Tiers|Progression Tiers]]
