# Progress Log 18

## Overview
Continuing my Internship at ProLab R, I worked through the user and group creation/management section of the **NDG Linux Essentials** course.

## Resource
- **Course:** NDG Linux Essentials
- **Topics Covered:** Group creation/modification/deletion, user configuration files, account planning, and user creation

## Daily Progress Log

**Monday - 28.9.2026**
- Completed the Lab test and Chapter quiz for the Chapter 15 - System and User Security. Started Chapter 16 - Creating Users and Groups
- Learned why separate user accounts matter on shared systems, and the concept of User Private Groups (UPG)
- Studied **groups** as the main mechanism for file sharing/collaboration, and how to verify group info with `grep` and `getent`
- Learned **`groupadd`** for creating groups (with `-g` for custom GID), GID range considerations to avoid UPG conflicts, and group naming guidelines

**Tuesday - 29.9.2026**
- Covered **`groupmod`** for renaming groups (`-n`) and changing GIDs (`-g`), including why GID changes orphan files while renaming does not
- Learned **`groupdel`** for deleting groups, the restriction against deleting a primary group, and using `find -nogroup` to locate orphaned files
- Began user account creation — the `/etc/passwd` and `/etc/shadow` files, and why `useradd` is safer than manual file edits

**Wednesday - 30.9.2026**
- Studied `useradd` default configuration via **`/etc/default/useradd`** (`-D` option) — GROUP, HOME, INACTIVE, EXPIRE, SHELL, SKEL, CREATE_MAIL_SPOOL
- Learned the **`/etc/login.defs`** file settings — password aging (PASS_MAX_DAYS, PASS_MIN_DAYS, PASS_MIN_LEN, PASS_WARN_AGE), UID/GID ranges, CREATE_HOME, UMASK, UPG, and encryption method
- Covered **account planning considerations** — username/UID guidelines, primary/supplementary groups, home directory options, skeleton directory, shell, and the comment (GECOS) field
- Learned to **create a user** with `useradd` using multiple options at once, and reviewed how the command updates `/etc/passwd`, `/etc/shadow`, `/etc/group`, `/etc/gshadow`, mail spool, and home directory
- Studied **password best practices** — avoiding personal info, length/composition/lifetime considerations, and balancing password change frequency against usability

## Key Takeaways
- Comfortable creating, modifying, and deleting groups with `groupadd`, `groupmod`, and `groupdel`
- Strong understanding of the default configuration files (`/etc/default/useradd`, `/etc/login.defs`) that shape new user accounts
- Practical fluency with `useradd` options for controlling UID, groups, home directory, skeleton directory, shell, and comment fields
- Clear grasp of password security principles and how they tie into account configuration

## Next Steps
- Continue into the next Linux Essentials chapter
- Practice creating users and groups hands-on in a virtual machine
