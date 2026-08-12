# Progress Log 4

## Overview
Continuing the Progress Log during my Internship at ProLab R, I worked through the final open source licensing topics and began the command line fundamentals section of the **NDG Linux Essentials** course.
This README documents my progress and key takeaways.

## Resource
- **Course:** NDG Linux Essentials
- **Format:** Structured, chapter-based course notes
- **Topics Covered:** Open source licensing (OSI, Creative Commons, business models), shells, commands, arguments/options, command history, variables, command types, aliases, functions, quoting, control statements

## Daily Progress Log

**Monday - 10.8.2026**
- Studied the **Open Source Initiative (OSI)** — its founding, philosophy, and how it differs from the FSF's copyleft-focused approach
- Learned about **BSD licenses** as examples of permissive open source licenses, and the distinction between copyleft and permissive licensing (BSD, MIT vs. GPL)
- Covered the terminology around **FOSS** and **FLOSS** (Free/Libre/Open Source Software)
- Explored **Creative Commons** licensing for non-software works — public domain concepts, the four core conditions (Attribution, ShareAlike, NonCommercial, NoDerivatives), and the six main CC licenses plus CC0
- Reviewed **open source business models** — how companies profit from free software through support/warranty sales (Canonical, Red Hat), growing community projects into businesses (Wireshark), and hardware/appliance bundling (TiVo, embedded devices)
- Began Chapter 5 with an introduction to why the Linux community embraces the **CLI**, and the productivity/portability benefits of learning it
- Learned how the **shell** interprets commands, compared Bash's key features, and reviewed the structure of the Bash **prompt**

**Tuesday - 11.8.2026**
- Learned the fundamentals of Linux **commands** — what a command is and the basic `command [options] [arguments]` structure
- Studied **arguments** in depth, including how commands like `ls` can accept single or multiple arguments
- Covered **options** in detail — single-letter vs. full-word options, combining options, and practical examples using `-l`, `-r`, and `-h`
- Explored the **command history** system — navigating with arrow keys, the `history` command, and re-executing commands using `!n`, `!-n`, `!!`, and `!commandname`
- Learned about **local (shell) variables** — how to set, access, and scope them to the current shell session
- Studied **environment variables** — the difference from local variables, key examples (`PATH`, `HOME`, `HISTSIZE`), and how to use `env`, `export`, and `unset`

**Wednesday - 12.8.2026**
- Deep-dived into the **PATH variable** — how the shell uses it to locate commands, how to view/modify it, and troubleshooting "command not found" errors
- Learned to use the **`type`** command to identify command sources
- Covered the four types of shell commands:
  - **Internal (built-in) commands** (e.g., `cd`)
  - **External commands** (binary executables located via `PATH`, using `which` and `type`)
  - **Aliases** (mapping short names to longer commands, viewing/creating them, and their session-only persistence)
  - **Functions** (combining multiple commands into a single reusable command, with proper syntax)
- Studied **quoting** in Bash — double quotes (blocking glob interpretation while still allowing variable/command substitution), single quotes (blocking all special interpretation), the backslash character (escaping individual characters), and backquotes/backticks (command substitution)
- Introduced **control statements** — using multiple commands together or conditionally, based on the success of a previous command

## Key Takeaways
- Solid understanding of the open source licensing landscape — OSI vs. FSF philosophies, permissive vs. copyleft licenses, and Creative Commons for non-software works
- Clear picture of how open source projects and companies build sustainable business models
- Strong foundational grasp of the Bash shell — commands, arguments, options, history, and variables
- Practical knowledge of command types (internal, external, aliases, functions) and how to identify them
- Understanding of Bash quoting rules and when to use double quotes, single quotes, backslashes, or backquotes

## Next Steps
- Continue through the remaining Linux Essentials chapters
- Practice command line exercises hands-on in a virtual machine
