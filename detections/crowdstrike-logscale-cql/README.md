# CrowdStrike LogScale — CQL Detections & Hunts

This directory contains original threat-hunting and detection-engineering queries written in CrowdStrike Query Language (CQL) for Falcon LogScale.

The focus is on behavioral analytics, attacker tradecraft, and detection logic mapped to MITRE ATT&CK.

## What You’ll Find Here
- High-signal hunting queries
- Detection concepts that can be operationalized
- Baseline analytics for normal behavior
- Tuning guidance and validation approaches

## Organization

Hunts are grouped by ATT&CK tactic (authentication, persistence, lateral-movement, etc.).

Each hunt includes:
- A query file (`.cql`)
- Comments explaining logic, assumptions, tuning, and testing

## Scope & Ethics
- No employer or customer data is included
- All logic is original and based on public documentation and community references
- Content is intended for educational purposes