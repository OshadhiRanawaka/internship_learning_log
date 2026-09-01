# Progress Log 9

## Overview
Continuing the Learning Week during my Internship at ProLab R, I worked through the text file viewing and I/O redirection section of the **NDG Linux Essentials** course.

## Resource
- **Course:** NDG Linux Essentials
- **Topics Covered:** Viewing text files, pagers, `head`/`tail`, pipes, and I/O redirection (STDIN/STDOUT/STDERR)

## Daily Progress Log

**Friday - 28.8.2026 (Completed on Wed 26.82026)**
- Completed the lab test and chapter quiz for chapter 9 and the Mid Term exam of the course.
- Learned the `cat` command for displaying text file contents, and why pager commands (`less`, `more`) are better suited for large files in chapter 10
- Covered pager movement (Spacebar, B, Enter, Q, H) and search commands (`/` forward, `?` backward, `n`/`Shift+N` for next/previous match)
- Learned `head` and `tail` for viewing the first/last lines of a file, including the `-n` option, negative/positive value quirks, and using `tail -f` to watch live file changes

**Saturday - 29.08.2026 (Completed on Thur 27.08.2026)**
- Learned command line **pipes** (`|`) for passing one command's output as input to another, and how pipe order affects results (e.g., combining `ls`, `nl`, and `tail`)
- Covered **I/O redirection** basics — the three standard streams: STDIN, STDOUT, and STDERR
- Learned to redirect **STDOUT** to a file using `>` (overwrite) and `>>` (append)
- Learned to redirect **STDERR** specifically using `2>`, and how to distinguish STDERR from STDOUT output

## Key Takeaways
- Comfortable viewing and paging through text files using `cat`, `less`, and `more`
- Practical use of `head`/`tail` for quick file inspection and live log monitoring
- Solid understanding of pipes and how command order affects chained output
- Clear grasp of STDOUT vs. STDERR redirection fundamentals

## Next Steps
- Continue the remaining of the course
- Practice chaining pipes and redirects hands-on in a virtual machine
