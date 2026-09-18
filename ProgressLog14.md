# Progress Log 14

## Overview
Continuing my Internship at ProLab R, I wrapped up the filesystem section and began networking fundamentals from the **NDG Linux Essentials** course.
Also continued working on the project - Payroll and HR Management System


## Resource
- **Course:** NDG Linux Essentials
- **Topics Covered:** Filesystem Hierarchy Standard, networking terminology, IP addressing, network device configuration, and DNS configuration files

## Daily Progress Log

**Monday - 14.9.2026**
- Learned the **Filesystem Hierarchy Standard (FHS)** — how directories are classified as shareable/not shareable and static/variable, and the four directory hierarchies (root, `/usr`, `/usr/local`, `/var`)
- Studied the detailed organization within the filesystem — home directories, binary directories (user vs. root-restricted), software application directories, library directories, and variable data directories under `/var`
- Completed the lab test and Chapter quiz of Chapter 13 - Where Data is Stored
- Worked on the project - Payroll and HR Management System.
- Built out the Payroll route: payroll runs list, a detailed earnings/deductions/validation view per run, salary structures, and a Loans & Advances tab.
- Implemented real maker-checker enforcement (a Payroll Officer can prepare a run but not approve it; only a Checker role can approve) and added a "New Payroll Run" action that auto-populates a draft period from existing attendance/leave data.

**Tuesday - 15.9.2026**
- Began Chapter 14 - Network Configuration with an introduction to why network access and configuration matter on Linux systems
- Learned **basic networking terminology** — host, network, Internet, Wi-Fi, server, service, client, and router
- Covered **networking features terminology** — packet, IP address, mask, hostname, URL, DHCP, DNS, Ethernet, and TCP/IP
- Studied **IP addressing** in depth — the difference between IPv4 (32-bit) and IPv6 (128-bit), and why IPv6 adoption remains limited despite its advantages
- Worked on the project - Payroll and HR Management System.
- Cross-checked the remaining unbuilt sidebar pages against the specification's phased roadmap, confirming Recruitment and Performance are intentionally deferred, and that Loans & Advances is already effectively covered via the new Payroll tab.
- Began the Devices route: biometric device directory with health status, sync history, and a "Retry Sync" action.

**Wednesday - 16.9.2026**
- Learned the two key questions when configuring network devices: wired vs. wireless, and DHCP vs. static addressing
- Covered configuring networks via **configuration files** when no GUI tool is available, including the primary IPv4 and IPv6 configuration files on CentOS (`ifcfg-eth0`)
- Learned how to apply network changes safely using `ifdown`/`ifup` versus the more disruptive `service network restart`
- Studied **DNS configuration** — the role of `/etc/resolv.conf`, and how `/etc/hosts`, `/etc/resolv.conf`, and `/etc/nsswitch.conf` work together to resolve hostnames, including the lookup order and fallback behavior
-  Worked on the project - Payroll and HR Management System.
- Confirmed Reports remains part of the core build order (Phase 5) and clarified Expenses' split scope — its employee-facing submission flow will come later via Self-Service, while the full admin approval module stays deferred.
- Built out the Reports route: a catalogue of all nine specification report types, with three made fully functional (Payroll, Attendance, Headcount/Turnover) reusing existing Dashboard chart components and department-scoped filtering.

## Key Takeaways
- Solid understanding of the Linux Filesystem Hierarchy Standard and how directories are organized and classified
- Strong foundation in core networking concepts and terminology
- Clear grasp of IPv4 vs. IPv6 and the practical reasons IPv6 adoption has been slow
- Practical knowledge of network configuration files and the proper way to apply and troubleshoot network changes

## Next Steps
- Continue with network tools (`ifconfig`, `ip`, `route`, `ping`) for monitoring and troubleshooting
- Practice network configuration hands-on in a virtual machine
- Keep working on the project- a Payroll and HR Management System
