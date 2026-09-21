# Progress Log 15

## Overview
Continuing my Internship at ProLab R, I worked through the network tools and troubleshooting commands section of the **NDG Linux Essentials** course.
Also continued working on the project - Payroll and HR Management System

## Resource
- **Course:** NDG Linux Essentials
- **Topics Covered:** Network interface and routing tools, DNS query tools, and remote login with SSH

## Daily Progress Log

**Thursday - 17.9.2026**
- Learned **`ifconfig`** for displaying network interface configuration, including the loopback device (`lo`)
- Studied the newer **`ip`** command (`ip addr show`) as the modern replacement for `ifconfig`, and compared their outputs
- Covered **`route`** for viewing the routing table, the `-n` numeric option, and its modern replacement `ip route show`
- Learned **`ping`** for testing host reachability, limiting attempts with `-c`, and why a failed ping doesn't always mean a host is unreachable
- Built the Employee Self-Service portal of the project as a fully separate layout from the admin shell, with personal Dashboard, Profile, Attendance, Leave, Payslips, and Requests views scoped to the logged-in employee's own data.

**Friday - 18.9.2026**
- Studied **`netstat`** for viewing network statistics, routing info, and open ports (`-i`, `-r`, `-tln`), and noted it's being replaced by `ss` and `ip` commands
- Learned **`ss`** as the modern socket statistics tool, including basic usage and the `-s` summary option
- Covered **`dig`** for testing DNS server functionality and resolving hostnames to IP addresses
- Learned **`host`** for hostname-to-IP and reverse lookups, plus querying specific DNS record types (CNAME, SOA) and comprehensive lookups with `-a`
- Studied **`ssh`** for connecting to and logging into remote machines, including username syntax and the `exit` command
- Learned about **RSA key fingerprints** in SSH — how they're verified and stored on first connection, what a "host identification has changed" warning means, and how to safely resolve it after a legitimate remote machine reinstall
- Diagnosed and fixed a data-sharing bug so leave requests and new sign-ups now correctly flow into the same shared data the admin pages read from, then traced and resolved a related blank-page regression affecting sign-in and the admin Leave page.
- Planned the visual redesign direction for the Self-Service portal (calmer, more personal styling distinct from the admin shell); implementation still pending.

**Saturday - 19.92026**
- Studied Material UI basics (purpose, core components, theming, trade-offs) to prepare for taking over a partially built project that uses it.
- Worked out how to connect the MUI MCP server and set project rules in Antigravity so the agent follows the project's MUI conventions.
- Prepared a post-clone checklist for setup and for auditing how MUI is used (version, theme, styling approach).
- Wrote an Antigravity audit prompt to map the codebase structure, reusable patterns, and progress against the spec, so the remaining work follows the existing conventions of the new repository of the project.


## Key Takeaways
- Comfortable using both legacy (`ifconfig`, `route`, `netstat`) and modern (`ip`, `ss`) network inspection tools
- Practical fluency with DNS troubleshooting tools (`dig`, `host`) for verifying name resolution
- Solid understanding of SSH for remote access, including the security implications of RSA key fingerprint mismatches

## Next Steps
- Continue into the next Linux Essentials chapter
- Practice using these network tools hands-on in a virtual machine for troubleshooting scenarios
- Keep working on the project- a Payroll and HR Management System
