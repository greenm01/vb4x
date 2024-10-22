# EC4X Specification v0.1

Written by Mason A. Green

In memory of Jonathan F. Pratt.

# Introduction

EC4X is an asynchronous turn based wargame of the classic eXplore, eXpand, eXploit, and eXterminate (4X) variety.

Upstart houses battle over a small region of space to dominate usurpers and seize the imperial throne. The game begins at the dawn of the third imperium in the year 2001. Each turn comprises one month of a thirteen month [Terran Computational Calendar](<https://www.terrancalendar.com/> "Terran Computational Calendar"). Turns cycle every 24-hours in real life (IRL) time.

The game is designed to facilitate remote play between friends over email or local tabletop play. Future releases will be server/client based and written in Rust. EC4X is a flexible framework; adapt it to your own requirements.

EC4X pays homage and is influenced by the following great titles:

- Esterian Conquest (EC)
- Victory by Any Means (VBAM)
- Empire of The Sun (EOS)
- Space Empires 4X (SE4X)
- Solar Starfire (SSF)
- Fractal, Beyond the Void (FBV)

Although not required, it is highly recommended to purchase physical copies of these classics to fully appreciate the art. Dive deep.

Esterian Conquest was a bulletin board system (BBS) door game from the early 1990's that initially inspired this project. EC was THE greatest game of all time (no arguments).

While not intended to be an accounting exercise, there is enough complexity in EC4X to allow for dynamic strategic decision making and surprising outcomes.

Victory is won by crushing your rivals and earning the most Prestige by end of game.

# 1.0 Turns

Each turn comprises four phases

1. Income phase
2. Command phase
3. Conflict phase
4. End of turn phase

# 2\.0 Game Assets

## 2\.1 Starmap

The starmap consists of a 2D hexagonal grid, each a flat-top hex that contains a solar system, interconnected throughout by procedural generated jump lanes. The map is sized by rings around the center hub, one per number of players.

The map takes inspiration from VBAM, and the 1st or 2nd edition campaign guides may be used to spawn a random map. The method is briefly explained below.

The center of the map is a special hub occupied by the last holdouts of the former imperial Empire. This system is heavily guarded by fighter squadrons and the home planet is fortified against invasion. The former Emperor has no offensive ships to speak of, which were scuttled by their crews at the height of the collapse. This is prime territory ripe for the taking. He who controls the hub holds great strategic power.

Solar systems have special traits and are procedural generated. They are filled with planets, moons, and gas giants that are variable in their suitability for colonization and production.

There are three classes of jump lanes: restricted, minor, and major. The hub is guaranteed to have six jump lanes connecting it to the first ring, making it an important strategic asset. Homeworlds on the outer ring will have three lanes. The number of lanes connecting the other hexes are randomly generated in accordance with VBAM. The class of all lanes are random.

Movement across the lanes is explained in Section 4.

Players start the game with one homeworld (Class H2 with rich raw materials and a settlement sized colony of 61 PU) 50 Satoshis (SAT) in the treasury, one spaceport, one shipyard, one fully loaded ETAC, a cruiser, two destroyers, and a scout. 

Each player's homeworld should be placed on the outer ring, as far as strategically possible from enemy home system(s).

## 2\.2 Solar Systems

Solar systems contain various F, G, K, and M class stars that are orbited by at least one terrestrial planet, suitable for colonization and terraforming. Otherwise systems are not charted and of no consequence to the task at hand.

Roll on the planet class and system resources tables below to determine the attributes for each hex on the starmap, excluding homeworlds.

Note that each newly established colony begins as Level 1 and has potential to develop into the max Population Unit (PU) for that planet. Ferry colonists from larger colonies to smaller colonies, via starliners, to increase population growth over the natural birth rate. 

Advances in terraforming tech will allow planets to upgrade class and living conditions.

**Planet Class Table**

| Roll 1D10 | Class | Conditions | Colony Potential | PUs     |
|:---------:|:-----:| ---------- | ---------------- |:-------:|
| 0         | E0    | Extreme    | Level I          | 1-20    |
| 1         | E1    | Extreme    | Level II         | 21-60   |
| 2, 3      | D0    | Desolate   | Level III        | 61-180  |
| 4, 5      | D1    | Desolate   | Level IV         | 181-500 |
| 6, 7      | H0    | Habitable  | Level V          | 501-1k  |
| 8*        | H1    | Habitable  | Level VI         | 1.1k-2k |
| 9*        | H2    | Habitable  | Level VII        | 2.1k+   |

\*Note: if the roll above is a natural eight (8), add a +1 modifier to your roll on the raw materials table. If the roll is a natural nine (9) add a +2 modifier.

**System Resources Table**

| Mudified Roll 1D10 | Raw Materials |
| ------------------ | ------------- |
| 0                  | Very Poor     |
| 2, 3               | Poor          |
| 4 - 7              | Abundant      |
| 8, 9               | Rich          |
| 10+                | Very Rich     |

## 2.3 Ships, Squadrons, Fleets, and Task Forces

### 2\.3.1 Space Force Ships

The base game includes a number of imperial classed space combatants listed in Section 9.

Feel free to create your own ships and races for asymmetrical warfare or narrative purposes.

### 2\.3.2 Merchant Marine Ships

The Merchant marine fleet comprises civilian crewed ships that provide commerce and transport services for the House. They have no weapons technology or defense, and are easily captured or destroyed by enemy combat ships. Guard them wisely with military escorts.

Merchant Marine attributes are listed in Section 9.

#### 2.3.2.1 Environmental Transformation And Colonization (ETAC)

ETACs are used to terraform and colonize uninhabited planets. After use they are scrapped and used by the colony to continue the terraforming process. They have a Carry Limit (CL) of one Population Transfer Unit (PTU) and must be pre-loaded with colonists.

#### 2.3.2.2 Traders

Traders earn SATs by trading between colonies within the House or with trade partners. They must have an uncontested path back across jump lanes to a House colony in order facilitate merchant activity and earn. Systems may only have one operational trader assigned per House.

#### 2.3.2.3 Starliners & Troop Transports

Starliners are massive ships that ferry Pilgrims between existing colonies. Passengers travel in stasis to optimize space, along with their associated life support equipment, factories, and supplies to make them economically productive at the new destination. They have a Carry Limit (CL) of 100 PTU.

Troop Transports are specialized ships that taxi Space Marine divisions between solar systems, along with their required combat gear, armored vehicles, and ammunition. They have a CL of one MM.

### 2\.3.3 Squadrons

The Space Force is organized by squadrons. Each squadron is commanded by a flagship with a Command Rating (CR) that will accommodate ships with a Command Cost (CC) that sum to less than or equal to the CR. This enables players to tactically group various classes of ships to balance combat effectiveness.

Squadrons fight as a unit and die as a unit. A squadron's total AS and DS values constitute a sum of all the ships under a flagship's command (including itself).

In non-hostile systems, ships in a squadron may be reassigned to an already existing squadron if the new flagship's CR allows. Squadrons may constitute a solo flagship.

Squadrons are only commissioned in systems with a functioning shipyard.

### 2\.3.4 Fleets

Squadrons are grouped together into fleets for the purpose of traversing jump lanes. Fleets may be joined or split off (creating new fleets) for strategic purposes in any non-hostile system. There is no limit to the number of squadrons assigned to a fleet.

### 2\.3.5 Task Force

A Task Force is temporary grouping of squadrons organized for combat. After the cessation of hostilities the task force is disbanded and surviving squadrons return to their respective fleets.

## 2\.4 Special Units

### 2\.4.1 Fighter Squadrons & Carriers

Fighters are small ships commissioned in squadrons that freely patrol a system. They are based planetside.

There is no limit to the number of fighter squadrons deployed in a system.

Because of their fast lightweight nature, fighters are considered to be in a crippled combat state, but without a reduction in attack strength (AS).

Carriers transport fighter squadrons between systems. Standard carriers hold up to three; super carriers hold up to five.

### 2\.4.2 Scouts

Scouts are autonomous drones outfitted with advanced sensors that aid with electronic warfare and information gathering. They give a boost to Task Forces during combat operations.

### 2\.4.3 Raiders

The Raider is the most advanced ship in the arsenal, outfitted with cloaking technology. They are expensive but have the firepower of a Battleship and shielding of a Cruiser.

**Stealth Roll**

| Stealth Tech Level | % Chance | 1D20 Roll |
|:------------------:|:--------:|:---------:|
| 0                  | 00       | NA        |
| 1                  | 15       | 18 - 2 0  |
| 2                  | 30       | 15 - 20   |
| 3                  | 45       | 12 - 20   |
| 4                  | 60       | 8 - 20    |

Fleets containing a Raider roll a 1D20 on the table above, with the approproate Stealth tech level, for a chance of going undetected by rival forces. The number of Raiders in the fleet does not affect the roll, nor rate multiple chances.

### 2\.4.4 Starbases

Starbases are powerful orbital fortresses that facilitate planetary defense and economic development via ground weather modification and advanced telecommunications. These powerful sentinels are limited to one operational unit per solar system.

Starbases require five months (five turns) to construct require a shipyard.

Starbases boost the morale of a colony by XYZ and production by XYZ every turn. Crippled starbases operate at 50% capacity and contribute half their normal morale and SATs to the colony.

### 2.4.5 Spaceports

Spaceports require two months (two turns) to construct planetside, and are used for launching heavy-lift ships and equipment into orbit.

### 2\.4.6 Shipyards

Shipyards are gateways to the stars. They are large bases constructed in orbit and require a spaceport to build over a period of three months (three turns).

The majority of ship construction and repair will occur at these important facilities. 

Shipyards are equipped with 10 docks for construction and repair. There is no limit on the number of Shipyards orbiting a colony.

### 2\.4.7 Planetary Shields & Ground Batteries

Planetary shields and Ground Batteries are planet based assets that provide an extra layer of defense to an player's colonies.

Planetary shields are restricted to homeworlds and provide system-wide electronic jamming that disrupt hostile forces assaulting the mother-system. They also serve to protect your homeworld from orbital bombardment. They are restricted to one unit per homeworld.

Ground batteries are immobile, low-tech, land based units that have the firepower of a battleship at half the cost. They lob kinetic shells into orbit and are not upgraded by technology and research.

Ground batteries are the only units that are constructed in the span of a single turn. Colonies may build them to no limit.

### 2\.4.8 Space Marines & Armies

Space Marines are ferocious devil dogs that capture enemy planets. They deploy in division sized units and will never surrender or abandon one of their own.

Marines are dropped on enemy planets by troop transports during an invasion or blitz.

Armies garrison your colonies and eradicate invaders. Their orders are to take no prisoners and protect the colony at all cost.

Marines fight alongside the Army if garrisoned planetside.

# X\.0 Prestige

Prestige is the key to victory. The House with the highest Prestige takes the title of Emperor.

There are several paths to the throne:

1. Destroy all of your rival's assets.
2. Crush your opponent's will and force them to capitulate.
3. Set a game end year, and employ a combination of tactical prowess and subversion to outfox your opponents.
4. Focus on economic development and population growth to outperform everyone else.
5. Let your rivals destroy one another, then clean House afterwards.
6. Outlast everyone.
7. All of the above.
8. Whatever the game allows.

Prestige points are won through a combination of military victory, population growth, production, subversion, technological development, and various other factors.

Performing poorly, mismanaging your colonies, acts of sabotage, and acts of subterfuge by other Houses will lower your prestige.

To prevent an open-ended stalemate, it may be prudent to set a game ending year. The goal of EC4X is to provide enough assymetry to prevent such a condition.
**(work in progress..... need help playtesting and regression analysis)**

TODO: Provide a prestige table showing the various factors, both positive and negative.

- Completely destroy a Task Force (+)
- Force a task force to retreat (+)
- Invade or blitz a planet (++)
- Capture merchant marine vessels (+)
- Lose a planet (--)
- Lose merchant marine vessels (-)
- Get surprised by a rogue fleet (-)
- Get ambushed by a rogue fleet (-)
- Lose a Starbase (-)
- Destroy a Starbase (+)
- Establish a new colony (+)
- Max out the population of a colony (+)
- Increase a planet's class via terraforming (+)
- Excessive tax rate (-)
- Invest IU above 50% of a colony's PU (+)
- Achieve a new tech level (+)
- Sabotage an enemy Shipyard (+)
- Spy on an enemy's colony (+)
- And so on.... get creative

# XY\.0 Economics

The standard unit of account in EC4X is the Satoshi (SAT), i.e. money. The power of a House is fueled by economic might, which in turn is a function of population growth and harvested resources.

SATs settle instanteously on the interdimensional Lightning network. (All comms and data are instaneous in this manner. Don't question; it's magic).

## XY\.1 Principles

**Population Unit (PU)**: A unit of colony population that provides 1 SAT of productivity to the House.

**Population Transfer Unit (PTU)**: A representative unit of colony population and associated cost of cargo, factories, and life support equipment to colonize a planet or transfer to another colony. ETACs and starliners move PTUs between solar systems.

PTUs enables transferring Pilgrims from larger collonies to smaller collonies without a signficant loss of PU from the mother-colony. 

PU = XXX

PTU = XXXX

The assumption is that this calculation will be performed in Excel or code. 

**Gross Colony Product (GCP)**: A monetary measure of the market value of all the final goods and services produced and rendered in a turn for each of your colonies, measured in SATs.

GCP = (PU * raw_index + IU) * el_mod

**RAW INDEX Table**

| RAW       | Habitable | Desolate | Extreme |
| --------- | --------- | -------- | ------- |
| Very Poor | 60%       | 60%      | 60%     |
| Poor      | 80%       | 75%      | 70%     |
| Abundant  | 100%      | 90%      | 80%     |
| Rich      | 120%      | 105%     | 90%     |
| Very Rich | 140%      | 120%     | 100%    |

Look up the Raw Material classification of your colony's system in the RAW column, and cross index with the planet's habital conditions.

**Net Colony Value (NCV)**: The net value of taxes collected from each of you colonies.

NCV = GCP * tax_rate

**Tax Rate**: The tax rate that applies to all of your colonies. Setting the tax rate above 65% will result in a negative impact to your prestige as a ruler, and slow population growth.

**House Treasury**: The total sum of NCV collected from colonies is transfered to the House treasury at the beginning of each month (turn). Unspent SATs from each turn rollover and earn 2% interest from *the galactic banking cabal that controls the layer two Lightning channels*.

**Industrial Units (IU)**: The house may invest in the planetary industry of each colony. IUs may be placed on Small colonies (D1 class planets) or larger. IU invested above 50% of the planet's PU will be donated to the colony and increase House prestige.

## XY\.2 Population Growth

Colonists love making babies and the population growth rate under normal conditions is 2% per month (turn), up to the max allowed PU for that planet.

## XY\.3 Trade

## XX\.4 Maintenance Costs

# XYZ\.0 Research & Technology

In a standard game, all tech levels start at zero.

## XYZ\.1 Upgrades

Houses may invest SATs to upgrade technologies, which are purchased in levels. 
TODO: table with cost

Technology upgrades may be purchased in the first and sixth months of the Terran calendar, i.e. the first and sixth turns of each game year. Levels must be purchased in sequential order, and only one level per technology each upgrade cycle.

## XYZ\.2 Weapons

Uprades improve the Attack Strength (AS) and Defence Strength (DS) of combat ships by 20% for each tech level (rounded down). The ship Production Costs (PC) also increases by 20%. Note that ships are limited in weapons tech level by their rated Hull Size (HS).

## XYZ\.3 Terraforming

Terraforming improve a planet's livable conditions, and thus the population limit. There are seven tech levels that correspond directly with the planet classes: E0 -> E1 -> D0 -> D1 -> H0 -> H1 -> H2. 

A planet may not skip a class, and each step costs the upper PU bound in SATs for the desired planet class. Example: Upgrading a D1 planet to a H0 planet requires level five terraforming and 1k SATs.

ETACs set the initial livable conditions for a Level I colony. Further terraforming is completed by colonists on the surface and do not require additional ETACs.

## XYZ\.4 Economics

EL = Economic Tech Level
TODO: el_mod

## XYZ\.5 Stealth

## XYZ\.6 Sabotage & Subversionn

# 3.0 Construction

Construction and repair of House assets is accomplished planetside or in orbit, with restrictions.  

The number of turns required to newly construct an asset, unless otherwise specified, is equal to the PC times 0.5 (rounded down). Assets remain decommissioned through the activity period.

TODO: Explain construction capacity and rate

## 3.1 Planetside Construction

Ground units and fighter squadrons are produced via colony industry, distributed across the surface or in underground factories.

Ships (excluding fighter squadrons) constructed planetside incur a 100% PC increase due to the added cost of orbital launch, and require a spaceport to commission.

## 3.2 Planetside Repair

Ground units and fighter squadrons are repaired and refitted planetside.

## 3.3 Orbital Construction

Shipyard construction of a ship in orbit is the standard method of commissioning a vessel, and incurs no penalty.

## 3.4 Orbital Repair

Ship repairs require a shipyard. The cost of repair equals one quarter (25%) of the unit's PC.

Example: A player wishes to repair a crippled tech-level III Cruiser. The cost is 7 * 0.25 = 1.75 SAT.

The logistics of repairing a ship planetside and returning it to orbit make it economically infeasible. Ships may be scrapped at a colony without restriction and earn 50% of the original PC back to the House treasury.

# 4\.0 Movement

## 4\.1 Escorts

If Shipyards or Starbases are ordered to move, they must be accompanied by a fleet escort. They can not move across jump lanes unassisted.

Merchant Marine ships may join a fleet for escort.

# 5\.0 Combat

## 5\.1 Principles

### 5\.1.1 Rules of Engagement (ROE)

ROE dictates how aggressive your fleet will respond when engaging with the enemy from a scale of 0 to 10. The higher the ROE, the more aggressive your fleet will engage with enemy fleets of increasing relative strength to your own. With a low ROE, your fleet will attempt to retreat more readily when engaged in combat. A low ROE does not guarantee survival against a more powerful fleet. Once engaged, fleets have the opportunity to retreat only after the first round of combat.

| **ROE** | **ORDERS**                                             |
| ------- | ------------------------------------------------------ |
| 00      | Avoid all hostile forces. (Non-combat forces)          |
| 01      | Engage forces only if they are defenseless.            |
| 02      | Engage forces only if your advantage is 4:1 or better. |
| 03      | Engage forces only if your advantage is 3:1 or better. |
| 04      | Engage forces only if your advantage is 2:1 or better. |
| 05      | Engage forces only if your advantage is 3:2 or better. |
| 06      | Engage hostile forces of equal or inferior strength.   |
| 07      | Engage hostile forces even if outgunned 3:2.           |
| 08      | Engage hostile forces even if outgunned 2:1.           |
| 09      | Engage hostile forces even if outgunned 3:1.           |
| 10      | Engage hostile forces regardless of their size.        |

### 5\.1.2 Combat Effectiveness Rating (CER)

A modified 1d10 roll applied to a combat unit’s AS for the purposes of reducing your opponent’s forces. There are two separate CER tables, one for space combat and another for ground combat.

| **Modified 1D10 Die Roll** | **Space Combat CER**             |
| -------------------------- | -------------------------------- |
| Less than zero, 0, 1, 2    | One Quarter (0.25) (round up)    |
| 3, 4                       | One Half (0.50) (round up)       |
| 5, 6                       | Three Quarters (0.75) (round up) |
| 7, 8                       | One (1)                          |
| 9                          | One\* (1)                        |
| 9+                         | One (1)                          |

\*If the die roll is a natural nine before any required modification, then a critical hit is achieved

| **Modified 1D10 Die Roll** | **Ground Combat CER**           |
| -------------------------- | ------------------------------- |
| Less than zero, 0, 1, 2    | One Half (0.5) (round up)       |
| 3, 4, 5, 6                 | One (1)                         |
| 7, 8                       | One and a half (1.5) (round up) |
| 9 or more                  | Two (2)                         |

Critical hits do not apply to ground combat.

### 5\.1.3 Battle Stations Preparedness

A battle stations preparedness modifier is applied to a player's CER
roll at the beginning of every combat round. The fog of war lends to chaos and unpredictable human behavior under mortal stress.

| **1D6 Roll** | **Battle Stations Modifier** |
| ------------ | ---------------------------- |
| 1            | Crews are in panic mode (-2) |
| 2            | Crews are scrambling (-1)    |
| 3, 4         | Crews are at the ready (0)   |
| 5            | Crews are on point (+1)      |
| 6            | Crews are in a frenzy (+2)   |

### 5\.1.4 Combat State

Squadron units are either undamaged, crippled, or destroyed.

Attack Strength (AS) represents a unit's offensive firepower and is a mutable type.

Defense Strength (DS) represents a unit's defensive shielding and is an immutable type.

**Reduced**: Degradation of combat state.

**Undamaged**: A unit’s life support systems, hull integrity, and weapons systems are fully operational.

**Crippled**: When an undamaged unit’s DS is equaled in battle by hits, that unit’s primary defensive shielding is compromised and the unit is reduced to a crippled combat state. AS is reduced by half.

**Destroyed**: In a crippled combat state, hits equal to DS reduces a unit's state to destroyed. The unit is dead and unrecoverable.

### 5\.1.5 Cloaking

Cloaking offers an advantage to a Task Force in the initial round of space combat, both on the defensive and offensive.

When defending a solar system, a cloaked fleet is considered to be in ambush.

When attacking a solar system, a cloaked fleet is considered to be a surprise.

Both may apply at the same time if opposing fleets are simultaneously cloaked.

Roll for stealth in accordance with Section 2.4.3.  

## 5\.2 Task Force Assignment

All of a player’s fleets arriving at a star system in the same turn, and fleets and squadrons already located in said system, are joined together into a single Task Force when battle commences. Fleets are temporarily disbanded and their collective squadrons fight under the Task Force as a monolith.

Task Forces assume the highest ROE of any fleet in the force.

Fighter squadrons deploy to their player's respective Task Force as independent squadrons.

Fleets that are cloaked, and remain undetected, may continue traveling through jump lanes in a contested star system. Otherwise the fleet will join their player's respective Task Force for battle.

Starbases, Orbital Shipyards, and Merchant Marine ships are screened behind the Task Force during combat operations and do not engage.

## 5\.3 Retreat

A Task Force may retreat from combat only after the first round of combat, in accordance with their ROE, and between rounds thereafter. The ROE is fixed at the beginning of combat and through all subsequent rounds.

A retreating Task Force will fall back to their original fleet formations and flee to the closest non-hostile star system.

### 5\.3.1 Starbases

Starbases never retreat from a solar system because of their massive size. They are too slow to maneuver.

Refer to Section 5.5 for handling orphaned assets if a Starbase is abandoned by a fleeing Task Force.

### 5\.3.2 Fighter Squadrons & Merchant Marine

Orphaned fighter squadrons are scuttled if there is no carrier capacity available during a retreat.

Starliners are captured and colonists enslaved if their escort fleet was destroyed or the transports were un-escorted at the commencement of hostilities. 

Space Marines never surrender and self-detonate their troop transports.

ETACs and traders rejoin their surviving escort fleets. If the fleet was destroyed or the ships were unescorted before hostilities, they are captured as spoils of war.

Like Starbases, Orbital Shipyards are too large and complex to retreat in an expedited manner. They are rigged to self-detonate before capture.

This section is null and void if Section 5.3.1 is in effect.

## 5\.4 Space Combat

### 5.4.1 Rounds

After Task Forces are aligned for battle, combat commences in a series of rounds until one side is completely destroyed or manages a retreat.

Combat action is simultaneous; all squadrons have the opportunity to fire on enemy forces at least once, regardless of damage sustained during a round.

At the beginning of each combat round, players add up the total AS of their surviving squadrons. The total value is then modified by the following:

Players roll a die in accordance with Section 5.1.2 to determine their CER, applying all applicable modifiers.

The CER multiplied by AS equals the number of total enemy hits.

**Die Roll Modifiers**

- Battle Stations: Section 5.1.3
- Scouts: +1 max
- Cloaked Surprise: +3 (first round only)
- Cloaked Ambush: +4 (first round only)
- Opposing homeworld defended by shields: -2

The player who rolled the die will determine where hits are applied within the following **restrictions**:

1. If the number of hits equal the opposing squadron's DS, the unit is reduced.
2. Squadrons are not destroyed until all other squadrons in the Task Force are crippled.
3. Excess hits may be lost if restrictions apply.

Crippled squadrons multiply their AS by 0.5, rounded up the nearest whole number.

Destroyed squadrons are no longer a factor and the Task Force loses their associated die roll modifiers (e.g. Scouts).

In computer moderated play, the algorithm will reduce opposing squadrons with the greatest AS, within restrictions.

### 5\.4.2 Critical Hits

Critical hits are a special case. Restriction \#2 above is nullified.

Additionally, if a player takes a critical hit and is unable to reduce a unit according to restriction \#1 above, then the squadron with the lowest DS is reduced.

### 5\.4.3 End of Round

After all hits are applied and squadrons are appropriately reduced (crippled or destroyed), recalculate the totel AS of all Task Forces.

Check each Task Force's ROE on the table in Section 5.1.1 by comparing AS strengths and determine if a retreat is warrented. If more than one Task Force remains in the fight, the next round commences via the same procedure as described above. 

Otherwise proceed to End of Combat.

### 5\.4.4 End of Combat

After the last round of combat the surviving Task Forces are disbanded and surviving squadrons rejoin their assigned fleets.

Retreating Task Forces must comply with the rules in Section 5.3.

### 5\.4.5 Example Combat

TODO

## 5\.5 Starbases

### 5\.5.1 Combat

If a hostile fleet has orders to bombard, invade, or blitz a colony, a Starbase is the first line of defense after the Task Force.

Combat will proceed in a similar fashion to Section 5.4, with the following restrictions:

1. If a player rolls a critical hit against a starbase on the first try, re-roll a second time.
2. Starbases receive an extra +2 die roll modifier.

Starbases are defensive citadels that are equipped with advanced sensors and massive artificial intelligence (AI) resources. Their shields are powerful and make them a challenge to strike a critical hit.

### 5\.5.2 Abandoned Starbase

In the special circumstance that a Starbase is orphaned by a retreating Task Force, the Starbase will screen other orphans and proceed straight to combat against hostile forces in accordance with Section 5.5.1.

## 5\.6 Planetary Bombardment

## 5\.7 Planetary Invasion, Blitz, and Ground Combat

# 8\.0 Diplomacy, Sabotage & Subversionn

# 9\.0 Asset Tables

## 9\.1 Imperial Space Force (Weapons Level 0)

PC = Production Cost, MC = Maintenance Cost, AS = Attack Strength, HS = Hull Size,

DS = Defensive Strength, CC= Command Cost, CR = Command Rating, CL = Carry Limit

| Class | Name             | HS  | PC  | MC    | AS  | DS  | CC  | CR  | CL  |
|:-----:| ---------------- |:---:|:---:|:-----:|:---:|:---:|:---:|:---:|:---:|
| CT    | Corvette         | 1   | 2   | 0\.1  | 1   | 2   | 1   | 2   | NA  |
| FF    | Frigate          | 1   | 3   | 0\.2  | 2   | 3   | 2   | 3   | NA  |
| DD    | Destroyer        | 1   | 4   | 0\.3  | 3   | 4   | 2   | 4   | NA  |
| CA    | Cruiser          | 2   | 5   | 0\.4  | 4   | 5   | 3   | 6   | NA  |
| BC    | Battle Cruiser   | 2   | 6   | 0\.5  | 4   | 6   | 3   | 8   | NA  |
| BB    | Battleship       | 3   | 8   | 1\.0  | 6   | 8   | 3   | 9   | NA  |
| DN    | Dreadnought      | 3   | 10  | 1\.25 | 9   | 9   | 4   | 10  | NA  |
| CV    | Carrier          | 1   | 8   | 1\.0  | 2   | 6   | 3   | 8   | 3   |
| CX    | Super Carrier    | 2   | 10  | 1\.5  | 3   | 9   | 4   | 10  | 5   |
| FR    | Fighter Squadron | 1   | 3   | 0\.2  | 3   | 2   | NA  | NA  | NA  |
| RR    | Raider           | 2   | 25  | 0\.5  | 6   | 5   | 3   | 4   | 0   |
| SC    | Scout            | 1   | 5   | 0\.1  | 0   | 1   | 1   | NA  | NA  |
| SB    | Starbase         | 3   | 50  | 2.5   | 45  | 50  | NA  | NA  | NA  |

## 9\.2 Merchant Marine

| **Class** | **Name**        | **PC** | MC  | CL      |
|:---------:| --------------- |:------:|:---:|:-------:|
| SS        | Shipyard        | 30     | 3   | 10      |
| ET        | ETAC            | 15     | 0.5 | 1 PTU   |
| TR        | Trader          | 6      | 0.5 | NA      |
| TT        | Troop Transport | 5      | 0.5 | 1 MM    |
| SL        | Starliner       | 15     | 2.0 | 100 PTU |

## 9\.3 Planet Based Units

| **Class** | **Name**         | **PC** | MC  |
|:---------:| ---------------- |:------:|:---:|
| PY        | Spaceport        | 20     | 1.0 |
| PS        | Planetary Shield | 35     | 2.0 |
| GB        | Ground Batteries | 4      | 0.1 |
| AA        | Armies           | 2      | 0.2 |
| MM        | Space Marines    | 3      | 0.2 |

# 10\.0 Play By Excel
