# Splunk — SPL Detections & Hunts

Detection engineering and threat hunting content written in Splunk Search Processing Language (SPL).

These detections are designed to turn raw endpoint and authentication telemetry into actionable security signals. The goal is to provide practical, readable, and tunable SPL content that can be adapted for real world defensive operations.

## What You’ll Find Here

- Behavioral detections and anomaly analytics
- Authentication abuse and failed-logon hunting
- LOLBin and living-off-the-land activity
- Suspicious file-write and process activity
- Browser extension inventory and watchlist hunting
- Baselines for normal host, user, and process behavior

## Current SPL Detections

| Detection | Category | Description |
|---|---|---|
| `browser-extension-hunt-host.spl` | Browser Extensions | Hunts installed browser extensions on a specific endpoint. |
| `browser-extension-watchlist-widespread.spl` | Browser Extensions | Identifies watched browser extensions across multiple hosts. |
| `failed-logon-bruteforce.spl` | Authentication | Detects repeated failed logon activity that may indicate brute force behavior. |
| `failed-logon-geo-anomaly.spl` | Authentication | Hunts failed logons from unusual or unexpected geographic locations. |
| `failed-logon-password-spray.spl` | Authentication | Detects password spraying patterns across multiple users. |
| `failed-logon-targeted-users.spl` | Authentication | Identifies repeated failed logons against high-value or targeted users. |
| `failed-logon-threat-intel-sources.spl` | Authentication / Threat Intel | Correlates failed logon activity with known or suspicious source indicators. |
| `file-write-burst-activity.spl` | File Activity | Detects bursts of file-write activity that may indicate staging, dumping, or automation. |
| `file-write-by-lolbin.spl` | LOLBin Activity | Hunts file writes performed by living-off-the-land binaries. |
| `file-write-executable-in-user-profile.spl` | File Activity | Detects executable content written into user profile paths. |
| `file-write-process-dump.spl` | Credential Access | Hunts for suspicious process dump file creation. |
| `file-write-registry-hive-export.spl` | Credential Access | Detects file writes associated with registry hive export activity. |
| `file-write-startup-folder.spl` | Persistence | Detects file writes to Windows startup folder locations. |
| `file-write-system32-dll.spl` | Defense Evasion / Persistence | Hunts DLL writes into System32 or other sensitive system paths. |
| `office-process-writing-executable.spl` | Initial Access / Execution | Detects Office processes writing executable content to disk. |

## Organization

Each hunt is intended to include:

- Query logic
- ATT&CK mapping
- Required data sources and fields
- Tuning guidance
- False positive considerations
- Testing and validation notes

## Data Source Assumptions

Most detections in this folder are currently written with CrowdStrike EDR style telemetry in mind and may reference fields such as:

- `event_simpleName`
- `ComputerName`
- `UserName`
- `FileName`
- `FilePath`
- `CommandLine`
- `ParentBaseFileName`
- `RemoteAddressIP4`

Field names may need to be adjusted depending on your Splunk data model, sourcetype, endpoint telemetry provider, or normalization strategy.

## Usage Notes

These detections are intended for lab, research, and educational use. Before deploying into production, validate each query against your environment, tune thresholds, and add known-good exclusions where appropriate.

Recommended tuning steps:

1. Confirm the required fields exist in your Splunk environment.
2. Test the query over a short time window.
3. Review results for common administrative or software management activity.
4. Add allowlists or exclusions for known good tools, users, hosts, and paths.
5. Expand the time range and validate detection quality before alerting.

## Project Goal

This folder is part of a broader detection engineering repository focused on building portable detection logic across multiple platforms, including Splunk SPL, CrowdStrike LogScale CQL, and Microsoft Sentinel KQL.