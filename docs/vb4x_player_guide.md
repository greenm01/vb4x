# VB4X Player Guide

Written by Mason A. Green

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

TODO: explain planet properties, similar to VBAM.

### 2\.2.2 Terraforming and Colonization

Terraforming time takes XYZ turns to complete. ETACs may be destroyed by hostile forces when caught in the act.

Colonization takes one turn to complete.

## 2\.3 Ships, Squadrons, Fleets, and Task Forces

### 2\.3.1 Ships

#### 2\.3.1.1 Combat Ships

The base game includes a number of imperial classed combatants, listed in Section 9. Feel free to create your own ships and races for asymmetrical warfare or narrative purposes.

It is recommended to maintain the predefined classes and attribute categories, and only tweak the ship names and attribute values for new ships.

Ships that are crippled in battle require repair at a ship yard to restore their combat effectiveness. Older technology ships may be retrofitted with new weapons tech.

Refer to Section 6.4 in regard to ship construction, repair, and upgrades.

#### 2\.3.1.2 Merchant Marine Ships

Merchant marine ships are civilian crewed ships that expand and fill the coffers of the empire. They have no weapons technology or defense, and are easily captured or destroyed by enemy combat ships. Protect them wisely with military escorts.

**Environmental Transformation And Colonization (ETAC)** ships are used to terraform and colonize uninhabited planets. After colonization they are scrapped and used by the colony.

**Trader** ships earn Production Points (PP) by trading between colonies within the empire or with diplomatic trade partners. They must have an uncontested travel path back across jump lanes to an empire controlled colony.

**Miner** ships earn PP by harvesting raw materials from inhospitable, unoccupied systems. They must have an uncontested travel path back across jump lanes to an empire controlled colony.

Merchant Marine attributes are found in Section 9.

### 2\.3.2 Squadrons

Combat ships are organized into squadrons. Each squadron is commanded by a flagship with a Command Rating (CR) that will accommodate ships with a Command Cost (CC) that sum to less than or equal to the CR. This enables empires to tactically group various classes of ships together during combat to balance the squadron's Attack Strength (AS), Defensive Strength (DS), and protect special ships.

