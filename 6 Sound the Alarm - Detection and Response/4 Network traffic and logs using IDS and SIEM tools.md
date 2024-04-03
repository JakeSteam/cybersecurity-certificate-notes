## Logs

Types:

- Network: Proxies, firewalls, etc
- System: OS
- Application: Specific programs
- Security: Security tools like IDS / IPS
- Authentication logs: Login attempts

## Detection systems

- HIDS: Host-based IDS, installed on a host / endpoint.
- NIDS: Network-based IDS, installed on network tech, monitors all traffic going through.

### Techniques

- Signature analysis: Low false positives, easy to evade.
- Anomaly-based analysis: Can detect new threats, has false positives.

### Signatures

Signatures specify detection rule, typically contain 3 things:

- Action: Alert / pass / reject (usually)
- Header: Src / dst IP address / ports / protocols
- Rule options: Additional options, e.g. filtering out noisy service

## Suricata

IDS, IPS, and NSM (network security monitoring).

Log files:

- `eve.json`: Standard log file, in JSON format.
- `fast.log`: Basic logging, shouldn't really be used.
