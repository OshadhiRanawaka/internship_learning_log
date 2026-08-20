# Progress Log 6

## Overview
Continuing the Learning Week during my Internship at ProLab R, I worked through the remaining help/documentation topics and began the filesystem navigation section of the **NDG Linux Essentials** course. 
This README documents my Monday–Wednesday progress and key takeaways.

## Resource
- **Course:** NDG Linux Essentials
- **Format:** Structured, chapter-based course notes
- **Topics Covered:** Finding files (`locate`), info documentation, additional help sources, filesystem structure, paths, and the `ls` command in depth

## Daily Progress Log

**Monday - 17.8.2026**
- Learned to find any file or directory using the **`locate`** command, including how its database is built/updated (`updatedb`), permission-based filtering, and narrowing results with `-c` and `-b`
- Studied **info documentation** as an alternative to man pages — its more structured, book-like organization with hyperlinked nodes, and how it compares to man pages as a learning resource vs. a reference tool
- Learned to **view info pages** using the `info` command, navigate with arrow keys, and move between nodes using `U` and `L`

**Tuesday - 18.8.2026**
- Covered detailed **info document navigation** — the full set of movement keys (Up/Down, PgUp/PgDn, Home/End, TAB, RET, `[`/`]`, `p`/`n`, `u`) accessible via Shift+H
- Learned how to **explore info documentation** broadly by running `info` with no arguments to browse the top-level menu/table of contents
- Explored **additional sources of help**, including the `--help` option available on most commands for quick usage summaries, and system documentation directories containing README files from software vendors
- Began Chapter 7 with an introduction to the Linux philosophy that **"everything is a file,"** and the importance of managing files/directories via the command line
- Learned the Linux **directory structure**, comparing it to Windows' "My Computer" model, and explored the root directory (`/`) using `ls /`
- Studied the **home directory** concept — its location under `/home`, its special access permissions, and its `~` shortcut symbol
- Learned to check current location using **`pwd`**, and to navigate directories using **`cd`**, including returning home with no arguments
- Covered **paths** in depth — the distinction between **absolute paths** (always starting from root `/`) and **relative paths** (starting from the current directory)

**Wednesday - 19.8.2026**
- Learned **shortcut navigation** using `..` (parent directory) and `.` (current directory)
- Deep-dived into the **`ls`** command:
  - Basic usage and listing other directories
  - Understanding the `--color` alias and bypassing it with `\ls`
  - Displaying hidden files with `-a`
  - Long listing format (`-l`) and interpreting file type, permissions, hard link count, owner, group, size, timestamp, and filename fields
  - Human-readable file sizes with `-h`
  - Listing directory details themselves with `-d`
  - Recursive listings with `-R`
  - Sorting listings by size (`-S`) and modification time (`-t`), combined with `-l`, `-h`, `--full-time`, and reverse sorting with `-r`

## Key Takeaways
- Confident using `locate` to search the filesystem broadly, and understanding its database-driven, permission-aware behavior
- Comfortable navigating and exploring documentation using both `info` and `--help`, in addition to man pages
- Strong grasp of the Linux filesystem hierarchy, the home directory, and the distinction between absolute and relative paths
- Practical, hands-on command of the `ls` command's many options for listing, sorting, and interpreting file metadata

## Next Steps
- Continue covering the remaining course materials
- Practice navigating and listing files hands-on in a virtual machine
