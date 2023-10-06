# Constituent Components

_This mod requires Greed 2.0.0 or higher._

Most of the components in Sins II are cool, but some leave something to be desired.

## Updated Components

### TEC Updates

- **Antimatter Engine**
    - autocast: now exists (triggers at `< 40%` antimatter)
- **Combat Repair System**
    - autocast: now exists (triggers at `300` HP missing)
    - healing: affects the fleet for 1/3 rate (`5 HPS`)
- **Derelict Specialists**
    - changed to Tier 1
    - added unique icon<br>![hud icon](textures/trader_derelict_specialist_unit_item_hud_icon.png)
- **Exotics Salvage Policy**
    - installation: `120` => `30` seconds
- **Heavy Gauss Slugs**
    - armor penetration: removed
    - armor shred: `15%` for `30s`, no stacking
- **Reserve Hangar**: removed restriction on already having a squadron
- **Salvage Kit**
    - scaling: now scales with combat repair droid research for `10/20/30 HPS`
    - targeting: can now apply to repair allied units as well
- **Volatile Accelerants**: passively grants `+25%` linear and angular speed
- **Missile Armor**: replaced with specialized variants. All types slow by `10%` and grant `+50` armor.
    - **Explosive Reactive Armor**: `-40%` missile and plasma damage<br>![hud icon](textures/trader_armor_specialization_missile_unit_item_hud_icon.png)
    - **Hylon Fiber Armor**: `-40%` phase gun and autocannon damage<br>![hud icon](textures/trader_armor_specialization_bullet_unit_item_hud_icon.png)
    - **Ablative Ice Armor**: `-20%` beam and laser damage<br>![hud icon](textures/trader_armor_specialization_energy_unit_item_hud_icon.png)

### Vasari Updates

For some reason, the Beam and Wave Modulators are both terrible, barely making a dent in a ship's overall DPS. For a component that is purely selfish, it's odd that they were so poorly-performing.

- **Nano Attack Swarm**: also deals `4 AMPS` (80 AM total)
- **Nano Repair Swarm**: while active, grants `30` armor.
- **Beam Moduator**: improved use as an anti-armor weapon
    - Passive Damage: removed
    - Passive Cooldown: `-40%/-80%`
    - Active Penetration: (`40/60%` => `75/150%`) = (`134/153 AP` => `168/240 AP`)
- **Wave Modulator**: improved shield cutting performance
    - Damage: `5/8%` => `20/30%`
    - Cooldown: `10/15%` => `15/20%`
    - DPS: `16/24%` => `38/56%`
- **Bomber Armor**: Fixed `1.16.10`'s component-not-selectable bug

## Added Components

### TEC Additions

- **Unbreachable Hull**
    - _Unbreachable Hull_ research is a prerequisite
    - `+2000` hull, `+0.4` HPS, `+75` armor
- **Sabotage Crews (Rebels)**<br>![hud icon](textures/trader_deploy_sabotage_crews_hud_icon.png)
    - A lategame offensive unit for TEC Rebels. When used, it deals damage to enemy factories in the gravity well and slows production.
    - `2000` damage, `-45%` build speed
- **Titan's Fervor (Loyalist)**<br>![hud icon](textures/trader_titans_fervor_hud_icon.png)
    - A lategame Ankylon component that grants any planet it orbits 50 garrison supply for as long as it remains there.
- **Deploy Constructor**<br>![hud icon](textures/trader_extra_constructor_hud_icon.png)
    - Game-start component that deploys a limited-lifetime constructor fully under manual control. The planet will not auto-schedule its jobs.

### Vasari Additions

- **Parasitic Payloads**<br>![hud icon](textures/vasari_breachseek_nanites_hud_icon.png)
    - Weapons deal `15%` bonus damage to targets missing hull points.
    - Higher research tiers upgrade the item to a small AoE (radius of `0/1000/1500` with target cap of `1/2/3`).
- **Subspace Sensor Array**<br>![hud icon](textures/vasari_subspace_array_hud_icon.png)
    - Increases weapon range by `10/20/30%`.
    - Increases bombing range by `0/150/200%`.
    - Ship counts as a mobile phase jump detector, with a range of `0/1/2` jumps.

### Other Changes

- **Archaeology Center Prototype**: clarified what this does in the UI

## Future Work

The below options are not firm plans, merely considerations.

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

- [Antorak] **Phase Bomb**: Single-use that phases out a massive area briefly, dealing mild damage to _everything_, including allies, strikecraft, and missiles.
- [Jarrasul] **Speed Boost**: Boost early colonization?
- [Vulkoras] **Staged Engines**: missile top speed +25%
- [Vulkoras] **Subspace Warheads**: missiles deal AoE damage
- [Skirantra] **Atmospheric Shielding**: own strikecraft can bomb planets
- [Skirantra] **Central Airwing Command**: boosts flight speed of all strikecraft in gravity well
    - see Volatile Accelerants
- **Subspace Tracker**: Applies a tracker to the target ship, allowing it to be tracked, wherever it goes.
    - See `provides_detection`.
- **Phase Jump Inhibitor**: titan upgrade that locks down the well.
    - late-game
- **Excavation Team**: greatly reduces the time and cost of excavation, increases rate of success
    - early-game
    - see `"excavation_track_build_price"` and `"excavation_track_build_time"`
- **Networked Jump Computer**: greatly reduces the jump time of nearby allies, as well as jump speed
    - see `"hyperspace_charge_time"` and `"hyperspace_speed"`
    - would this be better for Vasari?
- **Nanomedicine Field Hospital**: _drastic_ reduction in bombing damage to _anyone_, increases allied loyalty, and generates favor _quickly_.
    - Should allow planet to survive Novaliths.
- **Mobile Exotic Factory**: improve it _somehow_...
    - ?give small RNG buffs to strikecraft?
    - ?add slow resource generation too, since you're never that low on slots?

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
