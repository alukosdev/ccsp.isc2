# Cloud Infrastructure Design

## Overview

Location is the major and primary concern when building a data center. It's important to understand the jurisdiction where the datacenter will be located. This means understanding the local laws and regulations under that jurisdiction. In addition, the physical location of the datacenter will also drive requirements for protecting data during threats such as natural disasters.

The industry standard for uptime in cloud service provision is "five nines," which means 99.999% uptime. This equates to less than six minutes per year.

:::info
A customer's ability to connect to a datacenter may be limited by a failure within the own customer's ISP. This would be a lack of availability from the customer's perspective but not a lack of uptime on the part of the provider.
:::

## Terminology

#### Chicken Coop

A design methodology in which a datacenter arranges racks within long rectangles with a long side facing the wind to provide natural cooling.

#### Redundancy

Deploying duplicate devices that can take over active operation if the primary device fails.

#### Resiliency

The ability to restore normal operations after a disruptive event. Redundancy is the foundation of resiliency.

## Design Principles

### Hardening

### Encryption

### Layered Defenses

Also referred to as "defense-in-depth", this is the practice of having multiple overlapping means of securing the environment with a variety of methods. These should include a blend of administrative, logical, technical, and physical controls.