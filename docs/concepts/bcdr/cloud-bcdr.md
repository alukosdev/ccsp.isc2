# Cloud BCDR

## Cloud vs. Traditional

Cloud backup provides many advantages over tape-based backup:

- *Convenience.* As long as you have an Internet connection, data can be backed up as it is saved to disk. Data can be synced across multiple computers so that the data is not only backed up, but it is also instantly shared with other users.
- *Safety.* Local disasters such as fire or flood are no longer concerns.
- *Ease of Recovery.* Online backup systems can be configured to maintain multiple versions of a file. While this may be available with local backup, the ease with which different versions of a file can be restored are superior in the cloud.
- *Ease of Access.* Data can be accessed from anywhere there is an Internet connection.
- *Affordability.* Capital expenditure is reduced as tape drives, libraries, servers, or other hardware is no longer necessary to perform the backup.

Advantages to using a cloud BC/DR include:

- Rapid elasticity
- Broad network connectivity
- On-demand self-service
- Experienced and capable staff
- Measured service

## Backup Methodologies

### Private Architecture &gt; CSP as BC/DR

The organization maintains its own on-premise IT infrastructure and uses a CSP for BC/DR purposes.

### Cloud Operations &gt; Primary CSP as BC/DR

The organization's infrastructure is already hosted in the cloud and they choose to use that same CSP for BC/DR purposes.

In some cases, cloud providers may offer a backup solution as a feature of their service and would ideally be located at another datacenter owned by the provider in case of a local disaster-level event.

### Cloud Operations &gt; Third-Party CSP as BC/DR

Regular operations are hosted by the cloud provider, but contingency operations require failover to another cloud provider.

## Shared Responsibilities

### Declaration

The cloud customer and provider must decide, prior to the contingency, who specifically will be authorized to make decisions for disaster declaration and the explicit process for communicating when it has been made.

### Testing

BC/DR testing will have to be coordinated with the cloud provider. This should be planned well in advance of the scheduled testing.

## Similarities to Traditional BC/DR

### Traditional Hot Site

This would equate to an *active-passive* cloud model.

- In an active-passive deployment, resources are held in a secondary datacenter in standby mode. This would be similar to a hot site in the traditional DR methodology.