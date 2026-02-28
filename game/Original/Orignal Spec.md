# SANCTUARY

<!-- mtoc-start -->

  * [World building](#world-building)
  * [Backstory](#backstory)
  * [Core game loops](#core-game-loops)
    * [Labour value theory](#labour-value-theory)
      * [Resource gathering](#resource-gathering)
      * [Crystal Farming & Production](#crystal-farming--production)
    * [Spatial progress, exploration and expansion](#spatial-progress-exploration-and-expansion)
      * [Survival](#survival)
    * [Progression systems](#progression-systems)
      * [**Combat & Defense**](#combat--defense)
      * [**Town Building & NPC Progression**](#town-building--npc-progression)
      * [*](#)
  * [Initial beats](#initial-beats)
  * [Gameloop](#gameloop)
  * [Progression trees](#progression-trees)
  * [Health/Mana system](#healthmana-system)
    * [Health system](#health-system)
    * [Mana system](#mana-system)
  * [Food System](#food-system)
  * [Initial items](#initial-items)
    * [Raw gem](#raw-gem)
    * [GemWood](#gemwood)
    * [GemPlanks](#gemplanks)
    * [WardSteel](#wardsteel)
    * [Magic essence](#magic-essence)
    * [Condensed gem sheet](#condensed-gem-sheet)
  * [Crystals](#crystals)
    * [Wild crystal lifecyle](#wild-crystal-lifecyle)
    * [Crystal growing mechanism](#crystal-growing-mechanism)
      * [Overview](#overview)
      * [Spraying mechanic](#spraying-mechanic)
      * [Crystal cores](#crystal-cores)
      * [Core projector](#core-projector)
      * [Growth feedback](#growth-feedback)
      * [Variety](#variety)
      * [Value](#value)
    * [Natural Crystal strucures](#natural-crystal-strucures)
      * [Power crystals](#power-crystals)
      * [Raw crystals](#raw-crystals)
      * [Dark Crystals](#dark-crystals)
      * [Crystal catalyst](#crystal-catalyst)
    * [Crystal power](#crystal-power)
    * [Crystal interaction](#crystal-interaction)
    * [Crystal types](#crystal-types)
    * [NPCs crystal patch](#npcs-crystal-patch)
  * [Crystal network](#crystal-network)
    * [Crystal network nexus gate](#crystal-network-nexus-gate)
  * [Tower system](#tower-system)
    * [Power relay](#power-relay)
    * [Anti fog tower](#anti-fog-tower)
  * [Knowledge system](#knowledge-system)
    * [Knowledge aquisition](#knowledge-aquisition)
    * [Level progession](#level-progession)
    * [Levels use](#levels-use)
      * [Skill unlock](#skill-unlock)
      * [Base stat unlock](#base-stat-unlock)
  * [Skill/Perk tree](#skillperk-tree)
    * [Social skill unlocks](#social-skill-unlocks)
    * [Farming/Foraging unlocks](#farmingforaging-unlocks)
    * [Spell unlock system](#spell-unlock-system)
    * [Slow unlocks](#slow-unlocks)
  * [Elemental Essence System](#elemental-essence-system)
  * [Spell progession system](#spell-progession-system)
    * [Spell types](#spell-types)
    * [Spell Crafting](#spell-crafting)
      * [Ingredients](#ingredients)
        * [Elemental Essence](#elemental-essence)
        * [Refined Crystals](#refined-crystals)
      * [Requirements](#requirements)
      * [Learning](#learning)
  * [Armor System](#armor-system)
    * [Armor Construction Ingredients](#armor-construction-ingredients)
  * [Portal](#portal)
    * [Portal Dyanmics](#portal-dyanmics)
    * [Portal Advancement](#portal-advancement)
  * [Export/import mechanism vis portal](#exportimport-mechanism-vis-portal)
  * [Export/import upgrade treeo](#exportimport-upgrade-treeo)
  * [Town progression](#town-progression)
    * [Building gameplay](#building-gameplay)
    * [Unlockable buildings](#unlockable-buildings)
      * [General merchant shop](#general-merchant-shop)
      * [Portal comms building](#portal-comms-building)
      * [Antifog technologies](#antifog-technologies)
      * [Common barracks](#common-barracks)
    * [Tech progression](#tech-progression)
    * [Growing town from nothing to something](#growing-town-from-nothing-to-something)
  * [Build Production chain](#build-production-chain)
    * [Crystals as power sources](#crystals-as-power-sources)
    * [Production buildings](#production-buildings)
    * [Automation alternatives](#automation-alternatives)
    * [Customisation/Vanity](#customisationvanity)
    * [Monster crystal farm interaction](#monster-crystal-farm-interaction)
  * [Map features](#map-features)
    * [Geography](#geography)
      * [Predominant geometry](#predominant-geometry)
    * [Constraints](#constraints)
      * [Crystal network constraint](#crystal-network-constraint)
      * [Cliffs](#cliffs)
      * [Fog](#fog)
        * [Fog Clouds](#fog-clouds)
        * [Cloud difficulty scaling](#cloud-difficulty-scaling)
        * [Variation](#variation)
          * [Variation routers](#variation-routers)
          * [Variation sources](#variation-sources)
        * [Traversal](#traversal)
        * [Tower](#tower)
    * [Mountain tunnel](#mountain-tunnel)
    * [Crystal Wall](#crystal-wall)
      * [Core Design](#core-design)
      * [The Crystal Nexus](#the-crystal-nexus)
      * [Monster Spawning & Attacks](#monster-spawning--attacks)
      * [Defensive Tower Mechanics (Introduction)](#defensive-tower-mechanics-introduction)
      * [Progression](#progression)
    * [Impassable river](#impassable-river)
      * [Improved River Obstacle Design](#improved-river-obstacle-design)
      * [1. Main design](#1-main-design)
      * [2. Boat](#2-boat)
      * [3. Strategic Crossing Points](#3-strategic-crossing-points)
      * [4. Integration with Town Safety](#4-integration-with-town-safety)
      * [5. Tower defense](#5-tower-defense)
      * [6. Optional boss](#6-optional-boss)
    * [Cloud Islands](#cloud-islands)
    * [Giant crystal tree](#giant-crystal-tree)
    * [Magic lakes](#magic-lakes)
  * [Story lines](#story-lines)
    * [Gamer](#gamer)
  * [What does the player build and sell](#what-does-the-player-build-and-sell)
  * [Day night](#day-night)
  * [NPC Advancement](#npc-advancement)
  * [Map Variety](#map-variety)
  * [NPC Progression System](#npc-progression-system)
* [Secrets](#secrets)
* [Factions](#factions)
* [Sliding window implementation](#sliding-window-implementation)

<!-- mtoc-end -->

## World building

Set in an alternate universe where Earth has magic because it leaks in from other dimensions through portals.
Elements from these other realms seep into Earth, causing magical manifestations and phenomena.
Manifestations from these dimensions appear as

- Magical zone anomolies where magic creatures generate and generally attempt to cause havoc on society
- Allows the use of magic by humans who have been randomly been altered by the forces of the alternate dimensions
- Earth has become dependent on magic gems, partly because they are required to continously combat the various
  incursions of entities from the alternate dimensions
- Whilst gems can be sourced from earth, as the demand grows entreprenurs have been dwelving into these alteranate dimensions
  to source gems for consumption on earth

- The player is one such entreprenur.

- A monopoloy coporation has evolved which now controls most of the infrastructure connecting earth to the other dimensions
  They are one of the main touch points with the player.

## Backstory

You begin your journey in the overworld, living with your parents in your hometown.
After studying crystal growing and saving up enough gems, you finally have the means to transport yourself—and all your belongings—to the other dimension
where you hope to make it big as a gem exporter.

However, during your journey through the portal, an irregularity occurs, and you lose most of your belongings...


## Core game loops

### Labour value theory

#### Resource gathering

- Gathering resources
- Loot variety

#### Crystal Farming & Production

- Plant crystal shards and grow crystals over time
- Harvest magic essence or break crystals for raw gems
- Build production chains powered by crystal energy
- Balance crystal growth (power/resources) vs monster spawning (danger)

### Spatial progress, exploration and expansion

- Crystal networks are arranged in cells in the map
- Crystal networks produce fog clouds which the player must destroy
- Crystal networks will restore clouds which the player has destroyed
- Thus as the player ventures out and explore, they will get boxed
  in, which creates a sense danger and risk
- When the player has destroyed the source of the fog, the entire
  network is unlocked, allowing full access to the resources
- Some crystal network central nexus can be tapped to power player crystal power network

- The town contains a power source, we can build out a network 
- Mana is a valuable scarce resources whilst the network is is always powered
- So the cells are destroying clouds which then drops some resources which the player
  can harvest, hwoever dust/shard ratio control how quickly player can acquire shards
  to grow crystals
- Towers can either destory cloud (high power cost), or simple push clouds back (lower power cost)
- However there are angry clouds which detect towers close the center which will fight back
  and attackk player (they do this by thrusting clouds at the player!)

- also in the cell are actual crystals which the player can harvest if they can get close enough
 - however these crystals are responsible for growing crystla catalyst which the player needs 
   to grow crystals
 - later we can also build crstyal catalyst harvested which will automatically harvest and store
   catlayst for the player to then harvest
- 
- can the player upgrade towers ? yes which will make them ore efficient

- we also need a slow level progress system built into the world like dungeons with levels
  because dungeon levels represent macro progress over long horizons
- we need a map feature which the player can continously attack or devote resources
  to upgrade in order to unlock ?
- for example in stardewvalley there was a dungeon which the player can progress through levels
  it gave a continued sense of progression in the game

- key exploration spell is the fog respulsor which the player can place down anywhere and good 
  for exploring the map to find different network variants to move towards. The spell 
  however can overwhelmend by agressive clouds

- remember there is also the exporter

- aslo end game is after player stars generating enough power, you get monsters spawn at the map outskirts
   which will come for the town, so then it becomes a massive  tower defense game, where you have
   to build towers are specific locations. to beat preogressively poerful waves though requir
   red gem tech, etc
- fog attack vs monster attack scaled differently though


#### Survival

- Manage hunger by eating 2-3 times daily
- Manage mana through crystal-crafted potions
- Navigate day/night cycle (dark crystals spawn stronger enemies at night)
- Sleep mechanic with penalties/bonuses based on hunger and rest duration

### Progression systems

#### **Combat & Defense**

- Fight monsters spawned by crystal patches and power sources
- Build and upgrade defensive towers to protect town and crystal farms
- Defend against periodic monster attacks from crystal nexus structures
- Clear natural crystal growths to reduce monster threat

#### **Town Building & NPC Progression**

- Build and upgrade buildings to attract NPCs
- Unlock new capabilities through town advancement
- Manage town resources, renown, and supply lines

#### *
*Export & Progression**

- Export gems and crafted items through the portal terminal
- Earn corporation benefits and increase export capacity
- Use profits to upgrade tech trees (combat spells, utility, buildings, portal)
- Unlock new crystal tiers and production capabilities

## Initial beats

- Player arrives in world
- Need to introduce main hooks quickly
- Resource gathering
  - Simple to figure out, player just clicks on items
- Fog destruction, tower, monsters
  - Close to the player are some resources protected by the fog
    player must build a tower to eleminate the fog
  - Serves as an introduction to fog exploration mechanics
- Farming
  - Npc lets player know they have started a small gem farm
    and invites the player to also share in using it
  - Later the player will have to expand the farm on their
    own
- Building machines
  - Player needs to discover this by using the menu system

## Gameloop

## Progression trees

- Combat spell upgrades
- Utility spell upgrades
- Town progress
- Exporter upgrade progression
- Crystal production building tech tree

## Health/Mana system

### Health system

### Mana system

- We do have a mana system, and need pots to replenish the mana
- Also mana recovers very slowly overtime by itself
- Pots are made from crystals
- Eventually mana requirements become quite large so need larger mana pots
- Crystal heirarchy which equates to different level of mana pots

## Food System

- The player needs to eat at least two/three times a day to keep their food levels high
- If they exceed their hunger limits they get penalised (movement speed and increased mana consumption, progressing until basically unplayable)

- Food is a very scarce asset in sanctuary. This is because human edible food does not grow in this dimension
- Food arrives via the exporter every morning. Enough at first for just one days worth of
- Food is expensive to import because it is a human organic material so costs alot of gems to stabilise

- The food constraint makes it very clear how dependent the town is on the exporter and so creates another goal
  for the player to upgrade

- Also the player will essentially not be able to reach the edges of the map until they can become non reliant
  on the importer for food. I.e when they are able to but food from the towns people. Though even then the
  amount of food available for sale ona daily basis will be limited

- However later in the game they will have the food amounts and teleporter network in order to survive mostly comfortably
  at night

- Very late in the game an npc will offer the player some way to establish a farm (like very end game).
  So yes in the late game we will turn this into a farming game

## Initial items

### Raw gem

- Most basic ingredient
- Dropped from:
  - Destroying crystals
  - Destroying trees (drops less then crystals)
  - Monsters also sometimes drop this

### GemWood

- Trees will grow as normal
- They will show some effects of the crystal corruption

### GemPlanks

- Refined from gem wood
- Used to make buildings

### WardSteel

- WardSteel is the derived version of metal from earth in this dimension, it is infused with
  magic. WardSteel is required for building in order to protect
- Occurs in raw form next to crystals which emenate power
- Usually guarded by monsters as they are attracted and are spawned by the power crystals
- Normal rocks already on the map may transform into it ?
- WardSteel tech level influenced by the powercrystal type.

### Magic essence

- Magic essence can be:
- Harvested from power crytals
- Monsters drop this (initial source)

### Condensed gem sheet

- These are sheets of gem infused used for various constructio
- Made from magic essence

## Crystals

### Wild crystal lifecyle

- Crystal catalyst spreads
- The fractal nature of network extends are hexagonal, i.e the from top down they conform to a hexagonal grid
- Crystal networks main goal is to continuously increase it's power production
- Crystal networks will
- Crystal catalyst will spawn crystal (which the player can harvest)
- Crystal catalyst and crystals absorb the energy of the sun at day and expend this to grow their network
- What role does crystal filament play in the life cycle ?
  It will be used as a binding/threading agent
  Analogies of bushes to, basically let's just use the bush model and make it crystal structure
  with some crystals poking out
  Crystal network uses bushes to protect the catalyst from damage i.e stepping on them once will damage the player
  Or earlier on they will simple impede progress
  So then we have another natural barrier towards progress on the map

consiousness which is still an undefined quantity
exists in phases

- that which binds to complex structure to express itself and expaned
- that which exists in raw farm and expresses itself through use
- the third form is ant-consiouss or the form which seeks self destruction
  but can only accomplish this goal by
- regions of the multiverse are dominated by these three phases

### Crystal growing mechanism

#### Overview

- Analogies
  - Crystal shard analogous to seeds
  - Crystal catalyst analogous to water

#### Spraying mechanic

- Player chooses the spraying spell
- Indicator of effected area ( a circular area )
- Crystal lacking catalyst will appear dull w/out color
- As they get sprayed their luminosity changes, and once fully sprayed they
  make a satisfying sound and some small particle effect animation
- Thus the player can upgrade the spell to spray a progressively larger area
- Spraying continously consumes crystal catalyst, however catalyst is relatively abundant

- Power crystals
  - Crystal power shards are used to grow power crystals
  - However power shards are of limited quantity and must be obtained by destroying wild power crystals

#### Crystal cores

- Crystal cores are obtained by extracting them from wild crystal nexus

#### Core projector

- Core projectors use crystal cores to project onto the ground crystal beds
  which can be used to grow crystal by planting crystal shards

- Core projectors must be built and will automatically consume crystal cores
  the player has accumulated, however the player probably should be able
  to change the layout configuration

- Different levels of core projects will exist with increased levels of beds
  generated

- Core projects should be upgradeable with modifires to
  - increase yield
  - increase growing speed
  - etc etc

- Each slot which can grow a crystal requires a crystal core

- Initally the player is introduced to crystal farming via the merchant npc who's has a core
  machine deployed which they intend to use to make potions

- Player can place core projectors mostly anywhere I think.
  Though there is the issue of player placing a projector where an npc building will eventually go

#### Growth feedback

- Continuous feedback on progress
  - Crystals grow over time, different texture to show progress

#### Variety

- Able to customise layout/variety/schedule
  - Player will be able to grow crystals of increasing rarity as game progresses
  - Some mechanism involved in geometry/arrangement of crystals that unlock certain crystal growth

#### Value

- Clear value and reward mechanism
  - Breaking/harvesting crystals is easy
  - This is what the overworld requires, can sell these crystals for money
  - Certain crystals will be used as magical ammo

### Natural Crystal strucures

- Crystals in nature appear in tiers:

#### Power crystals

- These crystals can be tapped to generate power, and connected to the player power network.
- Power crystals are the source of crystal networks
- Crystal networks expand naturally and lower tier crystals which can be harvested by the player
- Monsters spawn in higher numbers around power crystals and defend the power crystals
- They will be generated strategically in the map to incentivise the player to explore the map
- They provide a natural progression system as the player must venture out further and further to acqurire more power
- Power crystals comes in tiers (Blue, Green, Red, Gold)
- Each crystal can also level up with enough maintenance/time

#### Raw crystals

- Raw crystals are the networks way of storing crystal powe generated from, trees bushes, and the network itself
- These crystals are non power generating but can be harvested by the player for raw gems
- These are the types of crystals which will be predominantly farmed by the player in their crystal farm

#### Dark Crystals

- These crystals are responsible for spawning powerful enemies at night time to constrain the player

#### Crystal catalyst

- The crystal networks also produce a crystal catalyst which can be harvested by the player.
- The crystal catalyst will appear on the map as a liquid like resource which the player can harvest.
- The harvesting mechanic will involve the player pointing their spell at the area and the catalyst will be syhponed
  into their inventory.

- Crystal catalyst is required to feed the player grown crystals to ensure they grow for that day

- Probably represent the crsytal catalyst growth as connected hexagonal area, too cpu intensive to model using polygons
- We will need to have pixel art representations of each possible arrangement of the hexagonal catalyst
- We either remove hexagons or maybe shrink them as correlated with the amount of health they have

### Crystal power

- Magic essence/ crystal power can be automatically harvested from cyrstals
- To convey the power need to build relays at periodic distances
- Therefore one can build harvest far away resources if they have a good relay network
- Can collect magic essence in large storage vats (nice animation to show the fluid type nature of maggic essence)
- Crystals generate power which powers your building
- Only certain spots in the game will allow you to grow crystals which
  provide continous power
- Otherwise just generic crystals will grow to a point then be static

### Crystal interaction

- Break the crystals if you want shards and gems
- Harvest crystals if you want (essence)

### Crystal types

- [Blue, Green, Red, Gold] Normal crystal levels
- Teleporter enabling crystal [takes time to grow hard to get shards]
- Black crystal,grows from death of humans, tech factions wants to buold cpus, creating consious machinws

### NPCs crystal patch

- Some npcs will mine their own crystal patch to produce stuff for you
- Early in the game you will be tasks with protecting their crystal patch for them

## Crystal network

- Crystals form networks

- Crystal network form natural barriers which compartmentalise the map so that the player has an immediate
  Crystal nexus at the intersection of network tendrils must be destroyed in order to proceed accross the map

- The nexus will spawn large amounts of enemies and it will take some effort to defeat them
  -> either by getting enough instrastructre to build towers
  -> or by levelling up enough to get spells

- Contained within the network cells are resources that are required for progression
  - Essence fountains

- networks create walls which the player must defeat

### Crystal network nexus gate

- These structure act as hard bariers between larger map sections
- The gate will spawn priests who will restore crystal networks
- Priests will ignore some hexagons at the start so player is not stressed out
- Number of priests spawn will depend on number of nexus destroyed
- Player will either need to position themselves or build a tower to defend it

- We need to also add some strategy to how player acquires crystal networks
- Player should actually go close to the gate because then they can catch the mobs
  at the start

## Tower system

### Power relay

- To route power around relays must be built to expand the reach of the power network

### Anti fog tower

- Uses power to eliminate fog clouds
- Has a relatively short range so the player has to move it to progess through the fog cloud

## Knowledge system


### Knowledge aquisition

- Actions in the game give experience
    -   Harvesting items
    -   Killing enemies
    -   Conversations
    -   Farming
    -   Killing clouds

### Level progession

- Getting enough knowledge will advance level

### Levels use


#### Skill unlock

- Use level points + (potentiall items to learn new skills)

- Reduce knowledge gain when player has lots of unused skill points

#### Base stat unlock

- Alternatiely can just boost mana pool + regeneration rate infinitely ?
  however with exponentially decreasing effectiveness, 


## Skill/Perk tree

### Social skill unlocks


### Farming/Foraging unlocks


### Spell unlock system
 
### Slow unlocks

- Slow field
    - Requires one level point
    - Requires x10 monster drops


## Elemental Essence System

Whilst gems represent power progression in the game, elemental essense represent cardiality.

**Essence Types & Sources:**

- **Fire:** Magma Fountains/Lava Geysers (volcanic regions)
- **Frost:** Glacial Fountains/Cryo Geysers (frozen tundra)
- **Storm:** Thunder Fountains/Lightning Geysers (mountain peaks)
- **Temporal:** Chronos Fountains/Time Geysers (ancient ruins - rare)
- **Gravity:** Void Fountains/Singularity Geysers (spatial anomalies - very rare)
- **Arcane:** Prismatic Fountains/Arcane Geysers (ley line convergences - rare)

**Extraction:**
 
 - See Fog variant system

## Spell progession system

### Spell types

- Fireball spell
- Firewall spell

- Storm gust
- Times frost explosion

- Gravity blackhole

### Spell Crafting

#### Ingredients

##### Elemental Essence

- Corresponds to fire/water/etc essences that can be harvested from map locations

##### Refined Crystals

- Refined crystals from crystal farming

#### Requirements

- Elemental Essence (determines spell type)
- Power Crystals (determines spell power)
- Optional Catalysts (adds special effects)

**Examples:**

- Fire Ball: 20 Fire Essence + 5 Crystals
- Fire Wall: 40 Fire Essence + 10 Crystals + 3 Force Shards
- Gravity Black Hole: 50 Gravity Essence + 15 Crystals + 5 Void Fragments

**Catalysts:**

- Force Shard (knockback) - 20% drop from guardians
- Prismatic Shard (multi-targeting) - 10% drop from convergence elites
- Void Fragment (gravitational wells) - 50% drop from bosses

#### Learning

- Crafted spells create consumable gems that permanently teach the spell when used
- Spells with slight variants however will override each other

## Armor System

- Armors are a consumable quasi physical/magic item which provide protection against death
- Armors must be applied to the player to have an effect. Applying armors takes seconds and is interruptible
- Once armors are applied they cannot be regenerated, i.e a new armor must be applied

### Armor Construction Ingredients

- WardSteel
- Crystal filament (of different levels)
- Crystal gems of some variety
- [Optionally a modifier] catalyst

## Portal

### Portal Dyanmics

- Portal by default allow limited transfer of entities between them except gems and other small objects
- However researchers have found ways to use gems to allow transport of other items from earth to dimensions sides
- It is also possible to strengthen the portal from the dimensions side so that it is easier to move items to/from portal

### Portal Advancement

- The portal is what provides the players information table with statistic
- The map provides information but it's range needs to be upgraded with the portal
- It must be provided with enough power/items to create permanent upgrades

## Export/import mechanism vis portal

- The export terminal is used to control the export mechanism
- The terminal has a chest which the player inputs items which are selected for exporting
- The player executes the exporting via a switch

- Why add the charge time for the exporting ?

## Export/import upgrade treeo

- The export/import machine has an upgrade tree as well

## Town progression

- how to represent the town building ui to the player ?

### Building gameplay

1. Player selects buildling from menu
2. Player places it on the map
3. A further requirement is that relevant npcs are available for cut scenes

### Unlockable buildings

#### General merchant shop

- Contains common items necessary for the player

#### Portal comms building

- This will start of as a simple open station which will reveal to the
  player the nature of the world map expansions system
- should be pretty easily buildable as it will introduce a major game mechanic/goal

#### Antifog technologies

- Sells antifog buildings for gold

- Buildings which when placed provides fog repellent for at least x number of hours in a raidus
  used 

- Building which can be placed and consumes clouds to provide crystal power

#### Common barracks

- Initial barracks which everyone will sleep in initially before building houses for everyone

### Tech progression

- NPC Shop + Gem field
  - Have to wait until npc gem fields grows to start buying potions

### Growing town from nothing to something

- Building and upgrading buildings
- Building certain buildings unlocks more things
- Player can decorate the town

- Town renown system
  - Player must upgrade the town to make it more attractive to potential

## Build Production chain

### Crystals as power sources

- Able to source energies from the crystals and accumulate them in large tanks
- Then enabled production chain to produce pots etc from the accumulated manag essences

### Production buildings

- Production building plans are placed and then built
- They have a menu which player can interact with
- They have a animations for when working

### Automation alternatives

- Instead of belts we use magic to move
- Central logisitcs tower which enables teleportation from certain buildings to other buildings
- However we need some kind of animation to show import/export of items

### Customisation/Vanity

- Decorate the town with little items to spruce up the town

### Monster crystal farm interaction

- Monsters will seek out your crystal farm and attempt to suck on your crystals to grow bigger
- Can build towers to protect your crystals
- However towers will consume your crystal resources

## Map features

### Geography

#### Predominant geometry

- The map will be open world, but the primary direction of progression is toward the north. The southern edge of the map is blocked, and the sides are bordered by natural obstacles such as oceans and mountains.
- There are a number of benefits:
  - This simplifies the nagivation for the player and introduces a natural progression in terms of exploration
  - It is also easy procedurally generate a world with a defined predominant direction
  - Also it simpler to design natural progression barriers as we can place them at some distance from the start point further out north

### Constraints

Constraining the player movement is required as the player needs some kind of obstacle to defeat

- Enemy difficult scales with distance from town center
- We introduce some fissures or other natural barriers which the player must overcome to continue progressing
- Player can't spend all time in the wild because they will run out food and food is scarce
- Can also restrict crystal production infrastructure to also limit exploration capability

#### Crystal network constraint

see [Crystal network](#crystal-network)

#### Cliffs

- Your usual basic cliffs should be procedurally generated to give variety to the map

#### Fog

##### Fog Clouds

- Some crystal networks produce a strucutre which emits fogClouds
- The fog is used as a main constraint to player exploration in the game
- Acts as map barrier which must be overcome to get access to the resources of the crystal networks

- Fog Cloud have a radius in which the player is damaged
- They slowly drift within the area controlled by the crysttal network cell
- FogClouds can be destroyed
  - by player spells
  - anti fog tower
- The crystal network will periodically refresh fogClouds the player has destroyed

- FogCloud damage, intensity and frequency increases during the night

- Need some other crystal structures which impose benefits to the fogClouds and make them basically
  harder to destroy, the the player will need to use their magic spells to remove these other structures

- Continoulsy eliminating fogClouds will slowly raise the agression level of the crystal network

##### Cloud difficulty scaling

- Need to also scale the difficulty of the clouds as well
- Higher levels clouds will seek the player out
  - Will overload certain cloud structures
- Clouds which correspond to gem level which will have higher damage and much tougher

- Will have a game mechanic emualting tornadoes/gust, i.e a large mass of clouds is emitted
  at the player from some source, so requires some specific stratergies to overcome


##### Variation

- There is some source of variation on the map which spreads through natural means
  and slowly converts particular fogs to drop different items/behave differently,
  the player is able to eventually control these sources to graduate the behaviour
  - The drops are required to advance up the skill tree
  - So some skills are gates behind the player being able to route successfully
  - In face

-> how do variant routers effect flow direction ?

-> GAMBLING
  -> randomly modify some source on the map
    -> adds a source, or randomly introduces a negative modifier


###### Variation routers

- Variation routers probably exist at the intersection of hexagons
- Variation routers only affect networks adajcent to them

- Not all hexagon intersection have routers, or some are yet to be  upgrades/discovered

###### Variation sources

- Varaiation sources have starting power which degrades
- Variaations can combine in different ways to produce different effects


##### Traversal

- Can destory the fog
- However it comes back
- Should have a method to prevent it coming back
    - Anti fog tower which will destroy fogs that come close
      (+ prevents new spawns)

- A spell which will prevent clouds from respawing in an area
  and slowly pushes clouds back

- So then the player pushes abit, finds a area they want to farm
  deploys the spell, farms then tries to get back

- A building which is very simillar to the spell bit lasts alot
  longer, and requires a power cell (which is produced from using
  a factory which uses crystal power)


- A players amour which grants passive cloud resist
- Players amour which 


##### Tower

- See [Anti fog tower](#Anti-fog-tower)

### Mountain tunnel

- Player encounters a large mountain blocking progress
- Player will have to build a mini town / excavation camp to excavate the mountain
- The excavation takes far too long for the player to do it, so they can hire people from the town
  to do it, however have to pay them, and supply food for them
- So have to manage food supply transport somehow to the mining site
- Tunner is dark, so player will have to be somewhat involved and build lighting through the tunnel
- Monsters also will periodically attack so need to hire protection
- There should be some benefit also for the player to be in the tunnel, i.e diggin will uncover important loot potentially
- Tunnel will expose branches

### Crystal Wall

#### Core Design

**Obstacle**: A massive impassable wall of living crystal that blocks progression to the next area.

#### The Crystal Nexus

- The wall is generated and continuously repaired by a **crystal nexus structure** on the opposite side
- The nexus exposes a **narrow opening** - the only weak point where the player can attack
- Destroying the nexus makes the wall destructible, exposing the next level of the map and higher-tier crystals

#### Monster Spawning & Attacks

- The nexus spawns monsters that periodically attack the town I
- Attack frequency scales with the number of power-generating crystal patches the player has cultivated
- This creates strategic tension: more crystals = more power but more danger
- Rewards players who balance offense (attacking the nexus) with defense (protecting the town)

#### Defensive Tower Mechanics (Introduction)

- To survive monster attacks and protect the narrow opening assault, players must build **defensive towers**
- Towers are powered by magic crystals the player has cultivated and grown
- This is the first major introduction to tower defense gameplay
- Players learn to position towers strategically to defend against waves while assaulting the nexus

#### Progression

- Once the nexus is destroyed:
  - The crystal wall becomes destructible
  - The next map level is exposed
  - Higher-tier crystals become available for harvesting
  - New challenges and obstacles emerge

- Next level mechanics (ok the islands)
- To progress through the islands the player must activate some kind of power source on the island which will enable the island to form a bridge to the next island when it is close by
- There is again some late level boss or obstacle which the player has to overcome to progress to the next level

### Impassable river

#### Improved River Obstacle Design

**Core Concept**: The river is a dynamic obstacle that introduces crystal mechanics, strategic decision-making, and foreshadows later defensive gameplay.

#### 1. Main design

- The river is too large to cross therefore the player must build a bridge in order to cross
- To cross the river the player must build three bridges, spanning two island waypoints
- Each island waypoint contains an milestone enemy fight as well as some valuable treasure

#### 2. Boat

- The player is able to build boat to travel along the river
- However crossing the river in the boat is not possible because the further away areas have magic tides which turn the player away
- The last island in the chain has the switch to turn of the river tides

#### 3. Strategic Crossing Points

- There will be several location where the player may build the bridge as there will be 2 - 3 island chains which the player can build a bridge to cross at

#### 4. Integration with Town Safety

- The river initially acts as a **natural barrier** protecting the town from the crystal wall's monsters
- Once bridged, it becomes a **vulnerability** - monsters can use it to attack
- This creates tension: crossing the river advances progress but increases danger
- Foreshadows the concept that the town is never truly safe

#### 5. Tower defense

- The bridge eventually becomes a central tower defense type mini game
- The bridge can be upgraded to support defensive towers for repelling attacking enemies
- The enemy will attack the bridge, attempt to destroy the towers, and gain control of the bridge
- When they gain control of the bridge they will build their own tower there and fortify it

#### 6. Optional boss

- There is a sea monster in the river which the player may optionally fight.
- However fighting the monster requires great peperation, and to solve a puzzle in order to lure the monster to the correct island to fight it

### Cloud Islands

- These are islands which float around the main map, so the player must use a specific spell to access these islands
  - Essentialy there are another scene which the player will load into
  - They are an interesting way for the player to move around the map
  - Clouds passing overhead may impart some specific effects to the map below
    - They may power up crystals
    - Thy may increase monster spawn rates and power ?
  - Later the player may be able to harness a cloud an place it above their farm

### Giant crystal tree

- Giant crystal tree with special monster types around it

### Magic lakes

## Story lines

### Gamer

Npc forced to come here who just wants to either go back or build a game pc so they can play computer games

## What does the player build and sell

- Magic wands
  - from cutting down trees

## Day night

- Dark crystals activate at night which spawn stronger enemies which will attack the player

- Nighttime enforces a reset and checkpoint, but a less intrusive
  notification system for events is needed.

- Sleep always ends at 6AM; less than 6 hours causes penalties,
  sleeping with a full stomach gives benefits, and being famished
  prevents recovery and exp gain

- The issue of the night is problematic
  -> it does force a reset and a mandatory checkpoint the user must go through
  -> however enforcing it is also annoying -> we need some other kind of notification system to signal to player of optional but beneficial events
  -> we don't allow user to control how much they sleep if player goes to sleep they always will wake up
  at the same time (6AM) if player sleep less than 6 hours they are penalised if player sleep with full stomach they get benefit if player is too hungry they get no experience and health doesn't recover

## NPC Advancement

how to npc start to advance?
-> they build a home
-> they build a business
-> when npcs get rich they provide benefits
-> they may

-> secure some supply lines for basics
-> secure some supply lines for advanced
-> advanced supply lines
-> entertainment
-> parties and celebrations are hosted for every great milestone the town goes through

npc start building out from the the central town teleportation square

## Map Variety

The fog won't be completely dark, it will be somewhat transparent as the player will have no idea where to go
In later levels the fog density can increase to really make it annoying to get through

Think about map variety:

- Lakes
- Rivers
- Trees
- Wand production trees
- Chests ? Or loot or other things
- Mining nodes
- Resources collection nodes

## NPC Progression System

And NPC start to advance

(clear sense of progress, but there is no time limit )
progression

-> keep the cooking pot filled with food for two days
-> npcs will be inclined to start gather materials
-> if cooking pot goes empty then they stop accumulating materials
-> npcs will actually accumulate materials by themselves as long as player
does minimum amount required

-> Reaching a self sustaining food supply eventually requires
-> renewable magic supply
-> some people to go hunting every day

maybe a progression of goals

-> secure food supply
-> secure some supply lines for basics

Resource Management
Resources usage
Building towers will require certain resources

Building up the town is one option, where the town starts of small, and exploration progress unlocks things
Maybe a fight with many of your allies against some monsters that come through ?

# Secrets

- These other dimensions feed off from the consciousness of humans
- What humans take for granted is missing in these other dimensions
- Certain human activities overall decrease conscioussness and this is extracted from earth dimensions

# Factions

- Different factions have developed on earth:
  - Expansionists who advocate for massively expanding humanity into alternative dimensions and importing resources
    back to earth for consumption
  - Death cults who believe alternative dimensions are the lure of the devil. They want to destroy the links to other dimensions
    and are incredibly violent
    - There was an unfortuante incident where unexpectedly a link destroyed trapping all expeditioners on the other side
      who are presumed now to be dead
  - The expansionists and death cults are at war with each other
  - Research organisations who seek to understand the other dimensions further before deciding on further actions. They have
    strict dogmatic beliefs about how the universe functions and other dimensions function. They believe researching other dimensions
    will help to understand the universe more and develop science to a point enough to destroy magic. Scientific progress has been
    slowed down in their view due to magic

- Unknownst to humanity there are also other portals from the other dimensions to even more dimensions. Finding this
  out in game is a huge revelation.

- Dimensional civilisations who migrate from one source of spirit to others and seek to harvest the spirit for their own use
  to live longer and to make these civilisations subservient to themselves.

- Also a Tom Bambodil type character who is wise and has travelled between dimensions using his own devices and seeks to
  maintain order between dimensions, whose origins and masters are mysterious. One of the main 'guides' in the story line.

# Sliding window implementation

Entities are only simulated in certain world chunks, not the
entire world. When entities are removed from the registry, their
data is saved in a standard format for later loading. Use entt's
archive functions to persist and restore entities.

The world uses a grid for tiles and generation, but entities do
not have to fit this grid. Collision can be checked by comparing
all entities, or by using spatial partitioning for better
performance. A grid is also needed for pathfinding, with a
minimum size of 16x16 pixels.

Some chunks and entities are always simulated. There is a global
registry for these always-simulated entities, and their data is
passed to local entities when they come into view. If a global
entity's chunk is active, update its components in the current
registry.
