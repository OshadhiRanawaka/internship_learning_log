# Progress Log 11

## Overview
Continuing my Internship at ProLab R, I wrapped up regular expressions and began shell scripting fundamentals from the **NDG Linux Essentials** course.
Also continued working on the project - Payroll and HR Management System

## Resource
- **Course:** NDG Linux Essentials
- **Topics Covered:** Regex (asterisk, anchors, backslash, extended regex), shell script basics, editing with nano, variables, conditionals, and loops

## Daily Progress Log

**Thursday - 3.9.2026**
- Learned the **asterisk (`*`)** character in regex — matching zero or more of the preceding character, and why it needs pairing with another character to be useful
- Covered **anchor characters** `^` (start of line) and `$` (end of line) for pinpointing match position
- Learned the **backslash (`\`)** for escaping special regex characters to match them literally
- Covered **extended regular expressions** (`grep -E`) — the `?` (optional), `+` (one or more), and `|` (OR/alternation) operators

**Friday - 4.9.2026**
- Completed the lab test and quiz for chapter 10.
- Began Chapter 11 with an introduction to turning command line skills into **reusable shell scripts**
- Learned shell script fundamentals — the shebang (`#!`) line, running scripts via `sh script` vs. directly with `./script` (and the `chmod +x` permission requirement)
- Learned to edit scripts using the **nano** editor — basic navigation, saving/exiting (`Ctrl+X`, `Ctrl+O`), cut/paste (`Ctrl+K`/`Ctrl+U`), and search commands
- Previewed the three core scripting concepts to learn next: variables, conditionals, and loops

**Saturday - 5.9.2026**
- Learned **variables** in shell scripts — assignment, interpolation with `$`, command substitution with backticks, user input via `read`, positional arguments (`$1`, `$0`), and exit codes (`$?`, `exit`)
- Covered **conditionals** — `if`/`else`/`elif` statements, the `test` command and its `[ ]` shorthand for file/string/numeric comparisons, and the `case` statement as a cleaner alternative for multiple pattern checks
- Learned **loops** — `for` loops for iterating over finite lists (variables, direct lists, and globs) and `while` loops for condition-based repetition

## Key Takeaways
- Strong grasp of anchors, escaping, and extended regex operators for precise pattern matching
- Comfortable creating, permissioning, and running basic shell scripts, and editing them in nano
- Practical understanding of shell scripting fundamentals — variables, conditionals (`if`/`case`), and loops (`for`/`while`) — as building blocks for automation

## Next Steps
- Continue building more complex shell scripts combining variables, conditionals, and loops
- Practice writing and running scripts hands-on in a virtual machine
