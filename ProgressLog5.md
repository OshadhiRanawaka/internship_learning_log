# Progress Log 5

## Overview
This week continued with the command line fundamentals section of the **NDG Linux Essentials** course, alongside onboarding research for a new project I've been assigned.
This README documents my progress and key takeaways.

## Resource
- **Course:** NDG Linux Essentials
- **Format:** Structured, chapter-based course notes
- **Topics Covered:** Control statements, man pages, searching and categorizing documentation, locating commands
- **Other:** Project onboarding demo video and Lovable tool tutorials

## Daily Progress Log

**Thursday - 13.8.2026**
- Wrapped up **control statements** in the shell:
  - **Semicolon (`;`)**: Running multiple commands sequentially, regardless of success or failure
  - **Double ampersand (`&&`)**: Logical "AND" — the second command only runs if the first succeeds
  - **Double pipe (`||`)**: Logical "OR" — the second command only runs if the first fails
- Began Chapter 6 with an introduction to why finding help on the command line is an essential skill given the sheer number of commands and options available
- Learned about **man pages** — their UNIX origins and their role in documenting command purpose and options
- Covered how to **view man pages** using the `man` command, navigate with arrow keys, exit with `Q`, and use `H` to view pager movement commands

**Friday - 14.8.2026**
- Watched a **demo video** covering the new project I've been assigned to, and gained a thorough understanding of the project's goals and overall focus
- Researched **Lovable** as a tool to quickly and efficiently build out the project system
- Watched tutorial videos demonstrating how to work with Lovable, along with quick tips for working more efficiently within the tool
- In Chapter 6 of the course I studied the **structure of man pages**, covering common sections: NAME, SYNOPSIS, DESCRIPTION, OPTIONS, FILES, AUTHOR, REPORTING BUGS, COPYRIGHT, and SEE ALSO
- Learned how to interpret **SYNOPSIS notation** — square brackets for optional items, ellipses for repeatable options, and pipe characters for mutually exclusive/equivalent options

**Saturday - 15.8.2026**
- Learned how to **search within a man page** using `/`, and navigate matches with `n` and `Shift+N`
- Explored how man pages are **categorized into nine sections** (general commands, system calls, library calls, special files, file formats, games, miscellaneous, system admin commands, and kernel routines), and how `man` searches sections in order
- Learned to handle **duplicate man page names** across sections using `man -f` (or `whatis`) to identify sections, and `man <section> <name>` to view a specific one
- Covered **keyword-based searching** across man pages using `man -k` (or `apropos`)
- Learned to locate a command's binary, source files, and man pages using the **`whereis`** command, and how to distinguish man pages (`.gz` files) from actual executables

## Key Takeaways
- Comfortable combining shell commands using `;`, `&&`, and `||` depending on desired execution logic
- Strong grasp of how to find and interpret help documentation via man pages
- Practical ability to locate commands and their documentation across man page sections using `whatis`, `man -f`, `man -k`, and `whereis`
- Clear initial understanding of the new project's goals and a starting toolkit (Lovable) to begin building it efficiently

## Next Steps
- Apply man page and command-lookup skills hands-on in a virtual machine
- Begin scoping out the new project's requirements and start prototyping using Lovable
