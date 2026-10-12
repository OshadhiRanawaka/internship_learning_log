# Progress Log 21

## Overview
Continuing my Internship at ProLab R, I worked through changing and defaulting file permissions, and began the special permissions section of the **NDG Linux Essentials** course.

## Resource
- **Course:** NDG Linux Essentials
- **Topics Covered:** `chmod` symbolic and numeric methods, `umask` default permissions, setuid, and setgid on files

## Daily Progress Log

**Thursday - 8.10.2026**
- Learned the **symbolic method** of `chmod`, which is best for changing a few permissions while leaving the rest alone. It combines who (`u`, `g`, `o`, `a`), an operator (`+`, `-`, `=`) and a permission type (`r`, `w`, `x`), and several changes can be combined with commas
- Learned the **numeric (octal) method**, where read is 4, write is 2 and execute is 1. Each of the three permission groups gets a digit from 0 to 7, and all nine permissions have to be specified, which makes this method better for drastic changes
- Saw that `stat` shows permissions in both symbolic and numeric form, unlike `ls -l`
- Studied **default permissions** with `umask`, which is subtracted from the maximum defaults (666 for files, 777 for directories). A new file can never start with execute permission, and the same umask gives different results for files and directories
- Learned that a umask set on the command line only lasts for that session, and that a permanent change goes in the user's `.bashrc`

**Friday - 9.10.2026**
- Completed the lab test and chapter quiz of Chapter 17 - Ownership and Permissions
- Began Chapter 18 - Special Directories and Files ,with an introduction to why special permissions (setuid, setgid and the sticky bit) exist when multiple users share directories and files
- Studied **setuid**, which runs an executable as its owner instead of the user who launched it. `passwd` is the example: it can modify `/etc/shadow` for normal users because it runs as root
- Learned to spot setuid in `ls -l` (lowercase `s` versus uppercase `S`), and how to add and remove it with `chmod` using `u+s` or the numeric 4000 value. A three-digit code removes any existing special permission
- Began **setgid**, which works with the group owner permissions and has two forms, one for files and one for directories
- Covered **setgid on files**, where a user gets temporary group access only while running the program. `/usr/bin/wall` is the example: it needs the `tty` group to write to terminal files

## Key Takeaways
- Can choose between the symbolic and numeric `chmod` methods depending on how many permissions need to change
- Understand how `umask` is subtracted from the maximum defaults, and why files and directories end up with different defaults
- Understand that setuid and setgid let a program temporarily act as its file's owner or group, and how to read them in `ls -l` output

## Next Steps
- Continue with the next Linux Essential course chapters
- Practice `chmod`, `umask` and special permissions hands-on in a virtual machine
