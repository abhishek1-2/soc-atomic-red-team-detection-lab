# T1082 — System Information Discovery

## Overview

This investigation simulates **MITRE ATT&CK T1082 — System Information Discovery**
using Atomic Red Team and investigates the resulting Windows telemetry in Splunk.

The objective was to understand how a discovery technique appears in endpoint
telemetry and how process relationships can be reconstructed during a SOC investigation.

---

## Lab Environment

- **Target:** Windows 11 VM
- **Hostname:** `Windows_for_soc`
- **SIEM:** Splunk Enterprise
- **Telemetry:** Sysmon
- **Adversary Simulation:** Atomic Red Team

---

## Technique

**MITRE ATT&CK:** T1082 — System Information Discovery

System Information Discovery allows an attacker to gather information about
the operating system and host after obtaining execution on a machine.

---

## Atomic Red Team Test

**Atomic:** T1082-1 — System Information Discovery 



The test was executed using:

```powershell
Invoke-AtomicTest T1082 -TestNumbers 1
```
## Screenshot 
[View Screenshot](../Screenshot/Screenshot(178).png) 
