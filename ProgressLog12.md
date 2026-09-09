# Progress Log 12

## Overview
Continuing my Internship at ProLab R, I worked through the computer hardware fundamentals section of the **NDG Linux Essentials** course.
Also continued working on the project - Payroll and HR Management System

## Resource
- **Course:** NDG Linux Essentials
- **Topics Covered:** Motherboards, processors, RAM, buses, hard drives, SSDs, optical drives, device management, video display devices, and power supplies

## Daily Progress Log

**Monday - 7.9.2026**
- Completed the lab test and quiz for Chapter 11 - Basic Scripting. Started Chapter 12 - Understanding Computer Hardware.
- Learned why hardware knowledge matters for Linux administrators, even with the rise of virtual machines
- Covered **motherboards** as the central hardware connecting the CPU, RAM, and other components
- Studied **processors** — the x86 vs. x86_64 architectures, multiprocessor/multi-core concepts, and checking CPU info with `arch` and `lscpu`
- Learned about **RAM** and swap space, and how to check memory usage with the `free` command
- Used Lovable to continue working on fixing the gaps between the requirements and the build. Fixed the gaps in the **Attendance** route page

**Tuesday - 8.9.2026**
- Studied **buses** (PCI, USB) and how components connect differently on desktops/servers vs. laptops/small form-factor devices
- Learned about **peripheral devices** and viewing them with `lspci` (PCI devices) and `lsusb` (USB devices), including cold-plug vs. hot-plug behavior
- Covered **hard drives** — partitions, MBR vs. GPT partitioning, device file naming conventions, and tools like `fdisk`, `gdisk`, and `parted`
- Learned about **solid state disks (SSDs)** — how they differ from spinning disks, and their advantages/disadvantages
- Continued working on fixing the gaps between the requirements and the build. Fixed the gaps in the **Leave** route page

**Wednesday - 9.9.2026**
- Covered **optical drives** (CD/DVD/Blu-Ray), read-only vs. writable media, and mounting conventions (`/media` vs. `/mnt`)
- Learned about **device management** in Linux — drivers, kernel modules, vendor support challenges, and community-driven driver development
- Studied **video display devices** — driver considerations, common cable types (VGA, DVI, HDMI, DisplayPort), and resolution matching
- Learned about **power supplies** — their role converting AC to DC power, and vulnerability differences between battery-backed (laptop) and non-battery systems
- Completed the lab test and quiz for Chapter 12 - Understanding Computer Hardware.
- Continued working on fixing the gaps between the requirements and the build. Fixed the gaps in the **Payroll** route page

## Key Takeaways
- Solid understanding of core computer hardware components and how they interconnect via the motherboard and buses
- Practical familiarity with commands for inspecting hardware (`arch`, `lscpu`, `free`, `lspci`, `lsusb`, `fdisk`)
- Clear grasp of storage technologies (spinning disks, SSDs, optical drives) and partitioning concepts (MBR vs. GPT)
- Awareness of driver/device management challenges specific to Linux, and key hardware considerations (video, power supplies)

## Next Steps
- Continue into the next Linux Essentials chapter
- Practice hardware inspection commands hands-on in a virtual machine
- Keep working on the project- a Payroll and HR Management System.
