# MFA

## Terminology

### Acronyms

| Acronym | Definition |
| :--- | :--- |
| MFA | Multifactor Authentication |
| TOTP | Time-Based One Time Passwords |

### Definitions

#### Step-Up Authentication

Step-up authentication is an additional factor or procedure that validates a user's identity by using the following means:

- Challenge questions
- Out-of-band authentication \(phone call or SMS\)
- Dynamic knowledge-based authentication \(questions unique to the end user\)

## Overview

Authentication requires a match against a template or a known quantity. Therefore, variables \(such as variable keystrokes\) aren't useful for authentication.

Multifactor authentication requires at least two of the following:

- *Type 1:* Something you know
- *Type 2:* Something you have
- *Type 3:* Something you are

In some cases, a fourth factor is mentioned:

- *Type 4:* Something you do \(linked to something you are\)
  - Physiological and behavioral, such as how you write or type.

This field is constantly evolving, and additional considerations include:

- TOTP
- Somewhere you are \(location based\)