# Storage Networks

## Terminology

### Definitions

#### Challenge Handshake Authentication Protocol \(CHAP\)

CHAP is used to periodically verify the identity of the client using a three-way handshake. This is done upon initial link establishment and may be repeated any time after the link has been established.

#### Initiators

The *consumer* of storage, typically a server with an adapter card in it called a HBA. The initiator commences a connection over the fabric to one or more ports on your storage system, which are called target ports.

#### Kerberos

Kerberos is a network authentication protocol that uses secret-key \(symmetric\) cryptography.

#### Network-Attached Storage \(NAS\)

A NAS is a network file server with a drive or group of drives, portions of which are assigned to users on that network. The user will see a NAS as a file server and can share files to it. NAS commonly uses TCP/IP.

#### Secure Remote Password \(SRP\)

SRP is a secure password-based authentication and key-exchange protocol. SRP uses a strong secret to enable parties to security communicate.

#### Storage Area Network \(SAN\)

A SAN is a group of devices connected to the network that provide storage space to users. Typically, the storage apportioned to the user is mounted to that user's machine, like an empty drive. The user can then format and implement a filesystem in that space according to their own preference. SANs usually use iSCSI or Fibre Channel protocols.

#### Simple Public-Key Mechanism \(SPKM\)

SPKM provides authentication, key establishment, data integrity, and data confidentiality in an online distributed application requirement.

SPKM is good for any application that uses GSSAPI calls.

The use of SPKM requires a PKI, which generates digital signatures for ensuring nonrepudiation.

#### Targets

The ports on your storage system that deliver storage volumes \(called target devices or LUNs\) to the initiators.

## Protocols

### iSCSI

iSCSI is an IP-based \(layer 3\) storage networking standard for linking data storage facilities. It provides *block-level* access to storage devices by carrying SCSI commands over a TCP/IP network. Because iSCSI is a layer 3 solution, it will permit routing of the traffic.

#### Best Practices

- Storage network traffic should not be shared with other network traffic \(management, fault tolerance, or vMotion\). A dedicated, local LAN or private VLAN should be provisioned to segregate iSCSI traffic.
- iSCSI does not handle overprovisioning of resources in a graceful manner. This practice should be avoided.
- iSCSI is unencrypted. Encryption must be added separately through IPsec \(tunneling\) and IKE \(security\).
- iSCSI supports authentication from the following protocols:
  - Kerberos
  - SRP
  - SPKM
  - CHAP