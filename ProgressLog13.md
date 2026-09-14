# Progress Log 13

## Overview
Continuing my Internship at ProLab R, I worked through the kernel, processes, memory, and logging section of the **NDG Linux Essentials** course.
Also continued working on the project - Payroll and HR Management System

## Resource
- **Course:** NDG Linux Essentials
- **Topics Covered:** Kernel fundamentals, `/proc` pseudo filesystem, process hierarchy, viewing processes (`ps`, `top`), memory management, and log files

## Daily Progress Log

**Thursday - 10.9.2026**
- Completed the lab test and quiz for Chapter 12 - Understanding Computer Hardware. Started Chapter 13 - Where Data is Stored.
- Reviewed the role of the **Linux kernel** — system call interface, process/memory management, virtual filesystems, networking, and device drivers
- Learned about the **`/proc`** pseudo filesystem — how it exposes process and hardware/kernel info, and its use by commands like `top` and `free`
- Studied **process hierarchy** — the `init` process (PID 1), parent/child relationships, PPID, and visualizing the process tree with `pstree`
- Learned to view process snapshots with **`ps`**, including `--forest`, `ps aux`/`ps -ef` for all processes, and filtering with `grep` or `-u`
- Covered **`top`** for real-time process monitoring — sorting by CPU%, interactive commands (`K` to kill, `R` to renice), and interpreting load averages

**Friday - 11.9.2026**
- Studied **memory management** fundamentals — virtual addressing, user space vs. kernel space, and why this separation gives Linux stability
- Learned to view memory usage with **`free`**, including the `-s`, `-m`, and `-g` options, and how to interpret physical memory, adjusted memory, and swap
- Covered **log files** — logging daemons (`syslogd`/`klogd`, `rsyslogd`, `journald`), common log files in `/var/log`, viewing logs with `cat`/`less`/`journalctl`, log rotation, and handling binary logs with `file`, `last`, and `lastb`
- Learned about **kernel messages** specifically — `dmesg`, the kernel ring buffer, its size limitations, and filtering kernel output with `grep`

**Saturday - 12.9.2026**
- Reviewed the project codebase to plan the Attendance route build, then hit Antigravity's credit limit partway through
- Verified role-based access across all 8 user roles on the Dashboard, catching and fixing a permissions gap and a wrong specification citation
- Found and fixed several bugs on the Employees and Attendance pages: broken tabs, a non-working Add Employee button etc.
- Restructured the Leave module's role permissions to match the specification, then fixed a related tab-navigation bug affecting three of its four views
- Built a working mock Sign In/Sign Up flow with persistent sessions, and upgraded Sign Up into a full employee registration form tied to the shared employee directory
- Fixed a non-functional filter on the Employees page
- Wrote a full implementation plan documenting the project's architecture and remaining work
- Planned a new "My Account" settings page and the shot order for a demo video

## Key Takeaways
- Solid understanding of how the kernel manages processes and memory, and how to inspect this via `/proc`
- Practical fluency with `ps`, `top`, and `pstree` for monitoring and troubleshooting processes
- Clear grasp of memory concepts (virtual addressing, swap) and how to monitor usage with `free`
- Strong foundation in Linux logging — locating, viewing, and filtering log files, including kernel-specific messages via `dmesg`

## Next Steps
- Continue into the next Linux Essentials chapter
- Practice process and memory monitoring commands hands-on in a virtual machine
- Keep working on the project- a Payroll and HR Management System
