# Network Models

![Network Models](/img/network-models.png)

## Traditional Networking Model

The traditional model is a **layered** approach with physical switches at the top layer and logical separation at the hypervisor level.

:::info
This model allows for the use of traditional network security tools. There may be some limitations on the visibility of network segments between VMs.
:::

## Converged Networking Model

The converged model is optimized for cloud deployments and utilizes **standard** perimeter protection measures. The underlying storage and IP networks are converged \(across the same infrastructure, as opposed to having a separate LAN and SAN\) to maximize the benefits for a cloud workload.

You can think of a converged network model as being a super network, one that is capable of carrying a combination of data, voice, and video traffic across a single network that is optimized for performance.

:::info
This method facilitates the use of virtualized security appliances for network protection.
:::