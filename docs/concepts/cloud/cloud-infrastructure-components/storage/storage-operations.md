# Storage Operations

## Tightly Coupled

All the storage devices are directly connected to a shared physical backplane, thus connecting all of them directly. Each component of the cluster is aware of the others and subscribes to the same policies and rulesets.

- Proprietary
- Shared physical backplane and network fixes the maximum size of the cluster
- Delivers a high-performance interconnect between servers
  - Allows for load-balanced performance
  - Allows for maximum scalability as the cluster grows \(array controllers, I/O ports, and capacity can be added into the cluster as required to service the load\)
- Fast, but loses flexibility\*

:::info
A tightly coupled cluster is usually confined to more restrictive design parameters, often because the devices might need to be from the same vendor \(proprietary\) in order to function properly. Although this may be a limiting factor, a tightly coupled architecture will also enhance performance as it scales.
:::

## Loosely Coupled

A loosely coupled cluster will allow for greater flexibility. Each node of the cluster is independent of the others, and new nodes can be added for any purpose or use as needed. They are only logically connected and don't share the same proximate physical framework, so they are only distantly physically connected through communication media.

A loose cluster offers performance, I/O, and storage capacity **within the same node**. As a result, performance scales with capacity and vice versa.

- Cost-effective
- Can start small and grow as demand requires
- Performance, I/O, and storage capacity are all contained within the same node
  - This allows performance to scale with capacity
- Scalability is limited by the performance of the interconnect

In a loosely coupled storage cluster, each node acts as an independent data store that can be added or removed from the cluster without affecting other nodes. This, however, means that the overall cluster’s **performance/capacity depends on each node’s own maximum performance/capacity**. Because each node in a loosely coupled architecture has its own limitations, the number of nodes will not affect overall performance.

- Distributed.
- Built for servers in multiple locations.