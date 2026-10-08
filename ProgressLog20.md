# Progress Log 20

## Overview
Continuing my Internship at ProLab R, I worked through file and directory permissions from the **NDG Linux Essentials** course, including a series of scenario-based exercises on how permissions are actually evaluated.

## Resource
- **Course:** NDG Linux Essentials
- **Topics Covered:** File types, permission groups and types, permission scenarios, and an introduction to `chmod`

## Daily Progress Log

**Monday - 5.10.2026**
- Learned how to read the 10-character permission string from `ls -l` — the file type character followed by three permission groups: user owner, group owner, and other
- Studied the three permission types (read, write, execute) and how their meaning differs between files and directories
- Reviewed the sample directory structure (`/`, `/data`, `/data/abc.txt`) used to work through the permission scenarios

**Tuesday - 6.10.2026**
- Worked through the first three permission scenarios:
  - **Scenario 1:** A user can't reach a file, even one they own, if they lack execute permission on a parent directory — always check every directory in the path
  - **Scenario 2:** Read permission on a directory is enough to list its contents with `ls`, but `ls -l` also needs execute permission
  - **Scenario 3:** Deleting a file depends on write and execute permission on the containing directory, not on the file's own permissions

**Wednesday - 7.10.2026**
- Worked through the remaining permission scenarios:
  - **Scenario 4:** Execute permission alone on a directory is enough to access files inside it by path, since read is only needed for listing
  - **Scenario 5:** Access can depend on a user's group memberships, so group membership has to be verified before concluding anything about access
  - **Scenario 6:** Permission checks follow a strict priority — if you own the file, only the owner permissions apply, even if group or other permissions are more generous
- Began **changing permissions** with `chmod` — the symbolic and numeric techniques, the basic syntax, and the requirement to own the file or be root

## Key Takeaways
- Can read and interpret `ls -l` permission strings, including file type and the three permission groups
- Understand that permissions on every parent directory in a path matter, not just the permissions on the target file
- Clear on how read, write, and execute behave differently on directories than on files
- Know that permission checking stops at the first matching category (owner, then group, then other) rather than combining them

## Next Steps
- Continue with the next Linux Essentials Chapters
- Practice setting and testing permissions on files and directories in a virtual machine
