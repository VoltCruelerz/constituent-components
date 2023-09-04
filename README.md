# Constituent Components

_This mod requires Greed 1.5.0 or higher._

Most of the components in Sins II are cool, but some leave something to be desired.

## Changes

### Existing Components

- **Antimatter Engine**
    - autocast: now exists (triggers at <40% antimatter)
- **Combat Repair System**
    - autocast: now exists (triggers at 300hp missing)
    - healing: affects the fleet for 1/3 rate (5hps)
- **Derelict Specialists**
    - changed to Tier 1
    - added unique icon
- **Exotics Salvage Policy**
    - installation: 120 => 30 seconds
- **Heavy Gauss Slugs**
    - armor penetration: removed
    - armor shred: 15% for 30s, no stacking
- **Reserve Hangar**: removed restriction on already having a squadron
- **Salvage Kit**
    - scaling: now scales with combat repair droid research for 10/20/30 HPS
    - targeting: can now apply to repair allied units as well
- **Volatile Accelerants**: passively grants +25% linear and angular speed
- **Missile Armor**: replaced with specialized variants. All types slow by 10% and grant +50 armor.
    - **Explosive Reactive Armor**: -40% missile and plasma damage
    - **Hylon Fiber Armor**: -40% phase gun and autocannon damage
    - **Ablative Ice Armor**: -20% beam and laser damage

### New Components

- **Unbreachable Hull**
    - _Unbreachable Hull_ research is a prerequisite
    - +2000 hull, +0.4 HPS, +75 armor

### Other Changes

- **Archaeology Center Prototype**: clarified text. Did _you_ know it gives you a cache of resources every 8 min? I sure didn't.

## Installation

**NOTE:** This mod requires [Greed](https://github.com/VoltCruelerz/Greed).

1. Download the latest release from [here](https://github.com/VoltCruelerz/constituent-components/releases)
2. Extract the zipped contents to `C:\Users\YOUR_USER\AppData\Local\sins2\mods\`, so that this file's path is `C:\Users\YOUR_USER\AppData\Local\sins2\mods\constituent-components\README.md`

## Future Work

- **Logistic Command**: increase productivity of factories while ship is in orbit
    - see `"factory_unit_build_price"`, `"factory_unit_build_time"`, `"factory_exotic_build_time"`
- **Mining Command**: increase productivity of mining while ship is in orbit
    - see `"orbital_extraction_metal_income_rate"`, `"orbital_extraction_crystal_income_rate"`
- **Martial Command**: planet regenerates loyalty (health) faster while ship is in orbit and strongly rejects hostile culture
    - see `"culture_resistance_rate"` and `"health_points_restore_rate"`
- **Excavation Team**: greatly reduces the time and cost of excavation
    - see `"excavation_track_build_price"` and `"excavation_track_build_time"`
- **Electronic Warfare**: enemy range reduced
- **Designated Target**: target takes additional damage
    - see Adaptive Force field, `"damage_taken"`
- **Sabotage Crews**: greatly reduces counterdeployment rates
    - see `"factory_unit_build_price"` and `"factory_unit_build_time"`
- **Supplemental Construction**: spawns another construction frigate that lasts for 10ish minutes
    - see `"structure_builder_count"`
- **Titan's Fervor**: Ankylon component that increases local garrison supply
- **Research Laboratory**: The ship counts as lab
    - see `"civilian_research_points"`, `"military_research_points"`, and `"research_time"`
- **Forward Deployment**: quickly set up ??? in remote gravity wells
    - see Argonev deployment
- **Networked Jump Computer**: greatly reduces the jump time of nearby allies, as well as jump speed
    - see `"hyperspace_charge_time"` and `"hyperspace_speed"`
- **Networked Airwing Command**: boosts flight speed of all strikecraft in gravity well
    - see Volatile Accelerants
- **Settlement Team**: ship gains colonize ability
- **Atmospheric Shielding**: strikecraft can bomb planets
- **Wide Frequency Jammer**: mass disable for everyone on the map
- **Parley**: Pay off pirates to reduce bounty
- **Privateers**: Hire some pirates

### Tradeoffs

- **Power Redirect - Weaponry**: massively boosts damage and rate of fire at the cost of speed
- **Power Redirect - Engines**: massively boosts maneuverability at the cost of rate of fire and damage
- **Power Redirect - Shields**: massively boosts shield regeneration and mitigation at the cost of weaeponry and maneuverability
- **Power Redirect - Abilities**: massively reduces cooldown at the cost of weaponry and maneuverability