Carriers are treated just like any other ship and remain attached to their assigned squadron. Their child fighter squadrons deploy separately and remain wholly independent unit the Task Force is disengaged, returning back to surviving carriers (if there's room) or fight to the death if orphaned in a retreat.

Merchant Marine ships and star bases do not join squadrons.

Squadrons fight as a unit and die as a unit. A squadron's total AS and DS values constitute a sum of all the ships under its command.

In non-hostile systems, ships in a squadron may be reassigned to an already existing squadron if the new flagship's CR allows. Squadrons may constitute a solo flagship. Fighters remain housed within their respective carriers.

Squadrons are newly commissioned only in systems with a functioning ship yard.

### 2\.3.3 Fleets

Squadrons are grouped together into Fleets for the purpose of traversing jump lanes. Fleets may be joined or split off (creating new fleets) for strategic purposes in any non-hostile system. There is no limit to the number of squadrons assigned to a fleet.

Merchant Marine ships and star bases may join a fleet for escort.

### 2\.3.4 Task Force

All of an Empire’s fleets arriving at a system in the same turn, and all fleets already located in said system, are joined together into a single Task Force when battle commences between two or more hostile Empires.

Fleets that are cloaked, and remain undetected, may continue jumping through hyperspace to a different sector. Otherwise the fleet will join their Empire’s respective Task Force for battle.

Merchant marine ships do not join the Task Force. Refer to Combat procedures in Section 5.

## 2\.4 Special Units

### 2\.4.1 Fighter Squadrons & Carriers

Fighters are commissioned in squadrons. They are small ships unequipped with jump drives and may not move independently between systems.

There is no limit on the number of fighter squadrons deployed in a friendly system, and they operate independently from carriers in said system. Moving them to a new system requires a mother ship.

Carriers hold up to three fighter squadrons and are assigned to regular ship squadrons just like other ships. Super carriers can hold up to five fighter squadrons.

### 2\.4.2 Scouts

Scouts are small drones outfitted with advanced sensors that aid with electronic warfare. They give a boost to their Task Force during combat operations.

Multiple scouts assigned to a task force do not lend additional benefits in combat, although it may be prudent to tactically place Scouts in more than one squadron in the event of destruction.

### 2\.4.3 Raider Cloaking

Raiders are the only ships outfitted with cloaking technology. They are not available until cloaking technology is researched and developed.

Fleets containing a Raider have a 33% chance (roll 1 or 2 on a 1D6) of going undetected in hostile systems. The number of Raiders in the fleet does not affect the roll, nor rate multiple chances.

Like scouts, place Raiders in multiple squadrons to distribute risk across the fleet.

### 2\.4.4 Starbases

Starbases are powerful orbital fortresses that facilitate planetary defense and economic development via ground weather modification and advanced telecommunications. These powerful sentinels are limited to one operational unit per colony.

Because of mass restrictions and continuous supply requirements, star bases are not equipped with jump drives and may not move out of their home systems.

Starbases require five months (five turns) to build at a shipyard, and may be destroyed by hostile forces while under construction. The invested PP are lost forever. Unfinished Starbases may not contribute to defense and their benefits do not incur until 100% completed.

Starbases may be upgraded with weapons tech at 50% of the current PC.

Starbases boost the morale of a colony by XYZ and production by XYZ every turn.

Crippled Starbases operate at 50% capacity and contribute half their normal moral and PP to the colony.

### 2\.4.5 Ship Yards

There are two classifications of ship yards: planetary and orbital. There is no limit to the number of ship yards that may be constructed at a colony. Like Star Bases, they may not be moved out of their home systems.

Ship yards require three months (three turns) to construct and are vulnerable to attack. They are manned and operated by civilian contractors and have no offensive or defensive capability.

Refer to Section 6.4 in regard to ship construction, repair, and upgrades.

### 2\.4.6 Planetary Shields & Ground Batteries

Planetary shields and Ground Batteries are planet based assets that provide an extra layer of defense to an Empire's colonies.

Planetary shields are restricted to homeworlds and provide system-wide electronic jamming that aids your Task Force in space combat on the home front. They also serve to protect your homeworld from orbital bombardment. They are restricted to one unit per homeworld.

Ground batteries are immobile, low-tech, land based units that have the firepower of a battleship at half the cost. They lob kinetic shells into orbit and are not upgraded by technology and research.

Ground batteries are the only units that are constructed in the span of a single turn. Colonies may build them to no limit.

### 2\.4.7 Troop Transports, Space Marines, & Armies

Troop transports are large size ships used to taxi Space Marines from one planet to another. It holds one Marine division and is not armed. This ship will drop troops on an enemy planet during an invasion or blitz.

Space Marines are ferocious devil dogs that capture enemy planets. They deploy in division sized units and will never surrender or abandon one of their own.

Armies garrison your colonies and eradicate invaders. Their orders are to take no prisoners and protect the colony at all cost.

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



# 5\.0 Combat

## 5\.1 Basic Principles

**Combat Effectiveness Rating (CER)**: A modified 1d10 roll applied to a combat unit’s attack strength (anti-ship, anti-fighter, anti-planet, anti-ground) for the purposes of crippling and destroying your opponent’s forces. There are two separate CER tables, one for space combat and another for ground combat.

**Rules of Engagement (ROE)**: Dictates how aggressive your fleet will respond when engaging with the enemy from a scale of 0 to 10. The higher the ROE, the more aggressive your fleet will engage with enemy fleets of increasing relative strength to your own. With a low ROE, your fleet will attempt to retreat more readily when engaged in combat. A low ROE does not guarantee survival against a more powerful fleet. Once engaged, fleets have the opportunity to retreat only after the first round of combat.

Note that fleets *may* avoid engagement entirely if equipped with cloaking technology, and remain undetected while transiting *through* a hostile sector.

| **Rules Of Engagement Table** |
| ----------------------------- |
| **ROE**                       |
| 00                            |
| 01                            |
| 02                            |
| 03                            |
| 04                            |
| 05                            |
| 06                            |
| 07                            |
| 08                            |
| 09                            |
| 10                            |

**Combat State**: Combat ships are either undamaged or reduced in a crippled state. The reduction cycle goes from undamaged to crippled to destroyed.

**Undamaged**: A unit’s hull integrity and life support systems are fully operational. No restrictions.

**Crippled**: When an undamaged military unit’s Defense Strength (DS) is overcome (breached) in battle, that unit’s primary defense shielding is compromised and will find itself in a reduced, crippled combat state. Subsequent damage sustained equal in full to DS will result in a catastrophic, unrecoverable, loss of hull integrity, i.e. destruction. DS is a fixed constant value that shall not be reduced at any time during sustained combat operations.

**Destroyed**: Dead and unrecoverable.

**TABLES**:

| **Space Combat Results Table** |
| ------------------------------ |
| **Modified 1D10 Die Roll**     |
| 0, 1, 2                        |
| 3, 4                           |
| 5, 6                           |
| 7, 8                           |
| 9                              |
| 9+                             |

\* If the die roll is a natural nine before any required modification, then a critical hit is achieved

| **Battle Stations Preparedness Table** |
| -------------------------------------- |
| 1D6 Roll                               |
| 1,2                                    |
| 3,4                                    |
| 5,6                                    |

| **Ground Combat Results Table** |
| ------------------------------- |
| **Modified 1D10 Die Roll**      |
| Less than zero, 0, 1, 2         |
| 3, 4, 5, 6                      |
| 7, 8                            |
| 9 or more                       |

## 5\.2 Task Force Assignment

All of an Empire’s fleets arriving at a star system in the same turn, and fleets already located in said system, are joined together into a single Task Force when battle commences between two or more enemies.

Task Forces assume the highest ROE of any fleet in their force.

Task Forces are composed of individual squadrons led by a single flagship with a valid command rating (CR). All ships in a squadron act as a single unit and are crippled or destroyed together. Their AS and DS factors are summed together for battle. This gives an Empire tactical flexibility regarding which ships are grouped within a squadron, mixed and matched with various capabilities and special modifiers.

Fighter squadrons protecting their home system join their Empire's respective Task Force as regular squadrons. Hostile carriers deploy their own fighter squadrons in a similar fashion.

Fleets that are cloaked, and remain undetected, may continue traveling in hyperspace through a contested star system. Otherwise the fleet will join their Empire’s respective Task Force for battle.

## 5\.3 Retreat

A Task Force may retreat from combat only after the first round of combat, in accordance with their ROE, and between rounds thereafter. The ROE is fixed at the beginning of combat and through all subsequent rounds.

A retreating Task Force will fall back to their original fleet formations and flee to the closest non-hostile star system.

## 5\.4 Space Combat

Once Task Forces are committed to battle, combat commences in a series of rounds until one side is completely destroyed or manages a retreat.

Combat action is simultaneous; all assets will have the opportunity to fire on enemy forces at least once, regardless of damage sustained during a round.

In the first combat round only, both empires will roll on the Battle Stations Preparedness Table listed in 5.1. The result will be applied as a die roll modifier when rolling for the CER in *round one only*.

At the beginning of each combat round, Empires add up the total AS of their remaining squadrons. The total value is then modified by the following:

Each empire will roll a die in accordance with The Space Combat Results Table (Exhibit A) to determine their CER, applying modifiers.

The CER multiplied by AS represents the number of hits received by the enemy.

**Die Roll Modifiers**

- Battle Stations Preparedness Table (round one only)

- Functional Scouts (**\+1)**

- Homeworld planetary shields (**\-2)** (to the enemy's roll, all rounds)

All Task Force ships fire on one another simultaneously. Each empire receiving AS hits will decide which squadrons are crippled or destroyed if their squadron DS is breached. Crippled squadrons reduce their AS by multiplying by 0.5, rounded up the nearest whole number. Destroyed squadrons are no longer a factor and the Task Force loses their associated die roll modifiers (e.g. Scouts).

All hits must be applied, although there may hits that are ineffective if a squadron’s DS blocks it.

In computer moderated play, the algorithm will apply damage to squadrons with the lowest AS in order to sustain maximum offensive power for the Task Force. Die roll modifiers are a factor in the calculation.

Squadrons are not reduced and destroyed until all other squadrons in the Task Force are already crippled.

Critical hits are the exception to the aforementioned rule. The computer moderator will reduce a squadron with the highest rated AS regardless of combat state if DS is breached.

**Note**: Starbases do not join a Task Force. If an enemy Task Force has orders to bombard, invade, or blitz a colony the Starbase will engage with the hostile fleet from orbit as described in this section. Substitute Task Force and Squadron with Starbase in the battle procedure.

Merchant Marine ships are screened behind the Task Force during combat operations, and rejoin their surviving fleets during a retreat. If the fleet is destroyed they are captured as spoils of war.

Example Combat Round:

## 5\.5 Planetary Bombardment

## 5\.6 Planetary Invasion, Blitz, and Ground Combat

# 6\.0 Economics

The unit of account is the Production Point (PP).

## 6\.1 Colony Production

## 6\.2 Trading & Mining

## 6\.3 Asset Maintenance Costs

## 6\.4 Ship Construction, Repair, and Upgrades

Ship construction, repair, and tech upgrades are performed at planetary and orbital shipyards. Construction capacity at the yard is limited by the colony's total production capacity value, regardless of PP in the Empire's treasury.

The number of turns required to complete ship orders is equal to the unit PC times 0.5 (rounded down). Construction takes time. Ships remain docked in the ship yard through the entire process. If the construction yard is destroyed, the ships are destroyed in their slipways and the invested PPs are lost.

# 7\.0 Technology & Research

Technology upgrades may be purchased in the first and sixth months of the Terran calendar, i.e. the first and sixth turns of each game year.

# 8\.0 Diplomacy & Subversion



# 9\.0 Asset Tables

## 9\.1 Imperial Navy

PC = Production Point Cost, MC = Maintenance Cost, AS = Attack Strength, DS = Defensive Strength,

CC= Command Cost, CR = Command Rating, CV = Carry Capacity

| Class            | Name             | PC               | MC               | AS               | DS               | CC               | CR               | CV               |
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

# 10\.0 Example Excel Worksheets




