---
tags:
  - sanctuary/design
  - framework
aliases:
  - Ludological Framework
---

# Design Framework

> *"Play is free movement within a more rigid structure."*
> — Katie Salen & Eric Zimmerman, *Rules of Play*

This section provides a **ludological overlay** on Sanctuary's game systems — analysing *how* the rules, constraints, and feedback loops create meaningful play, rather than *what* each system does. It cross-cuts every implementation area in the vault.

---

## The Magic Circle

In Sanctuary, the **magic circle** — the boundary between the game world and the outside — is made literal by the [[Sanctuary/Combat/Fog System|Fog System]].

- **The fog is the boundary of play.** Everything outside the player's cleared zone is hostile, unknown, and mechanically inaccessible.
- **The player's network is the expanding safe zone.** Each cleared [[Sanctuary/Crystals/Crystal Power & Networks|crystal network]] extends the magic circle outward.
- **Crossing the boundary has real cost.** Fog damage, [[Sanctuary/Combat/Fog System#Boxing-In Mechanic|boxing-in]], and resource loss create genuine stakes at the frontier.
- **The boundary fights back.** [[Sanctuary/Combat/Fog System#Fog Network Aggression|Fog aggression]] and the [[Sanctuary/Combat/Combat & Defense|assault system]] mean the boundary is not passive — it actively resists expansion.

The result: the magic circle is not a metaphor but a *core mechanic*. The entire game is about expanding your circle of safety and influence against a world that pushes back.

---

## Mechanical Verbs

Every game can be distilled to its **core verbs** — the atomic actions available to the player. Sanctuary's verbs are:

| Verb | Primary System | Description |
| ---- | -------------- | ----------- |
| **Spray** | [[Sanctuary/Crystals/Crystal Growing|Crystal Growing]] | Plant and water crystals using the spraying mechanic |
| **Repel** | [[Sanctuary/Combat/Fog System#Traversal|Fog Traversal]] | Push back fog with spells, towers, and buildings |
| **Excavate** | [[Sanctuary/Progression/Core Depths|Core Depths]] | Descend dungeons beneath destroyed emitters |
| **Harvest** | [[Sanctuary/Crystals/Crystal Interaction|Crystal Interaction]] | Break or harvest crystals for gems and essence |
| **Build** | [[Sanctuary/Town/Buildings|Buildings]] / [[Sanctuary/Combat/Tower System|Tower System]] | Construct town infrastructure and defensive towers |
| **Export** | [[Sanctuary/Economy/Export Import System|Export Import System]] | Ship gems through the portal for upgrades and imports |

These verbs interlock through the [[Sanctuary/Core Loops/Core Game Loops|Core Game Loops]]: Spray → Harvest → Build → Repel → Excavate → Export → (repeat at higher tier).

---

## Design Pillars

### 1. Growth Creates Danger
The [[Sanctuary/Design/Feedback Loops#The Growth Paradox|Growth Paradox]] is Sanctuary's defining tension. Every investment in crystal farming simultaneously increases the player's power *and* the world's hostility. This ensures that progress never feels safe — there is always a new threat scaling to meet the player.

### 2. Territory as Progression
Unlike level-based or XP-based progression, Sanctuary makes **physical space on the map** the primary measure of progress. Clearing [[Sanctuary/Crystals/Crystal Power & Networks#Crystal Networks|crystal networks]], extending [[Sanctuary/Crystals/Crystal Power & Networks#Power as Reach|power reach]], and building [[Sanctuary/Town/Town Progression|town infrastructure]] all manifest as visible territorial gain.

### 3. Scarcity Drives Choice
[[Sanctuary/Design/Constraints|Constraints]] — especially [[Sanctuary/Progression/Food System|food scarcity]], [[Sanctuary/Crystals/Crystal Power & Networks#Central Command Point|power caps]], and [[Sanctuary/Crystals/Crystal Growing#Resource Hierarchy|crystal core rarity]] — ensure that the player cannot do everything at once. Every resource spent on one system is unavailable to another, creating the [[Sanctuary/Design/Meaningful Choice|meaningful choices]] that sustain engagement.

### 4. Layered Complexity
The game [[Sanctuary/Design/Learning Patterns|teaches progressively]] — from safe tutorial fog networks to the full tower-defense assault system. Each [[Sanctuary/Design/Progression Tiers|tier]] introduces new mechanics on top of mastered ones, following Koster's principle that fun comes from *learning patterns*.

---

## Design Notes

- [[Sanctuary/Design/Constraints|Constraints]] — What limits and pressures shape play
- [[Sanctuary/Design/Feedback Loops|Feedback Loops]] — Virtuous spirals and balancing mechanics
- [[Sanctuary/Design/Meaningful Choice|Meaningful Choice]] — Decision matrices and strategic tensions
- [[Sanctuary/Design/Progression Tiers|Progression Tiers]] — Consolidated tier reference
- [[Sanctuary/Design/Learning Patterns|Learning Patterns]] — How the game teaches mechanics

---

## Related

- [[Sanctuary/Core Loops/Core Game Loops|Core Game Loops]]
- [[Sanctuary/Core Loops/Progression Systems|Progression Systems]]
- [[Sanctuary/Sanctuary Hub|Sanctuary Hub]]
