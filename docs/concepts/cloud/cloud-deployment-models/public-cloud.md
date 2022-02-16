# Public Cloud

## Overview

> **NIST SP 800-145**
>
> The cloud infrastructure is provisioned for **open use** by the general public. It may be owned, managed, and operated **by a business, academic, or government organization, or some combination of them**. It exists **on the premises of the cloud provider.**

The public cloud is what we typically think of when discussing cloud providers. The resources \(hardware, software, facilities, and staff\) are owned and operated by a vendor and sold, leased, or rented to anyone \(offered to the public-hence the name\).

Examples of public cloud vendors include Rackspace, Microsoft Azure, and Amazon Web Services \(AWS\).

## Risks

#### Multitenant Environments

- Conflict of Interest
- Escalation of Privilege
- Information Bleed
- Legal Activity

#### Vendor Lock-In

Vendor lock-in occurs when the organization creates a dependency on the provider.

- Limitations to moving \(bandwidth from old provider or otherwise\)
- Unfavorable contracts
- Using proprietary data formats
- Regulatory constraints \(where other providers may not be able to meet needs\)

:::info
While there are several ways to avoid vendor lock-in, the best way is through favorable contract language. To avoid lock-in, the organization has to think in terms of *portability.*
:::

#### Vendor Lock-Out

When the cloud provider goes out of business, is acquired, or ceases operation for any reason.

To avoid lock-out, the organization should consider the provider's:

- Longevity
- Core Competency
- Jurisdictional Suitability
- Supply Chain Dependencies
- Legislative Environment

## Threats

- Loss of Policy Control
- Loss of Physical Control
- Lack of Audit Access
- Rogue Administrator
- Escalation of Privilege
- Contractual Failure

:::info
Threats impacting the private model also affect the public model:

- Malware
- Internal Threats
- External Attackers
- Man-in-the-Middle Attacks
- Social Engineering
- Theft/Loss of Devices
- Regulatory Violations
- Natural Disasters
:::

:::info
The terms "public" and "private" can be confusing, because we might think of them in the context of who is offering them instead of who is using them. Remember: A public cloud is owned by a specific company and is offered to anyone who contracts its provided services, whereas a private cloud is owned by a specific organization but is only available to users authorized by that organization.
:::