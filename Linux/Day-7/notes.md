 PROCESS MANAGEMENT:
 ------------------

      A process is a set of instructions being executed in memory.  

      - PID – Process ID  
      - PPID – Parent Process ID  

 TYPES OF PROCESSES:
 ------------------
 
1. Running Process
   ----------------
   
        Actively executing on the CPU.  
        Example: When you run `top`, it’s running as long as it’s on CPU.

2. Stopping Process:
   -----------------
        Temporarily stopped by a signal.  
        Example: `Ctrl + Z` pauses a process.

3. Sleeping Process:
   -----------------
       Not running, waiting for a resource or event.  
       Example: Waiting for user or file input.

4. Waiting Process:
   ---------------
       Waiting for a resource or event to continue.

5. Zombie Process:
   -------------- 
       A process that has finished execution but still has an entry in the process table.

6. Orphan Process:
   ---------------  
       A running process whose parent has terminated.



 PROCESS COMMANDS:
 -----------------
     -- ps            # Show snapshot of current processes
     -- ps -ef        # Full-format listing with parent-child relation
     -- ps -aux       # Show all processes including daemons

KILL A PROCESS:
---------------
-- kill -9 <PID>
-- Use ps -ef or top to find the PID of the process to kill.

PACKAGE MANAGEMENT:
-------------------
-- Package management refers to installing, upgrading, configuring, and removing software.

| Distribution       | Package Format | Package Manager     |
| ------------------ | -------------- | ------------------- |
| Ubuntu/Debian      | `.deb`         | `apt`, `dpkg`       |
| RHEL/CentOS/Fedora | `.rpm`         | `yum`, `dnf`, `rpm` |
| Arch Linux         | -              | `pacman`            |
| SUSE               | `.rpm`         | `zypper`            |

Difference Between yum & rpm:
----------------------------
| Feature             | yum                         | rpm                         |
| ------------------- | --------------------------- | --------------------------- |
| Full Form           | Yellowdog Updater Modified  | Red Hat Package Manager     |
| Type                | High-level package manager  | Low-level package manager   |
| Dependency Handling | Automatically resolves deps | Doesn’t handle dependencies |
| Data Rollback       | Supports rollback           | No rollback support         |
| Update Support      | Supports package updates    | Limited                     |

Difference Between Hard Link & Soft Link:
-----------------------------------------
| Hard Link                              | Soft Link                          |
| -------------------------------------- | ---------------------------------- |
| Copy of a file (points to same data)   | Shortcut/reference to a file       |
| Works only for files                   | Works for files and directories    |
| Shares same inode as original file     | Has a different inode              |
| Deleting original does NOT affect link | Deleting original breaks soft link |



