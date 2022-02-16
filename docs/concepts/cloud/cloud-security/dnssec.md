# DNSSEC

## Terminology

### Acronyms

| Acronym | Definition |
| :--- | :--- |
| KSK | Key Signing Key |
| ZSK | Zone Signing Key |

## Overview

DNSSEC is a suite of extensions that adds security to the DNS protocol by enabling DNS response validation using a process called zone signing.

Specifically, DNSSEC provides:

- Origin authority
- Data integrity
- Authenticated denial of existence

With DNSSEC, the DNS protocol is much less susceptible to certain types of attacks:

- Cache poisoning/spoofing
- Pharming
- MITM

DNSSEC uses digital signatures embedded in the data. The DNSSEC digital signature verifies you are communicating with the site you intended to visit \(authenticity\). DNSSEC puts additional records in DNS alongside existing records. The new record types, such as RRSIG and DNSKEY, can be accessed the same way as common records such as A, CNAME, and MX. A public and private key will exist for each zone. When a request is made, the request include information signed with a private key; the recipient then unlocks it with the public key.

It's important to note that DNSSEC does *not* provide encryption.

DNSSEC does *not* protect against:
