 DIRECTORIES UNDER /:
 -------------------

    In Linux, the `/` directory is known as the root directory.  
    It is the top-level directory in the Linux File System hierarchy.  
    Every file and directory starts here — it is the parent of all directories.

## Key Points About `/` (Root Directory)
- `/` is the base of the entire Linux File System.  
- Everything (files, devices, mounted drives) is located under `/`.  
- Not to be confused with `/root` (which is the home directory of the root user).  

---

## Common Directories Under `/`

| Directory | Description |
|-----------|-------------|
| `/bin`    | Essential binary executables (Ex: ls, cp) |
| `/boot`   | Boot loader files (Ex: vmlinuz, initrd) |
| `/dev`    | Device files (Ex: /dev/sda, /dev/null) |
| `/etc`    | System configuration files |
| `/home`   | User home directories |
| `/lib`    | Essential shared libraries for `/bin` and `/sbin` |
| `/media`  | Mount point for removable media (USB drives) |
| `/mnt`    | Temporary mount point for filesystems |
| `/opt`    | Optional software packages |
| `/proc`   | Virtual filesystem providing process info |
| `/root`   | Home directory of the root user |
| `/run`    | Running system data (Ex: PIDs, sockets) |
| `/sbin`   | System binaries (used by root user) |
| `/srv`    | Data for services (Ex: web servers) |
| `/sys`    | Virtual filesystem related to devices |
| `/tmp`    | Temporary files (auto-cleared) |
| `/usr`    | User programs, libraries, and documentation |
| `/var`    | Variable data like logs, mail, spool files |

---

# BASIC LINUX COMMANDS

```bash
ls                 # Display all files
ls -l              # Display long-listed files
ls -lh             # Files with human-readable sizes
ls -lt             # Files in table format
ls -lr             # Files in reverse order
ls -lrth           # Reverse order, human-readable
ls -lrth directory # View contents of a directory
ls -li             # Files with inode numbers
ls -la             # Show all files including hidden
du -sh filename    # Check file size
du -sh *           # Check sizes of all files
df -hT             # Check disk usage
date               # Check date & time
cat /etc/os-release # Check OS details

AWK COMMAND

Used to extract specific columns from data.

Syntax:
cat filename | awk '{print $1}'



