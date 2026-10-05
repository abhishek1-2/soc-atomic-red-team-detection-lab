# SOC Adversary Simulation & Detection Lab

A hands-on SOC lab where I simulate MITRE ATT&CK techniques using Atomic Red Team, collect Windows telemetry with Sysmon, investigate the activity in Splunk, and develop detection logic.

## 🎯 Project Objective

The goal of this project is to practice the complete SOC investigation workflow:

ATT&CK Technique → Adversary Simulation → Windows Telemetry → Sysmon → Splunk → Investigation → Detection

Rather than only studying attack techniques theoretically, I simulate controlled adversary behavior inside an isolated Windows virtual machine and investigate the resulting telemetry.

---

## 🧪 Lab Environment

| Component | Purpose |
|---|---|
| Windows 11 VM | Target / monitored endpoint |
| Atomic Red Team | Adversary simulation |
| Sysmon | Endpoint telemetry |
| Splunk Enterprise | SIEM / investigation |
| Kali Linux | Supporting security lab |

### Windows Endpoint

Hostname:

`Windows_for_soc`

---

## 🔴 Adversary Simulation

I use Atomic Red Team tests mapped to MITRE ATT&CK techniques.

Each investigation follows:

1. Select an ATT&CK technique
2. Review the Atomic Red Team test
3. Execute the test in the isolated Windows VM
4. Observe the resulting Windows activity
5. Collect telemetry with Sysmon
6. Investigate the events in Splunk
7. Correlate process and parent-child relationships
8. Develop detection logic
9. Document the investigation

---

# Investigation 01 — T1082

## System Information Discovery

### MITRE ATT&CK

**Technique:** T1082 — System Information Discovery

### Atomic Red Team Test

**T1082-1 — System Information Discovery**

Execution:

```powershell
Invoke-AtomicTest T1082 -TestNumbers 1
