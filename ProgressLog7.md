# Progress Log 7

## Overview
This part of the Learning Week covered file and directory manipulation topics from the **NDG Linux Essentials** course, alongside completing the hands-on labs and quizzes for Chapters 7 and 8.
This README documents my Thursday, Friday, and Saturday progress and key takeaways.

## Resource
- **Course:** NDG Linux Essentials
- **Format:** Structured, chapter-based course notes plus hands-on labs and quizzes
- **Topics Covered:** Globbing, copying files/directories, moving and renaming files, creating and removing files/directories

## Daily Progress Log

**Thursday - 20.08.2026**
- Completed the **lab and quiz for Chapter 7** (Linux filesystem navigation — directory structure, paths, and the `ls` command)
- Reviewed the importance of **case-sensitivity** in Linux and the underlying UTF-8/ASCII character standard in Chapter 8
- Learned **globbing** fundamentals — how glob characters are interpreted by the shell before any command runs
- Covered the **asterisk (`*`)** character for matching zero or more of any character
- Covered the **question mark (`?`)** character for matching exactly one character, and combining it with `*` 
- Learned the **bracket (`[ ]`)** characters for matching a character from a set or range 
- Studied the **exclamation point (`!`)** character for negating a character range within brackets
- Explored the quirks of using **`ls` with glob patterns**, including why listing directories vs. files produces different output, and the `-d` fix

**Friday - 21.08.2026**
- Learned the **`cp`** command for copying files, including its basic syntax and default behavior
- Covered **verbose mode (`-v`)** for `cp`, and renaming files during a copy by specifying a new destination filename
- Studied the risks of **overwriting data** with `cp`, and the safeguards: `-i` (interactive) and `-n` (no-clobber)
- Learned that `cp` doesn't copy directories by default, and how to enable this with the recursive **`-r`** option, including the `-r` vs. `-R` distinction across commands
- Studied the **`mv`** command for moving files, including permission requirements
- Learned how `mv` is also used for **renaming files**, both when moving to a new directory and when renaming in place
- Covered additional `mv` options: `-i`, `-n`, `-v`, and noted `mv` has no `-r` option since it moves directories by default

**Saturday - 22.08.2026**
- Learned to create empty placeholder files using the **`touch`** command
- Studied the **`rm`** command for deleting files, the importance of the `-i` interactive option, and the permanent nature of deletions
- Covered removing **directories** using `rm -r` versus `rmdir` (only works on empty directories)
- Covered  on how to make directories using `mkdir` command
- Completed the **lab and quiz for Chapter 8** (file and directory manipulation)

## Key Takeaways
- Strong command of globbing patterns (`*`, `?`, `[ ]`, `!`) for flexible, pattern-based file matching
- Practical, hands-on fluency with `cp`, `mv`, `touch`, `rm`,`rmdir` and `mkdir` for everyday file and directory management
- Clear understanding of the safety considerations around overwriting and deleting files, and the options (`-i`, `-n`) that help prevent accidental data loss
- Reinforced Chapter 7 and Chapter 8 concepts through completed labs and quizzes

## Next Steps
- Continue into the next Linux Essentials chapter
- Apply globbing and file manipulation commands hands-on in real project work where relevant
