# Windows 11 – IT Support Troubleshooting Lab

## Overview

This lab demonstrates basic Windows 11 troubleshooting and system monitoring skills using a virtual machine environment.

The objective was to investigate system performance, identify resource bottlenecks, and review Windows system logs using built-in administrative tools.

## Environment

- Operating System: Windows 11
- Virtualization: VMware Workstation
- CPU: Intel Core i5-10400F
- RAM: 4 GB allocated to the virtual machine
- Network: VMware virtual network
- Host Lab: Windows Server 2019 + Windows 11

---

## 1. Task Manager – Resource Monitoring

I used Windows Task Manager to monitor system resource utilization.

### Areas Reviewed

- CPU utilization
- Memory utilization
- Disk utilization
- Network activity
- Running applications
- Background processes

### Observation

The Disk resource reached 100% utilization during the troubleshooting session while CPU and memory usage remained significantly lower.

This demonstrates how Task Manager can be used to identify a potential disk-performance bottleneck.

---

## 2. Performance Monitoring

The Performance tab in Task Manager was used to examine system resource behavior over time.

### Resources Monitored

- CPU
- Memory
- Disk
- Ethernet

### Findings

The virtual machine showed:

- Low CPU utilization
- Moderate memory utilization
- High disk utilization
- Minimal network activity

This helped isolate the primary performance issue to disk activity rather than CPU or network usage.

---

## 3. Event Viewer

Windows Event Viewer was used to inspect system-level events and warnings.

### Navigation

`Event Viewer → Windows Logs → System`

### Event Reviewed

- Log: System
- Source: DistributedCOM
- Event ID: 10016
- Level: Warning

The event was reviewed to practice identifying the event source, event ID, severity level, and additional event information.

### Troubleshooting Approach

When investigating Windows issues, Event Viewer can be used to:

1. Identify the affected Windows log.
2. Review the event severity.
3. Identify the event source.
4. Check the Event ID.
5. Review the event details.
6. Determine whether the event is related to the reported issue.

---

## Skills Demonstrated

- Windows 11 troubleshooting
- Task Manager
- Performance monitoring
- Resource utilization analysis
- Disk troubleshooting
- Event Viewer
- Windows system logs
- Event ID investigation
- Basic incident troubleshooting
- Virtual machine administration

---

## Tools Used

- Windows 11
- VMware Workstation
- Task Manager
- Event Viewer

---

## Lab Evidence

Screenshots included in this repository demonstrate:

1. Task Manager – Processes and resource utilization
2. Task Manager – CPU and system performance
3. Event Viewer – System log and Event ID 10016
4. Windows 11 virtual machine environment

---

## Conclusion

This lab provided practical experience with Windows troubleshooting and system monitoring.

The investigation demonstrated how to use built-in Windows administrative tools to identify resource utilization issues and investigate system events.

These are fundamental skills for IT Support, Help Desk, and Technical Support roles.
