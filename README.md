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

#### Phase 2.1 — Shelter Traffic & Building AI 🔧

Phase 2.1 is a major polish pass for shelter navigation, crowded entrances, doors, and larger buildings.

Already implemented or being refined:

- Faster night and rain shelter navigation
- Reduced unnecessary circling around houses
- Villagers commit more reliably to their selected shelter
- Improved waiting behavior around busy entrances
- Better double-door support
- Villagers can use both sides of double-door entrances
- Major reduction in repeated door opening/closing sounds
- Improved coordination between villagers using the same entrance
- More reliable automatic door closing after traffic clears
- Better support for large and multi-room buildings
- Villagers should leave large buildings properly during daytime
- Villagers should spread around the inside of houses instead of packing into one area
- Improved entrance queueing to reduce villagers pushing and cramming together
- All large-building improvements are designed to work generically and are not hardcoded for one specific world or building

Phase 2.1 is currently undergoing final testing and bug fixes before being marked stable.
