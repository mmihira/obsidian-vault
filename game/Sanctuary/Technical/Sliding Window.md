---
tags:
  - sanctuary/technical
---

# Sliding Window Implementation

## Entity Simulation

- Entities are only simulated in certain **world chunks**, not the entire world
- When entities are removed from the registry, their data is saved in a standard format for later loading
- Use entt's archive functions to persist and restore entities

## World Grid

- The world uses a grid for tiles and generation, but entities do not have to fit this grid
- Collision can be checked by comparing all entities, or by using **spatial partitioning** for better performance
- A grid is also needed for pathfinding, with a minimum size of **16×16 pixels**

## Always-Simulated Entities

- Some chunks and entities are **always simulated**
- There is a global registry for these always-simulated entities
- Their data is passed to local entities when they come into view
- If a global entity's chunk is active, update its components in the current registry

## Related

- [[Sanctuary/Map/Map Overview|Map Overview]]
