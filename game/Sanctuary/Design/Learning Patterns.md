---
tags:
  - sanctuary/design
  - framework
---

# Learning Patterns

> *"Fun is just another word for learning."* — Raph Koster, *A Theory of Fun*

Sanctuary teaches its mechanics through **progressive disclosure** — introducing systems one at a time in controlled environments before combining them in the open world. This note maps how the game scaffolds complexity across early, mid, and late game.

---

## Early Game: Safe Foundation

### Tutorial Fog Networks
- The first fog networks are **small and tutorial-sized** ([[Sanctuary/Combat/Fog System#Fog Network Aggression|Fog System]])
- Slow fog regeneration, passive defenders, single emitter (Tier 1)
- [[Sanctuary/Crystals/Crystal Power & Networks#Crystal Network Nexus Gate|Nexus gate priests]] initially ignore some hexagons so the player is not overwhelmed
- Teaches: fog damage, fog clearing, boxing-in risk, basic resource gathering

### Safe Zone Establishment
- Player starts with a small cleared area around town ([[Sanctuary/Crystals/Crystal Power & Networks#Power Visualization|Power Visualization]])
- Early power network is a tiny circle — tangible baseline for growth
- [[Sanctuary/Map/Map Overview|Southern edge blocked]], creating a natural northward funnel
- Teaches: territory as progression, power as reach

### NPC Introductions
- [[Sanctuary/Town/NPC System|NPCs]] introduce systems through guided interactions
- Merchant NPC arrives with a [[Sanctuary/Crystals/Crystal Growing|core machine deployed for potions]] — the player's first exposure to crystal farming
- [[Sanctuary/Town/Buildings|Portal Comms Building]] is deliberately easy to build because it introduces world map expansion and the [[Sanctuary/Economy/Export Import System|export system]]
- Keeping the [[Sanctuary/Town/NPC System|cooking pot]] filled is the first town management task — simple, repeatable, with clear feedback
- Teaches: NPC economy, crystal farming basics, export loop

### Food as Exploration Leash
- [[Sanctuary/Progression/Food System|Food scarcity]] limits how far the player can stray from town
- Only 1 day's supply imported each morning — a natural tether
- The player *feels* the constraint before understanding the system
- Teaches: resource management, return-to-base rhythm, export upgrade motivation

---

## Mid Game: Mechanical Depth

### Crystal Wall Tower Defense Introduction
- The [[Sanctuary/Map/Crystal Wall|Crystal Wall]] is Sanctuary's first **major tower defense challenge**
- A massive living crystal barrier with a nexus that continuously repairs damage
- Only a narrow weak point exists — forces strategic tower positioning
- Monster attack frequency scales with cultivated crystal patches (first encounter with the [[Sanctuary/Design/Feedback Loops#The Growth Paradox|Growth Paradox]])
- Teaches: tower placement strategy, Destroy vs. Push modes, defense-as-investment

### Geometry Farming
- [[Sanctuary/Crystals/Crystal Growing|Crystal geometry]] unlocks progressively:

| Stage | Skill Level | Pattern | Reward |
| ----- | ----------- | ------- | ------ |
| Basic | Beginner | Any arrangement | Standard growth |
| Intermediate | Practiced | Adjacency synergy | Bonus yields |
| Advanced | Experienced | Triangles, rings, spirals | Rare crystal types |
| Mastery | Expert | Hybrid patterns | Unique resources |

- Each stage builds on understanding from the previous one
- Advanced projectors (9 → 16 bed slots) physically expand the design space
- Teaches: pattern recognition, spatial reasoning, long-term planning

### Assault Telegraphing
- The [[Sanctuary/Combat/Combat & Defense|21-day assault cycle]] introduces structured threat
- Telegraphing gives **advance warning** before waves arrive
- Early assaults (Level 1–3) use Common gem tier — manageable with basic defenses
- Teaches: preparation cycles, resource stockpiling, defensive infrastructure

### Fog Variation as Puzzle
- [[Sanctuary/Combat/Fog System#Variation System|Variation routers]] at hexagon intersections modify fog behaviour
- Player learns to read variation sources and route them intentionally
- Drops gate [[Sanctuary/Progression/Skill Perk Tree|skill tree]] advancement — clear incentive to engage
- Teaches: fog networks as interactive systems (not just obstacles), variation routing as a strategic mini-game

---

## Late Game: Mastery Challenges

### Assault Escalation
- Assault levels 7–10 require **Rare gems** from [[Sanctuary/Progression/Core Depths|Core Depths]] floor 26+
- Level 11+ requires **Legendary gems** — Rift drops or boss rewards
- Full tower defense with waves from map outskirts
- Catch-up mechanics exist: [[Sanctuary/Town/NPC System|mercenary NPCs]], building sacrifice for burst power, tactical retreat
- Teaches: system mastery, multi-front defense, resource triage under pressure

### Endgame Path Selection
- Two paths diverge: [[Sanctuary/Progression/Central Rift|The Rift]] mega-dungeon vs. [[Sanctuary/Combat/Combat & Defense|Invasion Origin]] surface assault
- Each path tests different skill sets (exploration vs. tower defense)
- Both require mastery of all prior systems
- Teaches: strategic identity, long-term commitment, replayability through alternative paths

### Inherently Aggressive Networks
- Late-game fog networks are **inherently aggressive once discovered** ([[Sanctuary/Combat/Fog System#Fog Network Aggression|Fog System]])
- No grace period — the network attacks immediately
- Requires proactive defense before exploration
- Teaches: reading the environment, pre-planning, risk assessment at a glance

---

## Feedback Systems

### Visual Feedback

| System | Visual Cue | What It Communicates |
| ------ | ---------- | -------------------- |
| [[Sanctuary/Crystals/Crystal Growing|Crystal Growth]] | Dull → Increasing glow → Full luminosity → Pulsing/unstable | Growth stage (Planted → Growing → Mature → Overgrown) |
| [[Sanctuary/Crystals/Crystal Growing|Spraying]] | Area indicator + luminosity change | Spray coverage and crystal response |
| [[Sanctuary/Crystals/Crystal Power & Networks#Power Visualization|Power Network]] | Glowing tendrils on map | Territory extent and progression |
| [[Sanctuary/Combat/Fog System|Fog Intensity]] | Cloud density and movement speed | Network aggression level |
| [[Sanctuary/Town/Town Progression|Town]] | Shelter → settlement → thriving town | Macro progression milestone |
| [[Sanctuary/Crystals/Crystal Power & Networks#Central Command Point|Command Point]] | Size and glow intensity | Power level and vulnerability |

### Audio Feedback
- Crystal growth stages produce distinct audio cues ([[Sanctuary/Crystals/Crystal Growing|Crystal Growing]])
- Spraying mechanic has responsive sound design for coverage feedback
- Fog intensity changes ambient audio — a passive danger indicator

### Systemic Feedback
- Monster scaling is **visible** — the player sees more monsters near larger farms
- [[Sanctuary/Combat/Combat & Defense|Assault telegraphing]] provides explicit warning
- [[Sanctuary/Progression/Knowledge System|Knowledge gain reduction]] when hoarding skill points — gentle nudge to commit
- Overgrown crystals pulse and become unstable — risk/reward made visible

---

## Scaffolded Complexity Model

```
MASTERY    ┃ Rift descent, Invasion Origin, hybrid geometry,
           ┃ inherently aggressive networks, Legendary gem crafting
           ┃
ADVANCED   ┃ Assault defense (7+), advanced geometry, Core Depths 26+,
           ┃ endgame path selection, multi-front fog management
           ┃
INTERMEDIATE ┃ Crystal Wall, tower modes, geometry farming, assault cycles,
           ┃ variation routing, NPC self-sustenance
           ┃
BASIC      ┃ Tutorial fog, safe zone, crystal spraying, food rhythm,
           ┃ first NPC, export loop, cooking pot
           ┃
           ┗━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
             EARLY GAME ──────► MID GAME ──────► LATE GAME
```

Each layer **requires** mastery of the layer below it. The game does not gate content with arbitrary level requirements — instead, the *systems themselves* create natural gates:
- You can't clear Tier 3 networks without understanding tower defense (learned at the Crystal Wall)
- You can't farm rare crystals without understanding geometry (learned through progressive projector tiers)
- You can't survive Assault 7+ without understanding the Growth Paradox (learned through mid-game scaling)

This is Koster's principle in action: **fun comes from learning new patterns**, and Sanctuary ensures there is always a new pattern to learn.

---

## Related

- [[Sanctuary/Design/Design Framework|Design Framework]]
- [[Sanctuary/Design/Progression Tiers|Progression Tiers]]
- [[Sanctuary/Design/Constraints|Constraints]]
- [[Sanctuary/Design/Feedback Loops|Feedback Loops]]
