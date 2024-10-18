# VB4X Specification v0.1

Written by Mason A. Green
2024

# 1\.0 Introduction

VB4X is a space based wargame of the classic eXplore, eXpand, eXploit, and eXterminate (4X) variety for two to nine players. Upstart Emperors battle over a small region of space to dominate usurpers and seize the imperial throne. The game starts at the dawn of the third imperium in year 2001. Each turn comprises one month of a thirteen month [Terran Computational Calendar](<https://www.terrancalendar.com/> "Terran Computational Calendar"). Turns cycle every 24-hours in real life (IRL) time.

The game is designed to facilitate remote play (play by email [PBEM], chat, server based, etc.), although IRL turn length may be modified for table top wargaming over the course of several hours.

VB4X is intended to be a relatively simple and flexible framework; adapt it to your own requirements.

VB4X pays homage and incorporates ideas from the following great titles:

- Esterian Conquest (EC)

- Victory by Any Means (VBAM)

- Empire of The Sun (EOS)

- Space Empires 4X (SE4X)

Although not required, it is highly recommended to purchase physical copies of these classics to fully appreciate the prior art.

Esterian Conquest was a bulletin board system (BBS) door game from the early 1990's that initially inspired this project.

VB4X should be simple enough to run from a well organized Excel spreadsheet. It's just data and your imagination, after all.

Paper and pencil may do the trick. Campaigns that are computer or third party moderated meet the sweet spot with fog of war elements.

While not intended to be an accounting exercise, there is enough complexity in VB4X to allow for dynamic strategic decision making and surprising outcomes.

Victory is achieved when all homeworlds are captured or subjugated.

# 2\.0 Assets

## 2\.1 Starmap

The starmap consists of a 2D hexagonal grid, each a flat-top hex that contains a solar system, interconnected throughout by procedural generated jump lanes. The map is sized by rings around the center hub, one per number of upstart Empires.

The map takes inspiration from VBAM, and the 1st or 2nd edition campaign guides may be used to spawn a random map. The method is briefly explained below.

The center of the map is a special hub occupied by the last holdouts of the former imperial empire. This system is heavily guarded by fighter squadrons and the home planet and is similarly fortified against invasion. The former Emperor has no offensive Naval assets to speak off, which were scuttled by their crews at the height of the collapse. This is prime territory ripe for the taking. He who controls the hub holds great strategic power.

Solar systems have special traits and are procedural generated. Some are rocky atmospheric planets similar to earth and prime for colonization, the former occupants nuked by the mad imperial emperor. Others host rocky barren planets with little to no atmosphere that require terraforming before settlement. The remaining solar systems are filled with gas giants, hostile moons, and asteroids belts that are only only good for hosting bases and mining operations.

There are three classes of jump lanes: restricted, minor, and major. The hub is guaranteed to have six jump lanes connecting it to the first ring, making it an important strategic asset. Homeworlds on the outer ring will have three lanes. The number of lanes connecting the other hexes are randomly generated in accordance with VBAM. The class of all lanes are random.

Movement across the lanes is explained in Section 4.

Empires start the game with one homeworld, 50 production points, a planetary shipyard, two ETACs, a cruiser, two destroyers, and a scout. An Empire's homeworld should be placed on the outer ring, as far as strategically possible from enemy home sector(s).

Only one homeworld is allowed per Empire.

## 2\.2 Planets

### 2\.2.1 Planet Attributes

TODO: explain planet properties and formation.

### 2\.2.2 Terraforming and Colonization

Terraforming time takes XYZ turns to complete. 

Colonization takes one turn to complete.

## 2\.3 Ships, Squadrons, Fleets, and Task Forces

### 2\.3.1 Ships

#### 2\.3.1.1 Combat Ships

The base game includes a number of imperial classed combatants, listed in Section 9. 

Feel free to create your own ships and races for asymmetrical warfare or narrative purposes.

#### 2\.3.1.2 Merchant Marine Ships

Merchant marine ships are civilian crewed ships that provide logistal and economic support for the empire. They have no weapons technology or defense, and are easily captured or destroyed by enemy combat ships. Protect them wisely with military escorts.

**Environmental Transformation And Colonization (ETAC)** ships are used to terraform and colonize uninhabited planets. After colonization they are scrapped and used by the colony.

**Trader** ships earn Production Points (PP) by trading between colonies within the empire or with trade partners. They must have an uncontested path back across jump lanes to a friendly colony in order facilitate merchant activity. Systems may only have one trader assigned per empire.

**Miner** ships earn PP by harvesting raw materials from inhospitable, unoccupied gas systems. They must have an uncontested path back across jump lanes to a friendly colony in order to deliver raw materials. Systems may only have one miner assigned per empire.

Merchant Marine attributes are found in Section 9.

### 2\.3.2 Squadrons

Combat ships are organized into squadrons. Each squadron is commanded by a flagship with a Command Rating (CR) that will accommodate ships with a Command Cost (CC) that sum to less than or equal to the CR. This enables players to tactically group various classes of ships to balance combat effectiveness.

Squadrons fight as a unit and die as a unit. A squadron's total AS and DS values constitute a sum of all the ships under a flagship's command (including itself).

In non-hostile systems, ships in a squadron may be reassigned to an already existing squadron if the new flagship's CR allows. Squadrons may constitute a solo flagship. 

Squadrons are only commissioned in systems with a functioning shipyard.

### 2\.3.3 Fleets

Squadrons are grouped together into fleets for the purpose of traversing jump lanes. Fleets may be joined or split off (creating new fleets) for strategic purposes in any non-hostile system. There is no limit to the number of squadrons assigned to a fleet.

### 2\.3.4 Task Force

A Task Force is temporary grouping of squadrons organized for combat. After the cesattion of hostilities the task force is disbanded and surviving squadrons return to their respective fleets.

## 2\.4 Special Units

### 2\.4.1 Fighter Squadrons & Carriers

Fighters are commissioned in squadrons and freely patrol solar systems. They are small ships that require a carrier to move between systems.

There is no limit on the number of fighter squadrons deployed in a system, and they operate independently from carriers in said system.

Carriers hold up to three fighter squadrons. Super carriers hold up to five.

### 2\.4.2 Scouts

Scouts are autonomous drones outfitted with advanced sensors that aid with electronic warfare. They give a boost to Task Forces during combat operations.

### 2\.4.3 Raider Cloaking

Raiders are the only ships outfitted with cloaking technology. They are not available until cloaking technology is researched and developed.

Fleets containing a Raider have a 33% chance (roll 1 or 2 on a 1D6) of going undetected in hostile systems. The number of Raiders in the fleet does not affect the roll, nor rate multiple chances.

### 2\.4.4 Starbases

Starbases are powerful orbital fortresses that facilitate planetary defense and economic development via ground weather modification and advanced telecommunications. These powerful sentinels are limited to one operational unit per solar system.

Starbases require five months (five turns) to construct and require an orbital shipyard to build. They may be destroyed by hostile forces while under construction. The invested PP are lost forever. Unfinished Starbases may not contribute to defense and their benefits do not incur until 100% complete.

Starbases boost the morale of a colony by XYZ and production by XYZ every turn. Crippled Starbases operate at 50% capacity and contribute half their normal moral and PP to the colony.

### 2\.4.5 Shipyards

There are two classes of shipyards: planetary and orbital. There is no limit to the number of shipyards located in a solar system. 

Planetary Shipyards require two months (two turns) to construct and Orbital Shipyards require three months (three turns) to construct. 

Planetary yards are immobile, although they are defended by planetary resources during an attack.

Both types are manned and operated by civilian contractors and have no offensive or defensive capability.

### 2\.4.6 Planetary Shields & Ground Batteries

Planetary shields and Ground Batteries are planet based assets that provide an extra layer of defense to an Empire's colonies.

Planetary shields are restricted to homeworlds and provide system-wide electronic jamming that aids your Task Force in space combat on the home front. They also serve to protect your homeworld from orbital bombardment. They are restricted to one unit per homeworld.

Ground batteries are immobile, low-tech, land based units that have the firepower of a battleship at half the cost. They lob kinetic shells into orbit and are not upgraded by technology and research.

Ground batteries are the only units that are constructed in the span of a single turn. Colonies may build them to no limit.

### 2\.4.7 Troop Transports, Space Marines, & Armies

Troop transports are large size ships used to taxi Space Marines from one planet to another. It holds one Marine division and is not armed. This ship will drop troops on an enemy planet during an invasion or blitz.

Troop Transports are not assigned to squadrons.

Space Marines are ferocious devil dogs that capture enemy planets. They deploy in division sized units and will never surrender or abandon one of their own.

Armies garrison your colonies and eradicate invaders. Their orders are to take no prisoners and protect the colony at all cost.

## 2\.5 Asset Construction, Repair, and Tech Upgrades

Asset construction, repair, and tech upgrades are performed at planetary and orbital shipyards. Construction capacity at the yard is limited by the colony's total production capacity value, regardless of PP in the Empire's treasury.

Military ships may be upgraded with weapons tech unless otherwise specified. Ground units and planetary shields may not.

Orbital shipyards stationed in uninhabited gas systems are limited by the mining capacity of the system.

The number of turns required to construct an asset, unless otherwise specified, is equal to the PC times 0.5 (rounded down). Assets remain docked in the shipyard through the construction period. If the yard is destroyed, the uncomissioned assets are destroyed along with the PP invested.

The act of raising Armies and Space Marines, building Ground Betteries, and installing Planetary Shields does not require a shipyard.

# 3\.0 Turn Sequence

1. Economics

2. Turn Orders

3. Movement

4. Diplomacy

5. Supply

6. Combat

7. Construction

8. Tech & Research

9. Update

# 4\.0 Movement

## 4\.1 Escorts

If Orbital Shipyards or Starbases are ordered to move, they must be accompanied by a fleet escort. They can not move across jump lanes unassisted.

Merchant Marine ships may join a fleet for escort.

# 5\.0 Combat

## 5\.1 Basic Principles

**Combat Effectiveness Rating (CER)**: A modified 1d10 roll applied to a combat unit’s attack strength (anti-ship, anti-fighter, anti-planet, anti-ground) for the purposes of crippling and destroying your opponent’s forces. There are two separate CER tables, one for space combat and another for ground combat.

**Rules of Engagement (ROE)**: Dictates how aggressive your fleet will respond when engaging with the enemy from a scale of 0 to 10. The higher the ROE, the more aggressive your fleet will engage with enemy fleets of increasing relative strength to your own. With a low ROE, your fleet will attempt to retreat more readily when engaged in combat. A low ROE does not guarantee survival against a more powerful fleet. Once engaged, fleets have the opportunity to retreat only after the first round of combat.

**Rules Of Engagement Table**

| **ROE**                                              | **ORDERS**                                           |
| ---------------------------------------------------- | ---------------------------------------------------- |
| 00                                                   | Avoid all hostile forces. (Non-combat forces)        |
| 01                                                   | Engage forces only if they are defenseless.          |
| 02                                                   | Engage forces only if your AS is 4:1 or better.      |
| 03                                                   | Engage forces only if your AS is 3:1 or better.      |
| 04                                                   | Engage forces only if your AS is 2:1 or better.      |
| 05                                                   | Engage forces only if your AS is 3:2 or better.      |
| 06                                                   | Engage hostile forces of equal or inferior strength. |
| 07                                                   | Engage hostile forces even if outgunned 3:2.         |
| 08                                                   | Engage hostile forces even if outgunned 2:1.         |
| 09                                                   | Engage hostile forces even if outgunned 3:1.         |
| 10                                                   | Engage hostile forces regardless of their size.      |

**Combat State**: Combat ships are either undamaged or reduced in a crippled state. The reduction cycle goes from undamaged to crippled to destroyed.

**Undamaged**: A unit’s hull integrity and life support systems are fully operational. No restrictions.

**Crippled**: When an undamaged military unit’s Defense Strength (DS) is overcome (breached) in battle, that unit’s primary defense shielding is compromised and will find itself in a reduced, crippled combat state. AS is reduced by half. Subsequent damage sustained equal in full to DS will result in a catastrophic, unrecoverable, loss of hull integrity, i.e. destruction. 

DS is a fixed constant that shall not be reduced at any time during sustained combat operations.

**Destroyed**: Dead and unrecoverable.

**Space Combat Results Table**

| **Modified 1D10 Die Roll**            | **Combat Effectiveness Rating (CER)** |
| ------------------------------------- | ------------------------------------- |
| Less than zero, 0, 1, 2               | One Quarter (0.25) (round up)         |
| 3, 4                                  | One Half (0.50) (round up)            |
| 5, 6                                  | Three Quarters (0.75) (round up)      |
| 7, 8                                  | One (1)                               |
| 9                                     | One\* (1)                             |
| 9+                                    | One (1)                               |

\* If the die roll is a natural nine before any required modification, then a critical hit is achieved

**Battle Stations Table**

| **1D6 Roll**                          | **Battle Stations Modifier**          |
| ------------------------------------- | ------------------------------------- |
| 1                                     | Crews are a distracted mess (-2)      |
| 2                                     | Crews are scrambling (-1)             |
| 3, 4                                  | Crews are at the ready (0)            |
| 5                                     | Crews are on point (1)                |
| 6                                     | Crews are out for blood (2)           |

**Ground Combat Results Table**

| **Modified 1D10 Die Roll**            | **Combat Effectiveness Rating (CER)** |
| ------------------------------------- | ------------------------------------- |
| Less than zero, 0, 1, 2               | One Half (0.5) (round up)             |
| 3, 4, 5, 6                            | One (1)                               |
| 7, 8                                  | One and a half (1.5) (round up)       |
| 9 or more                             | Two (2)                               |

## 5\.2 Task Force Assignment

All of a player’s fleets arriving at a star system in the same turn, and fleets already located in said system, are joined together into a single Task Force when battle commences. Fleets are temporarily disbanded and their collective squadrons fight under the Task Force as a monolith.

Task Forces assume the highest ROE of any fleet in their force.

Fighter squadrons deploy to their player's respective Task Force as independent squadrons.

Fleets that are cloaked, and remain undetected, may continue traveling through jump lanes in a contested star system. Otherwise the fleet will join their player's respective Task Force for battle.

Starbases, Orbital Shipyards, Merchant Marine Ships, and Troop Transports are screened behind the Task Force during combat operations and do not engage.

## 5\.3 Retreat

A Task Force may retreat from combat only after the first round of combat, in accordance with their ROE, and between rounds thereafter. The ROE is fixed at the beginning of combat and through all subsequent rounds.

A retreating Task Force will fall back to their original fleet formations and flee to the closest non-hostile star system.

### 5\.3.1 Starbases

Starbases never retreat from a solar system because of their massive size. They are too slow to maneuver.

Refer to Section 5.5 for handling orphaned assets if a Starbase is abandoned by a fleeing Task Force. 

### 5\.3.2 Fighter Squadrons, Troop Transports, Merchant Marine Units, and Orbital Shipyards

Orphaned fighter squadrons are scuttled if there is no carrier capacity available for a retreat.

Troop transports are captured and the Space Marines enslaved if their escort fleet was destroyed or the transports were unescorted at the commencement of hostilities.

Merchant Marine Ships rejoin their surviving escort fleets. If the fleet was destroyed or the ships were unescorted before hostilities, they are captured as spoils of war.

Like Starbases, Orbital Shipyards are too large and complex to retreat in an expidited manner. They are rigged to self detonate before capture.

This section is null and void if Section 5.3.1 is in effect.

## 5\.4 Space Combat

After Task Forces are aligned for battle, combat commences in a series of rounds until one side is completely destroyed or manages a retreat.

Combat action is simultaneous; all squadrons have the opportunity to fire on enemy forces at least once, regardless of damage sustained during a round.

At the beginning of each combat round, players add up the total AS of their surviving squadrons. The total value is then modified by the following:

Players roll a die in accordance with The Space Combat Results Table to determine their CER, applying all applicable modifiers.

The CER multiplied by AS equals the number of enemy hits.

**Die Roll Modifiers**

- Battle Stations Table: Roll every round

- Scouts active in the Task Force: +1 max

- Homeworld protected by shields in the contested system: -2 to opposing Task Forces   

The player who rolled the die will determine where hits are applied within the following restrictions:
1. If the number of hits equal the opposing squadron's DS, the unit is reduced.
2. Squadrons are not destroyed until all other squadrons in the Task Force are crippled.
3. Excess hits may be lost if restrictions apply.

Crippled squadrons multiply their AS by 0.5, rounded up the nearest whole number.

Destroyed squadrons are no longer a factor and the Task Force loses their associated die roll modifiers (e.g. Scouts).

In computer moderated play, the algorithm will reduce squadrons with the greatest AS to ensure maximum damage, within restrictions.

### 5\.4.1 Critical Hits

Critical hits are a special case. Restriction #2 above is nullified. 

Additionally, if a player takes a critical hit and is unable to reduce a unit according to condition #1 above, then the squadron with the lowest DS is reduced.

### 5\.4.2 End of Round

After all hits are applied and squadrons are appropriately reduced (crippled or destroyed), the next round commences via the same procedure above.

### 5\.4.3 End of Combat

After the last round of combat the surviving Task Forces are disbanded and surviving squadrons rejoin their assigned fleets. 

Retreating Task Forces must comply with the rules in Section 5.3.

### 5\.4.4 Example Combat

## 5\.5 Starbases

If an enemy fleet has orders to bombard, invade, or blitz a colony, a Starbase provides the first line of planetary defense.

In the special circumstance that an escorted Starbase is orphaned by a retreat, the Starbase will screen other orphans and go straight to combat against enemy forces.

## 5\.6 Planetary Bombardment

## 5\.7 Planetary Invasion, Blitz, and Ground Combat

# 6\.0 Economics

The unit of account is the Production Point (PP).

## 6\.1 Colony Production

## 6\.2 Trading & Mining

## 6\.3 Asset Maintenance Costs

# 7\.0 Technology & Research

Technology upgrades may be purchased in the first and sixth months of the Terran calendar, i.e. the first and sixth turns of each game year.

# 8\.0 Diplomacy & Subversion

# 9\.0 Asset Tables

## 9\.1 Imperial Navy

PC = Production Cost, MC = Maintenance Cost, AS = Attack Strength, DS = Defensive Strength,

CC= Command Cost, CR = Command Rating, CV = Carry Limit

| Class            | Name             | PC               | MC               | AS               | DS               | CC               | CR               | CL               |
| ---------------- | ---------------- | ---------------- | ---------------- | ---------------- | ---------------- | ---------------- | ---------------- | ---------------- |
| CT               | Corvette         | 2                | 0\.1             | 1                | 2                | 1                | 2                | 0                |
| FF               | Frigate          | 3                | 0\.2             | 2                | 3                | 2                | 3                | 0                |
| DD               | Destroyer        | 4                | 0\.3             | 3                | 4                | 2                | 4                | 0                |
| CA               | Cruiser          | 5                | 0\.4             | 4                | 5                | 3                | 6                | 0                |
| BC               | Battle Cruiser   | 6                | 0\.5             | 4                | 6                | 3                | 8                | 0                |
| BB               | Battleship       | 8                | 1\.0             | 6                | 8                | 3                | 9                | 0                |
| DN               | Dreadnought      | 10               | 1\.5             | 9                | 9                | 4                | 10               | 0                |
| CV               | Carrier          | 8                | 1\.0             | 1                | 6                | 3                | 8                | 3                |
| CX               | Super Carrier    | 10               | 1\.5             | 1                | 9                | 4                | 10               | 5                |
| FR               | Fighter Squadron | 3                | 0\.2             | 3                | 2                | 0                | 0                | 0                |
| RR               | Raider           | 7                | 0\.6             | 4                | 6                | 3                | 4                | 0                |
| SC               | Scout            | 5                | 0\.2             | 0                | 1                | 2                | 0                | 0                |
| TT               | Troop Transport  | 4                | 0\.2             | 0                | 1                | 0                | 0                | 3                |
| SB               | Starbase         | 50               | 2                | 35               | 50               | 0                | 0                | 0                |

## 9\.2 Merchant Marine

| **Class**          | **Name**           | **PC**             |
| ------------------ | ------------------ | ------------------ |
| MR                 | Miner              | 5                  |
| TR                 | Trader             | 6                  |
| ET                 | ETAC               | 15                 |
| PY                 | Planetary Shipyard | 15                 |
| SS                 | Shipyard           | 20                 |

## 9\.3 Ground Based Units

| **Class**        | **Name**         | **PC**           |
| ---------------- | ---------------- | ---------------- |
| PS               | Planetary Shield | 35               |
| GB               | Ground Batteries | 4                |
| AA               | Armies           | 2                |
| MM               | Space Marines    | 3                |

# 10\.0 Play By Excel
