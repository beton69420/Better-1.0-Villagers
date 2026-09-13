# Better-1.0-Villagers
Better 1.0 Villagers improves Minecraft 1.0 villagers while keeping the classic 2011 feel. Villagers can use doors, avoid water, seek shelter, socialize, avoid hazards, gain more visual variety, and farms are protected from trampling. SPC/WorldEdit compatible.

# Better 1.0 Villagers

Better 1.0 Villagers is a mod for Minecraft Java Edition 1.0.0 that improves villagers while keeping the classic 2011 Minecraft feel.

The goal is to make villagers smarter, more useful, and more alive without turning them into modern Minecraft villagers.

Current and planned improvements include better door behavior, water avoidance, sheltering at night and during rain, simple social behavior, danger awareness, more classic villager varieties, and farmland protection.

The mod is designed to stay lightweight, old-school, and compatible with legacy tools such as Single Player Commands and WorldEdit.

> Think of it as: **“What if Mojang had polished Minecraft 1.0 villagers a little more?”**
>
> ## Current Status

Better 1.0 Villagers v1.0 is currently in development.

### Phase 1 — Complete ✅

- Villagers can open wooden doors
- Villagers close doors after walking through
- Improved doorway pathfinding
- Villagers avoid getting stuck in water
- SPC compatibility confirmed
- WorldEdit compatibility confirmed

### Phase 2 — Complete ✅

Phase 2 focuses on making villagers behave more naturally around their village and properly use shelter.

- Villagers stay within a soft village perimeter instead of wandering far into forests
- Villagers naturally disperse around the village during the day
- Villagers avoid forming huge crowds in one location
- Villagers seek shelter inside houses at night
- Villagers seek shelter during rain
- Villagers distribute themselves across multiple houses instead of all choosing one house
- Houses use lightweight occupancy and reservation logic
- Villagers remain sheltered instead of immediately wandering back outside
- Villagers gradually leave houses in the morning
- Unreachable shelter targets are abandoned so villagers can choose another house
- Phase 1 door and water behavior remains compatible
- SPC compatibility confirmed
- WorldEdit compatibility confirmed

#### Phase 2.1 — Advanced Village & Building AI 🔧

Phase 2.1 is a major polish and intelligence update focused on villager traffic, doors, large buildings, multi-room navigation, and more reliable shelter behavior.

Because the scope became much larger during testing, Phase 2.1 is being developed in three sub-phases.

---

### Phase 2.1A — Traffic & Door Reliability ✅

Phase 2.1A focuses on making villagers move through entrances more naturally and reliably.

Implemented:

- Improved villager entrance queueing
- Villagers wait more respectfully instead of heavily cramming into doors
- Better single-door traffic flow
- Improved double-door traffic
- Double doors behave as two independent traffic lanes
- One double-door leaf can remain open while the other stays closed
- Villagers only open the door leaf they actually need
- Player-opened door leaves remain player-controlled
- Villager-managed door leaves are tracked separately
- Villager-managed door ownership can recover after world reloads
- Reduced unnecessary repeated door opening and closing
- Major reduction in door sound spam
- Improved handling of mirrored double-door states
- Villagers detect doors that are physically unreachable
- Doors blocked by fences, walls, solid blocks, or inaccessible terrain are rejected
- Villagers can choose an alternative reachable entrance
- Temporary crowding is not mistaken for permanent structural blockage
- Short-lived unreachable-door information can expire if the player changes the building
- Villager-vs-villager movement deadlocks are detected
- One villager can briefly yield so both villagers can continue moving
- Improved narrow-path and head-on traffic behavior
- Better angled approaches to entrances
- Door-closing failsafes for mod-managed doors
- Existing Phase 1 and Phase 2 behavior remains compatible
- SPC compatibility preserved
- WorldEdit compatibility preserved

Live testing has confirmed much more natural shelter queues, including large groups of villagers entering houses without the heavy pushing and cramming seen previously.

A small daytime door-closing polish is currently being finalized so the last villager closes a managed door shortly after safely clearing the entrance.

---

### Phase 2.1B — Building & Interior Intelligence

Phase 2.1B will focus on teaching villagers how to navigate and use larger and more complicated buildings.

Planned features:

