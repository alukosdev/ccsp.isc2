# PCI DSS

Payment Card Industry Data Security Standards

## Terminology

### Acronyms

| Acronym | Definition |
| :--- | :--- |
| AoC | Attestation of Compliance |
| ASV | Approved Scanning Number |
| DSS | Data Security Standards |
| ISA | Internal Security Assessor |
| PAN | Primary Account Number |
| PCI | Payment Card Industry |
| PFI | PCI Forensic Investigator |
| QSA | Qualified Security Assessor |
| RoC | Report of Compliance |
| SAD | Sensitive Authentication Data |
| SAQ | Self-Assessment Questionnaire |

### Definitions

#### ISA

An ISA is an individual who has earned a certificate from the PCI Security Standards Company for their sponsoring organization. This certified person has the ability to perform PCI self-assessments for their organization.

#### QSA

QSAs are the independent groups/entities which have been certified by PCI SSC for compliance confirmation in organization procedures.

#### RoC

A RoC is a form that has to be filled by *all level 1 merchants* undergoing a PCI DSS audit. The ROC form is used to verify that the merchant being audited is compliant with the PCI DSS standard.

#### SAD

Examples include CVV or PIN numbers.

#### SAQ

The PCI DSS SAQs are validation tools intended to assist merchants and service providers report the results of their PCI DSS self-assessment.

## Overview

VISA, MasterCard, and American Express established PCI DSS as a security **standard** to which all organizations or merchants that accept, transmit, or store cardholder data, regardless of size or number of transactions, **must comply.**

:::info
PCI DSS is a standard, *not* a regulation.
:::

## Components

PCI DSS is a comprehensive and intensive security standard that lists both technical and nontechnical requirements based on the number of credit card transactions for the applicable entities.

### Merchant Levels

| Level | Description |
| :--- | :--- |
| 1 | Any merchant-regardless of acceptance channel-processing more than 6 million transactions per year. Any merchant that the credit card issuer, at its sole discretion, determines should meet the Level 1 requirements to minimize risk to the credit card issuer's system. |
| 2 | Any merchant-regardless of acceptance channel-processing 1-6 million credit card transactions per year. |
| 3 | Any merchant processing 20,000 to 1 million credit card e-commerce transactions per year. |
| 4 | Any merchant processing fewer than 20,000 credit card e-commerce transactions per year and all other merchants-regardless of acceptance channel-processing up to 1 million credit card transactions per year. |

:::info
Merchants at different tiers are required to have more or fewer audits in the same time frame as merchants in other tiers, depending on the tier. Businesses at level 1 are required to undergo a **yearly PCI audit** conducted by a QSA.
:::

### Merchant Requirements

All merchants, regardless of level and relevant service providers, are required to comply with the following **12 domains/requirements:**

- Install and maintain a firewall configuration to protect cardholder data
- Avoid using vendor-supplied defaults for system passwords and other security parameters.
- Protect stored cardholder data.
- Encrypt transmission of cardholder data across open, public networks.
- User and regularly update antivirus software.
- Develop and maintain secure systems and applications.
- Restrict access to cardholder data by business need-to-know.
- Assign a unique ID to each person with computer access.
- Restrict physical access to cardholder data.
- Track and monitor all access to network resources and cardholder data.
- Regularly test security systems and processes.
- Maintain a policy that addresses information security.

The 12 requirements list more than 200 controls that specify required and minimum security requirements for the merchants and service providers to meet their compliance obligations.

