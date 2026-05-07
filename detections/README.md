# 🔎 Detections & Threat Hunting

This section contains original detection engineering and threat hunting content across multiple platforms and query languages.

## Platforms
- **CrowdStrike LogScale (CQL)** → `crowdstrike-logscale-cql/`
- **Splunk (SPL)** → `splunk-spl/`
- **Microsoft Sentinel (KQL)** → `sentinel-kql/`

## Organization
Hunts are organized by MITRE ATT&CK tactic:

- authentication
- execution
- persistence
- privilege-escalation
- defense-evasion
- credential-access
- discovery
- lateral-movement
- command-and-control
- exfiltration
- impact

Each hunt folder typically includes:

- `query.*`
- `README.md` describing goal, logic, tuning, and validation.

## Notes on Data & IP
- All queries are original.
- No employer or customer data is included.
- Syntax and techniques are based on public documentation and community references.
