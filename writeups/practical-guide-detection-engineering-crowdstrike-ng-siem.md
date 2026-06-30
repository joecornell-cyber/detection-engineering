# A Practical Guide to Detection Engineering in CrowdStrike NG-SIEM

**Published:** June 17, 2026  
**Platform:** Medium  
**Author:** Joseph Cornell  
**Article:** [A Practical Guide to Detection Engineering in CrowdStrike NG-SIEM](https://medium.com/@joe88cornell/a-practical-guide-to-detection-engineering-in-crowdstrike-ng-siem-25931f1a0120)

## Overview

This article introduces practical detection engineering concepts using CrowdStrike NG-SIEM and CrowdStrike Query Language.

The writeup covers how analysts can move beyond vendor provided detections and begin building custom detection logic that helps close visibility gaps in their environment.

## Topics Covered

- What CrowdStrike NG-SIEM is
- How CrowdStrike Query Language works
- How to think like a detection engineer
- Mapping detections to MITRE ATT&CK
- Validating telemetry before building detections
- Building practical CQL detections
- Common CQL functions used in detection engineering
- Learning resources for CrowdStrike LogScale and NG-SIEM

## Example Detection Concepts

The article walks through practical detection examples, including:

| Detection Concept | Platform | Focus Area |
|---|---|---|
| File Write by Living off the Land Binary | CrowdStrike Falcon LogScale | LOLBin abuse, payload staging, suspicious file writes |
| Office Process Writing Executable or Script Files | CrowdStrike Falcon LogScale | Initial access, macro abuse, suspicious document behavior |

## Related Repository Content

The examples in the article align with detection logic in this repository, especially the CrowdStrike LogScale CQL detections.

Related detection folders:

- [`../detections/crowdstrike-logscale-cql/`](../detections/crowdstrike-logscale-cql/)
- [`../detections/splunk-spl/`](../detections/splunk-spl/)
- [`../detections/sentinel-kql/`](../detections/sentinel-kql/)

Related detection files may include:

- [`../detections/crowdstrike-logscale-cql/file-write-by-lolbin.lql`](../detections/crowdstrike-logscale-cql/file-write-by-lolbin.lql)
- [`../detections/crowdstrike-logscale-cql/office-process-writing-executable.lql`](../detections/crowdstrike-logscale-cql/office-process-writing-executable.lql)
- [`../detections/splunk-spl/file-write-by-lolbin.spl`](../detections/splunk-spl/file-write-by-lolbin.spl)
- [`../detections/splunk-spl/office-process-writing-executable.spl`](../detections/splunk-spl/office-process-writing-executable.spl)

## Key Takeaways

- Detection engineering should start with attacker behavior, not query syntax.
- MITRE ATT&CK can help map detection coverage and identify monitoring gaps.
- Custom detections help organizations address risks that vendor provided content may miss.
- Telemetry validation is critical before writing or deploying detection logic.
- CQL functions such as `groupBy()`, `table()`, `eval()`, `regex()`, `format()`, `in()`, `match()`, and `case()` are useful building blocks for detection engineering.

## Why This Writeup Matters

This article supports the broader goal of this repository: building practical, portable detection engineering content across multiple platforms.

The same detection ideas can often be adapted across:

- CrowdStrike Falcon LogScale / NG-SIEM using CQL
- Splunk using SPL
- Microsoft Sentinel using KQL

## External Link

Read the full article on Medium:

[A Practical Guide to Detection Engineering in CrowdStrike NG-SIEM](https://medium.com/@joe88cornell/a-practical-guide-to-detection-engineering-in-crowdstrike-ng-siem-25931f1a0120)