# Progress Log 19

## Overview
Continuing the my Internship at ProLab R, I wrapped up user account management and began file ownership and permissions from the **NDG Linux Essentials** course.

## Resource
- **Course:** NDG Linux Essentials
- **Topics Covered:** Password management, modifying/deleting users, file ownership, and group ownership commands

## Daily Progress Log

**Thursday - 1.10.2026**
- Learned how to **set user passwords** via `passwd`, including the different rules for root vs. regular users and the three-attempt limit for regular users
- Covered **`chage`** for managing password aging settings
- Studied **`usermod`** for modifying existing user accounts — comment field, home directory, groups, locking/unlocking, UID/login name changes — and the important distinction between `-G` (replaces groups) and `-aG` (appends groups)
- Learned **`userdel`** for deleting users, the difference between deleting with and without `-r`, and why locking an account (`usermod -L`) is often a safer alternative to deletion
- Completed the lab test chapter quiz for Chapter 16 - Creating Users and Groups

**Friday - 2.10.2026**
- Began Chapter 17 - Ownership and Permissions, with an introduction to file ownership (user owner and group owner) and permissions
- Studied **file ownership** fundamentals — how UID/GID (not names) are used internally, and how orphaned ownership appears when a UID/GID no longer matches an account
- Learned **`newgrp`** for temporarily switching the primary group for new file creation, and the `groups` command for quickly listing group memberships
- Covered **`chgrp`** for changing a file's group owner, including the `-R` recursive option and permission restrictions for non-root users
- Learned **`chown`** for changing user ownership (root-only) and optionally group ownership in the same command, plus the `stat` command for detailed file ownership info

## Key Takeaways
- Practical fluency with password management commands (`passwd`, `chage`) and account lifecycle commands (`usermod`, `userdel`)
- Clear understanding of the safer alternatives to deleting accounts, such as locking
- Solid grasp of how file and group ownership work internally (UID/GID-based) and how to view/change them with `chgrp`, `chown`, `newgrp`, and `stat`

## Next Steps
- Continue into the next Linux Essential chapters
- Practice user management and ownership commands hands-on in a virtual machine
