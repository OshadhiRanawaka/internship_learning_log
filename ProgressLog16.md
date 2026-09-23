# Progress Log 16

## Overview
Continuing the my Internship at ProLab R, I worked through the user and group account management section of the **NDG Linux Essentials** course.
Also continued working on the project - Payroll and HR Management System

## Resource
- **Course:** NDG Linux Essentials
- **Topics Covered:** Administrative accounts, user/group account files, system accounts, and viewing user/login information

## Daily Progress Log

**Monday - 21.9.2026**
- Learned why user accounts and file permissions exist to provide system security, and how groups help manage shared access
- Studied why direct root login is discouraged, and the two alternatives: `su` (switching users, requiring the target account's password) and `sudo` (running individual commands as root using your own password, with full logging for accountability)
- Reviewed the Nimbroll - Payrolland HRMS spec, API docs, and frontend/backend guides, converted them to Markdown, and set up AGENTS.md plus docs/ for the workspace, frontend, and backend.
- Ran the codebase audits on both repos, reviewed the reports, and updated the AGENTS.md files to match the findings.

**Tuesday - 22.9.2026**
- Learned the structure of **`/etc/passwd`** — username, password placeholder, UID, primary GID, comment, home directory, and shell fields
- Studied **`/etc/shadow`** in depth — the encrypted password field and all the password aging fields (last change, minimum, maximum, warn, inactive, expire, reserved)
- Covered **system accounts** — how they differ from regular user accounts (UID range, no login shell, no usable password) and why they shouldn't be deleted carelessly
- Reviewed the actual frontend and backend source directly, going deeper than the earlier audit reports.
- Found real issues the audit missed — and corrected both AGENTS.md files with them.
- Split all remaining work into cross-repo, frontend-only, and backend-only lists in a shared file, with a suggested build order.

**Wednesday - 23.9.2026**
- Learned the structure of **`/etc/group`** — group name, password placeholder, GID, and user list fields, and how primary vs. secondary group membership is defined
- Studied the **`id`** command for viewing user/group info, including `-g` (primary group) and `-G` (all groups) options
- Learned **`who`** and **`w`** for viewing currently logged-in users and system status, and **`last`** for viewing full login history from `/var/log/wtmp`

## Key Takeaways
- Solid understanding of the security reasoning behind `su` vs. `sudo`, and when each is appropriate
- Strong grasp of the `/etc/passwd`, `/etc/shadow`, and `/etc/group` file structures and what each field controls
- Practical fluency with `id`, `who`, `w`, and `last` for investigating user activity and login history

## Next Steps
- Continue into the next Linux Essentials chapter
- Practice user/group account inspection commands hands-on in a virtual machine
- Keep working on the project- a Payroll and HR Management System
