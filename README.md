# Detection Engineering

A collection of detection engineering content, SIEM detections, threat hunting queries, security labs, and hands-on defensive security research focused on modern enterprise environments.

This repository is focused on building practical, reusable detection engineering content across multiple platforms, including CrowdStrike Falcon LogScale / NG-SIEM, Splunk, and Microsoft Sentinel.

## Repository Contents

This repository contains:

- SIEM detections and threat hunting queries
- Detection engineering research
- CrowdStrike LogScale / NG-SIEM CQL detections
- Splunk SPL detection ports
- Microsoft Sentinel KQL content
- Security lab documentation
- Active Directory, cloud, and Wazuh lab notes
- Technical writeups related to detection engineering and defensive security

---

## Repository Structure

```text
detections/
├── crowdstrike-logscale-cql/
├── sentinel-kql/
└── splunk-spl/

labs/
├── active-directory/
├── cloud/
└── wazuh/

writeups/
├── README.md
└── practical-guide-detection-engineering-crowdstrike-ng-siem.md
```

---

## Detection Engineering

The `detections/` directory contains threat hunting and detection engineering content for multiple SIEM and security platforms.

### Platforms

- CrowdStrike Falcon LogScale / NG-SIEM using CQL
- Splunk using SPL
- Microsoft Sentinel using KQL

### Detection Categories

Examples include:

- Failed logon anomaly detection
- Password spray detection
- Brute force activity
- Rare user logons
- Suspicious file write activity
- LOLBin and living-off-the-land activity
- Office process writing executable content
- Registry hive export detection
- Process dump file creation
- Browser extension monitoring
- Scheduled task monitoring
- Threat intelligence enrichment
- Beaconing detection research

---

## Splunk SPL Detections

The `detections/splunk-spl/` directory contains Splunk SPL versions of detection logic from this project.

Current SPL coverage includes authentication, browser extension hunting, LOLBin activity, suspicious file writes, persistence-related file activity, and credential access-related behaviors.

Example SPL detections include:

- `failed-logon-password-spray.spl`
- `failed-logon-bruteforce.spl`
- `failed-logon-geo-anomaly.spl`
- `failed-logon-targeted-users.spl`
- `file-write-by-lolbin.spl`
- `file-write-process-dump.spl`
- `file-write-registry-hive-export.spl`
- `office-process-writing-executable.spl`
- `browser-extension-hunt-host.spl`

---

## Labs

The `labs/` directory contains hands on cybersecurity lab environments and documentation.

### Active Directory Lab

Active Directory focused lab notes for identity, authentication, Windows security, and enterprise attack-path research.

### Cloud Security Lab

Cloud focused security research environment for:

- Identity monitoring
- Cloud attack simulations
- Logging and telemetry analysis
- Security configuration testing

### Wazuh SIEM Lab

Custom Wazuh deployment used for:

- Endpoint monitoring
- Log ingestion
- Detection engineering
- Alert validation

---

## Writeups

The `writeups/` directory contains published articles, companion notes, and technical documentation related to detection engineering and defensive security research.

Current writeups include:

- [A Practical Guide to Detection Engineering in CrowdStrike NG-SIEM](./writeups/practical-guide-detection-engineering-crowdstrike-ng-siem.md)

Topics covered include:

- CrowdStrike NG-SIEM
- CrowdStrike Query Language
- Detection engineering methodology
- MITRE ATT&CK mapping
- Threat hunting workflows
- Practical detection examples
- SIEM query development

---

## Goals of This Repository

This repository is used to:

- Improve detection engineering skills
- Build reusable defensive security content
- Document hands on security research
- Practice SIEM and telemetry analysis
- Explore attacker behavior and detection opportunities
- Develop repeatable security workflows
- Map detection ideas across multiple SIEM platforms
- Share practical examples for analysts, threat hunters, and detection engineers

---

## Status

This repository is actively maintained and continuously updated with:

- New detections
- Splunk SPL ports
- CrowdStrike LogScale / NG-SIEM CQL detections
- Microsoft Sentinel KQL content
- Lab improvements
- Threat hunting queries
- Writeups and research notes
- Detection tuning ideas

Some content may be incomplete or experimental while under development.

---

## Disclaimer

This repository is intended for educational and research purposes only.

All testing is performed in authorized lab environments.