- Better support for multi-room buildings
- Villagers understand that internal doors are not necessarily exterior exits
- Persistent building-exit behavior during clear daytime
- Villagers sheltered deep inside a building will continue navigating until they actually reach outdoors
- Normal daytime wandering will not interrupt building egress
- Better indoor population distribution
- Villagers spread around large interiors instead of crowding into one room or corner
- Doorways, hallways, and staircases are avoided as permanent idle locations
- Support for multi-story buildings
- Support for basements and underground rooms
- Detection of reachable interior floors
- Villagers can travel between floors using valid paths
- Population is distributed between floors based on usable space and crowding
- Small populations will not be unnecessarily spread across every floor
- Additional floors become populated only when the building population is large enough to benefit from them
- Large populations can distribute across multiple floors and basements
- Lightweight floor-capacity and reservation logic
- Better staircase traffic
- Villagers gradually leave upper floors and basements when shelter is no longer needed
- Staggered morning exits to reduce traffic jams

The system will be designed generically for vanilla structures and player-built houses rather than being hardcoded for any specific test world or mansion.

---

### Phase 2.1C — Regression, Optimization & Stabilization

Phase 2.1C will be the final stabilization pass before Phase 2.1 is considered complete.

Planned work:

- Full regression testing of Phase 1, Phase 2, Phase 2.1A, and Phase 2.1B
- Repeated day/night/rain/clear-weather testing
- 2, 5, 10, 20, and 30-villager stress tests
- Single-door traffic tests
- Double-door traffic tests
- Blocked and unreachable entrance tests
- Multi-room building tests
- Multi-story building tests
- Basement tests
- Large custom-building stress tests
- Reservation and temporary-state cleanup
- Door ownership cleanup
- Performance checks
- Reduced unnecessary pathfinding and repeated building scans
- SPC regression testing
- WorldEdit regression testing
- Existing-world compatibility testing
- Final documentation cleanup
- Final manual gameplay verification

Phase 2.1 will only be marked stable after automated testing and real gameplay testing both pass.

## Future Development Roadmap

### Phase 3 — Social & Danger Awareness

Phase 3 will make villagers feel more aware of each other and their surroundings while keeping the classic Minecraft 1.0 style.

Planned features include:

- Lightweight villager social behavior
- Small natural villager groups
- Reduced unnecessary isolation
- Basic danger awareness
- Better reactions to nearby zombies
- Better reactions to creepers
- Fire awareness
- Lava avoidance
- Cactus avoidance
- Dangerous-drop avoidance
- Simple panic and escape behavior
- Improved hazard pathfinding

The goal is not to create modern Minecraft villager AI, but to make classic villagers feel less unaware of obvious danger.

---

### Phase 4 — Villager Variety

Phase 4 will improve visual variety while preserving the classic Minecraft 1.0 appearance.

Planned features include:

- More natural distribution of existing villager appearances
- Preservation of original Minecraft 1.0 profession/appearance IDs
- Additional classic-style villager varieties where appropriate
- Low-resolution textures designed to match the original 2011 art style
- SPC-spawned villager variants remain supported

No modern workstation or profession system will be added.

---

### Phase 5 — Farm Protection & Final v1.0 Polish

Phase 5 will focus on village farms and final release preparation.

Planned features include:

- Villagers avoid trampling farmland
- Passive mobs avoid unnecessary farmland trampling where practical
- Player movement does not unintentionally break the mod's farm logic
- Normal crop growth remains unchanged
- Normal crop planting and harvesting remain unchanged
- Water hydration behavior remains unchanged
- Final compatibility testing
- Final performance testing
- Final bug fixes
- Public v1.0 release preparation

---

## Possible Updates After v1.0

### v1.1 — Village Personality Update

Possible features:

- Lightweight villager personality traits
- Social villagers
- Shy villagers
- Wanderers
- Homebodies
- Curious villagers
- Small differences in preferred wandering behavior
- House preferences
- Profession-biased daytime movement
- More natural idle behavior
- Improved morning routines
- Additional villager skins and polish

These personalities would remain lightweight and would not introduce modern villager mechanics.

### v1.2 — Village Expansion Tools

Possible SPC-integrated village tools:

- `/villagegen`
- Generate a new classic-style village near the player's position
- Detect an existing village and expand it instead of creating a second overlapping village
- Terrain-aware building placement
- Connected roads
- Safe avoidance of important player structures
- Village generation preview
- Confirmation before world changes
- Undo support
- Newly generated village areas automatically recognized by Better 1.0 Villagers

This feature is planned for the future and is not part of the current Phase 2.1 development.
