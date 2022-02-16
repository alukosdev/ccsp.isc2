# Logical Design

## Overview

The following is true about the logical design for a network:

- It lacks specific details such as technologies and standards while focusing on the needs at a general level.
- It communicates with abstract concepts, such as a network, router, or workstation, without specifying concrete details.

Abstractions for complex systems, such as network designs, are important because they simplify the problem space so humans can manage it \(such as a WAN diagram\).

Logical designs are often described using terms from the customer's *business* vocabulary.

:::info
An important aspect of a logical network design is that it is part of the requirements set for a solution to a customer problem.
:::

Virtualization will leverage a hypervisor to assist with logical separation. A number of items should be considered in the logical design. These include:

- *Communications access.* What is allowed and what is not allowed?
- *Secure communications across the management plane.*
- *Secure storage.*
- *Disaster recovery.*