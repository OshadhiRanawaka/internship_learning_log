# Progress Log 22

## Overview
Continuing the Learning Week during my Fullstack Developer Internship at ProLab R, I finished the special permissions section and worked through file links in the **NDG Linux Essentials** course.

## Resource
- **Course:** NDG Linux Essentials
- **Topics Covered:** Setgid on directories, the sticky bit, hard links and symbolic links

## Daily Progress Log

**Monday - 12.10.2026**
- Learned how **setgid on a directory** makes new files take the directory's group instead of the creator's primary group, and that new subdirectories inherit setgid too
- Learned to spot it with `ls -ld`, where a lowercase `s` in the group execute position means setgid and group execute are both set, and an uppercase `S` means setgid is set but not in effect
- Worked through the shared project directory example, where `bob`, `sue` and `tim` from different primary groups need a shared `/home/team` directory, and setgid lets them all access each other's files through the `team` group
- Covered how to **set and remove setgid** with `chmod`, using `g+s` and `g-s` symbolically or adding and subtracting 2000 numerically

**Tuesday - 13.10.2026**
- Studied the **sticky bit**, which stops users from deleting files they don't own in a shared directory. Only the file's owner or root can delete a file in such a directory
- Saw it in use on `/tmp` and `/var/tmp`, and learned to spot it in `ls -l` as a `t` in the others' execute position. A lowercase `t` means sticky and execute are both set, and an uppercase `T` means only the sticky bit is set
- Learned to set and remove it with `o+t` and `o-t`, or by adding and subtracting 1000 numerically
- Began **links** with the problem they solve: reaching a deeply buried file that other people update often, where a copy won't work. The two methods are hard links and symbolic links

**Wednesday - 14.10.2026**
- Learned **hard links** by looking at how the filesystem tracks files: an inode holds the metadata and data block pointers but not the file name, and directories store the name-to-inode association. A hard link is two names pointing to the same inode
- Used `ls -i` to see inode numbers, `ls -li` to see the link count, and `ln target link_name` to create a hard link
- Learned **symbolic links**, which are files that point to another file by path, created with `ln -s`. They show up as an `l` file type with an arrow to the target in `ls -l`
- Compared the two methods:
  - Hard links have no single point of failure, but soft links break if the original is deleted
  - Soft links are easier to see, while hard links need `find -inum` to locate
  - Soft links can cross filesystems, while hard links can't because inode numbers are per filesystem
  - Soft links can point to directories, while hard links to directories aren't allowed

## Key Takeaways
- Understand how setgid on directories and the sticky bit support safe file sharing among multiple users
- Can read the `s`/`S` and `t`/`T` indicators in `ls -l` output and set or remove the special permissions with `chmod`
- Understand how inodes work and why a hard link is a second name for the same file, rather than a pointer to it
- Know when to choose a hard link and when to choose a symbolic link, based on each method's strengths and limits

## Next Steps
- Continue into the Chapter lab test and quiz for chapter 18. Completing the course feedback.
- Practice creating and comparing hard and symbolic links hands-on in a virtual machine
