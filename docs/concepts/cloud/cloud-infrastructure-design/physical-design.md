# Physical Design

## Terminology

### Definitions

#### Cable Mining

The process of reviewing, identifying, and removing cables that are no longer being used.

#### Mean Time Before Failure \(MTBF\)

A measure of component reliability. It provides the average time between system or component failures.

#### Mean Time to Repair \(MTTR\)

Represents the average time required to repair a device that has failed or requires repair.

#### Mean Time to Switchover \(MTTS\)

The average time to switch over from a service failure to a replicated failover instance \(backup\).

#### Plenum

In building construction, a plenum is a separate space provided for air circulation for heating, ventilation, and air-conditioning \(sometimes referred to as HVAC\) and typically provided in the space between the structural ceiling and a drop-down ceiling.

:::info
Cold air is usually circulated through plenums.
:::

## Overview

The basic idea of physical design is that it communicates decisions about the hardware used to deliver a system. The following is true about a physical network design:

- It is created from a logical design.
- It often expands elements found in a logical design.

For instance, in terms of networking, a WAN connection on a logical design diagram can be shown as a line between two buildings. When transformed into a physical design, that single line can expand into the connection, routers, and other equipment at each end of the connection. The actual connection media might be shown on a physical design, along with manufacturers and other qualities of the network implementation.

Four items that would be considered in datacenter design:

- MTBF
- MTTR
- **Automating** service enablement
- Consolidating monitoring capabilities

## Facilities and Redundancy

The following factors should be taken into consideration when designing a datacenter:

- Regulatory issues
- Geographic location
- Redundancy issues

### Geography

#### Rural Design

- Availability of emergency services is a concern.

#### Urban Design

- Municipal codes can restrict building design.

### Redundancy

#### Power Redundancy

- Power Provider Redundancy
- Power Line Redundancy
- Power Conditioning and Distribution Redundancy

#### Communications Redundancy

#### Personnel Redundancy

- Cross-Training
- Water
- Egress
- Lighting

#### Security Redundancy

- Perimeter defenses should use layered approach
- Vehicular approach/access, to include driveways that wind and curve and/or include speed bumps as well as bollards
- Guest/visitor access through a controlled entry point
- Proper placement of hazardous or vital resources
- Interior physical access controls
- Specific physical protections for highly sensitive assets
- Fire detection and suppression systems
- Sufficient power for all these functions

#### Holistic Redundancy

[Uptime Institute](../../../standards/data-center-design/uptime-institute.md)

#### External Redundancy

- Power feeds/lines
- Power substations
- Generators
- Generator fuel tanks
- Network circuits
- Building access points
- Cooling infrastructure

#### Internal Redundancy

- Power distribution units \(PDUs\)
- Power feeds to rack
- Cooling units
- Networking
- Storage units
- Physical access points

## Efficiency

A minimum effective \(clear\) height of 24 inches should be provided for raised floor installations. Additional clearance can help achieve a more uniform pressure distribution in some cases, but is not necessary.

The power requirements for cooling a datacenter depend on the amount of heat being removed \(not generated\) and the temperature delta between the data center and the outside air.

- Temperature: 64.4 to 80.6 F \(18 to 27 C\)
- Humidity: 40%-60%
- Dew point: 41.9 to 59 F \(5.5 to 15 C\)

## Safety

### Fire Suppression

#### FM-200

FM-200 is used as a replacement for older Halon systems specifically because it \(unlike Halon\) does not deplete the ozone layer. It is discharged into the room within 10 seconds and suppresses fire immediately.

- Odorless
- Colorless
- Liquefied compressed gas \(at room temperature\)
- It is stored as a liquid and dispensed in to the hazard as a colorless, electrically non-conductive vapor that is clear and does not obscure vision.
- Classified as a "clean agent" which means that it is safe to use within occupied spaces. It is nontoxic at levels used for fire suppression.
- Does not leave a residue after discharge.
- Does not deplete the ozone and has a minimal impact on the environment relative to the impact a catastrophic fire may have.

#### Halon

It is considered a good practice to avoid all unnecessary exposure to Halon.

- Effective gaseous fire suppression agent.
- It depletes the ozone and is harmful to the environment.

### Fire/Smoke Detection

Codes require detectors under the floor or above the ceiling where HVAC piping, electrical feeders, or IT cables are placed within these plenum spaces.

#### Spot-type Detectors

- *Ionization-based*. Uses a small amount of radioactive material.
- *Photoelectric*. Uses a light source and a photosensitive sensor.

#### Aspirating/Air Sampling Smoke Detectors \(ASSD\)