## Overview

Security hardening: Strengthening a system to reduce its vulnerabilty and attack surface.
Attack surface: All the potential vulnerabilities.

Conducted on:

- Hardware
- OS
- Applications
- Networks
- Databases
- Physical space

Examples are:

- Patches
- Config changes
- Disabling used services
- Reducing permissions

Regular penetration testing also helps

## OS hardening

Regular interval tasks:

- Patch updates
- Backups
- Wiping old hardware
- Removing unused software

One-off:

- Secure encryption
- Strong password policy

### Baseline configuration

> A baseline configuration is a documented set of specifications within a system that is used as a basis for future builds, releases, and updates.

## Preventing brute force attacks

- Salting & hashing
- MFA / 2FA
- Captcha
- Strong password policies

## Network hardening

Regular interval tasks:

- Firewall rules maintenance
- Network log analysis
- Patch updates
- Server backups

One-off:

- Port filtering on firewalls
- Network access privileges
- Using isolated subnets for departments / security zones
- Using modern encryption standards

### Hardware

- Intrusion detection system: Monitors traffic, alerts to possible intrusion.
- Intrusion prevention system: Monitors traffic, actively stops the activity.

## Cloud hardening

Considerations:

- Identity access management (IAM): managing digital identities / authorisations.
- Configuration
- Attack surface
- Zero-day attacks (usually patched quicker!)
- Visibility & tracking
- Hypervisors
  - Type 1 runs on host computer hardware, usually used by cloud service providers.
  - Type 2 runs on host computer software.
