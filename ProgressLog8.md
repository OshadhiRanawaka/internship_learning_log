# Progress Log 8

## Overview
Continuing the Learning Week during my Internship at ProLab R, I worked through the archiving and compression section of the **NDG Linux Essentials** course.
This README documents my Monday–Tuesday progress and key takeaways.

## Resource
- **Course:** NDG Linux Essentials
- **Format:** Structured, chapter-based course notes
- **Topics Covered:** File compression, archiving with `tar`, and ZIP file handling

## Daily Progress Log

**Monday - 24.08.2026**
- Learned why **archiving and compression** matter for Linux administrators, even with cheap disk space — easier distribution, log management, backups, and faster transmission
- Studied the distinction between **archiving** (combining files) and **compression** (shrinking file size)
- Covered **lossless vs. lossy compression**, and how they apply differently to documents/logs versus media files like images
- Learned to compress and decompress files using **`gzip`** and **`gunzip`**, including checking compression ratios with `gzip -l`
- Compared `gzip` with alternative tools **`bzip2`/`bunzip2`** and **`xz`/`unxz`**, and their respective trade-offs in compression ratio vs. CPU time
- Began learning the **`tar`** command for archiving multiple files into one — covering its three core modes: create, extract, and list
- Learned **Create Mode** (`tar -c`) in depth — building tarballs, combining archiving with compression using `-z` (gzip) or `-j` (bzip2), and file extension conventions

**Tuesday - 25.08.2026**
- Learned **List Mode** (`tar -t`) — viewing archive contents without extracting, and how `tar` preserves directory structure and recurses into subdirectories automatically
- Explored using **pipelines** (`bunzip2 -c | tar -t`) to manually decompress and list archive contents as an alternative to built-in options
- Learned **Extract Mode** (`tar -x`) — extracting full archives, using verbose output (`-v`), the importance of keeping `-f` as the last flag, and extracting specific files from an archive
- Studied **ZIP file handling** using the `zip` and `unzip` commands — noting key differences from `tar` (no `-f` flag needed, no automatic recursion without `-r`) (9.4)
- Learned to **list ZIP contents** with `unzip -l`, extract archives (including handling overwrite prompts), and extract specific files using exact paths or wildcard patterns

## Key Takeaways
- Solid understanding of compression fundamentals — lossless vs. lossy, and when each is appropriate
- Practical fluency with `gzip`/`gunzip` and awareness of alternative tools (`bzip2`, `xz`) and their trade-offs
- Strong command of `tar`'s three modes (create, extract, list) and how to combine archiving with compression
- Working knowledge of ZIP file management via `zip`/`unzip`, including key behavioral differences from `tar`

## Next Steps
- Continue into the next Linux Essentials chapters
- Practice archiving and compressing files hands-on in a virtual machine to reinforce `tar` and `zip` workflows
