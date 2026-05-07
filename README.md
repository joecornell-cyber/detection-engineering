# Detection Engineering

A collection of detection engineering content, security labs, threat hunting queries, and hands-on defensive security research focused on modern enterprise environments.

This repository contains:
- SIEM detections and threat hunting queries
- Detection engineering research
- Security lab documentation
- Active Directory and cloud security exercises
- Wazuh and endpoint monitoring labs
- Offensive security writeups from a defensive perspective

---

# Repository Structure

```text
detections/
├── crowdstrike-logscale-cql/
├── sentinel-kql/
└── splunk-spl/

labs/
├── cloud/
└── wazuh/

writeups/
├── oscp/
└── pjpt/
```

---

# Detection Engineering

The `detections/` directory contains threat hunting and detection engineering content for multiple SIEM and security platforms.

## Platforms

- CrowdStrike LogScale (LQL/CQL)
- Microsoft Sentinel (KQL)
- Splunk SPL

## Detection Categories

Examples include:
- Failed logon anomaly detection
- Password spray detection
- Brute force activity
- Rare user logons
- Suspicious file write activity
- Office spawning executables
- Registry hive exports
- Beaconing detection research
- Browser extension monitoring
- Scheduled task monitoring
- Threat intelligence enrichment

---

# Labs

The `labs/` directory contains hands-on cybersecurity lab environments and documentation.

## Current Labs

### Cloud Security Lab (In progress)
Cloud-focused security research environment for:
- Identity monitoring
- Cloud attack simulations
- Logging and telemetry analysis
- Security configuration testing

### Wazuh SIEM Lab (Still Documenting)
Custom Wazuh deployment used for:
- Endpoint monitoring
- Log ingestion
- Detection engineering
- Alert validation

---

# Writeups

The `writeups/` directory contains technical notes, walkthroughs, and learning documentation related to:
- OSCP preparation
- PJPT preparation
- Hack The Box style environments
- Enumeration methodology
- Privilege escalation research
- Web application testing

---

# Goals of This Repository

This repository is used to:
- Improve detection engineering skills
- Document hands-on security research
- Build reusable defensive security content
- Practice SIEM and telemetry analysis
- Explore attacker behavior and detection opportunities
- Develop repeatable security workflows

---

# Status

This repository is actively maintained and continuously updated with:
- New detections
- Lab improvements
- Threat hunting queries
- Writeups and research notes
- Detection tuning ideas

Some content may be incomplete or experimental while under development.

---

# Disclaimer

This repository is intended for educational and research purposes only.

All testing is performed in authorized lab environments.
