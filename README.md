# Constituent Components

_This mod requires Greed 1.8.1 or higher._

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
- **Sabotage Crews (Rebels)**
    - A lategame offensive unit for TEC Rebels, when used, it deals damage to enemy factories in the gravity well and slows production to a crawl.
    - 2000 damage, -45% build speed
- **Titan's Fervor (Loyalist)**
    - A lategame Ankylon component that grants any planet it orbits 50 garrison supply for as long as it remains there.
- **Deploy Constructor**
    - Game-start component that deploys a limited-lifetime constructor fully under manual control. The planet will not auto-schedule its jobs.

### Other Changes

- **Archaeology Center Prototype**: clarified text. Did _you_ know it gives you a cache of resources every 8 min? I sure didn't.

## Future Work

### TEC

- **Mining Command**: increase productivity of mining while ship is in orbit
    - see `"orbital_extraction_metal_income_rate"`, `"orbital_extraction_crystal_income_rate"`, `"on_current_spawner_current_gravity_well_changed"`
- **Logistic Command**: increase productivity of factories while ship is in orbit
    - see `"factory_unit_build_price"`, `"factory_unit_build_time"`, `"factory_exotic_build_time"`, `"on_current_spawner_current_gravity_well_changed"`
- **Martial Command**: planet regenerates loyalty (health) faster while ship is in orbit and strongly rejects hostile culture
    - see `"culture_resistance_rate"` and `"health_points_restore_rate"`
- **Electronic Warfare**: enemy range reduced
- **Designated Target**: target takes additional damage
    - see Adaptive Force field, `"damage_taken"`
- **Parley**: Pay off pirates to reduce bounty
- **Wide Frequency Jammer**: mass disable for everyone in orbit

### Vasari

- phase missiles: thematics?
- beams: anti-armor
- pulse beams: extreme anti-armor at the cost of damage
- waves: high damage, high RoF, shield popping
- pulse guns: basic, quick tracking

- [Kortul/Vulkoras] **Electroseeking Nanites**: Bonus damage on-hit to enemy that lacks full hull.
- [Antorak] **Phase Bomb**: Single-use that phases out a massive area briefly, dealing mild damage to _everything_, including allies, strikecraft, and missiles.
- [Jarrasul] **Speed Boost**: Boost early colonization?
- [Vulkoras] **Expendable Engines**: missile top speed +25%
- [Vulkoras] **Subspace Warheads**: missiles deal AoE damage
- [Skirantra] **Atmospheric Shielding**: own strikecraft can bomb planets
- [Skirantra] **Subspace Engines**: own strikecraft go _much_ faster
- **Ionized Waves**: Wave cannons deal bonus damage to shields
- **Defense Matrix**: Point defense guns of nearby allies improve _drastically_
    - probably with RoF or gimbal rate?
- **Debris Harvester**: Harvest debris from enemies?
- **Phase Sensor**: unit that detects incoming phase jumps
    - early-game
- **Phase Jump Inhibitor**: titan upgrade that locks down the well.
    - late-game
- **Excavation Team**: greatly reduces the time and cost of excavation, increases rate of success
    - early-game
    - see `"excavation_track_build_price"` and `"excavation_track_build_time"`
- **Research Laboratory**: The ship counts as lab
    - see `"civilian_research_points"`, `"military_research_points"`, and `"research_time"`
- **Networked Jump Computer**: greatly reduces the jump time of nearby allies, as well as jump speed
    - see `"hyperspace_charge_time"` and `"hyperspace_speed"`
    - would this be better for Vasari?
- **Networked Airwing Command**: boosts flight speed of all strikecraft in gravity well
    - see Volatile Accelerants
- **Nanomedicine Field Hospital**: _drastic_ reduction in bombing damage to _anyone_, increases allied loyalty, and generates favor _quickly_.
    - Should allow planet to survive Novaliths.

#### Rebels

- copy items from other factions
    - TEC
        - Armor boosts
        - Hosted Market: collect taxes on the ship
    - Advent
        - Beam Damage Boost

#### Loyalists

- **Scorched Earth**: increases bombing damage by 40%, instills a buff that reduces population growth by 80% for 10 minutes.

### Tradeoffs

- **Power Redirect - Weaponry**: massively boosts damage and rate of fire at the cost of speed
- **Power Redirect - Engines**: massively boosts maneuverability at the cost of rate of fire and damage
- **Power Redirect - Shields**: massively boosts shield regeneration and mitigation at the cost of weaeponry and maneuverability
- **Power Redirect - Abilities**: massively reduces cooldown at the cost of weaponry and maneuverability

### Maybe Someday

- Casaba Howitzers
- Missiles Have Riders
- Missile Retargeting
- Flares
- Missile Jammer
