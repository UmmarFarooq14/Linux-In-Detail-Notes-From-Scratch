 LINUX KERNEL SYSTEM:
 --------------------

        -- The Linux Kernel is the core component of the Linux operating system.  
        -- It acts as a bridge between hardware and software, managing system resources and services.



 TYPES OF KERNELS:
 -----------------

      | Type               | Description                                             |
      |--------------------|---------------------------------------------------------|
      | Monolithic Kernel  | Entire OS runs in a single address space (Linux uses this) |
      | Microkernel        | Minimal services in kernel space; rest in user space    |
      | Hybrid Kernel      | Mix of monolithic and microkernel (e.g., Windows NT)    

 MAIN RESPONSIBILITIES:
 ----------------------

    | Function                | Description                                         |
    |------------------------|-----------------------------------------------------|
    | Process Management      | Schedule processes, manage multitasking, priorities|
    | Memory Management       | Handle RAM allocation, virtual memory, swap        |
    | File System Management  | Manage read/write, permissions, mount points       |
    | Device Management       | Use drivers to interact with hardware              |
    | Networking              | Enable communication between systems               |
    | Security                | Manage permissions, system calls, SELinux          |



 KERNEL COMPONENTS:
 ------------------

     1. **Process Scheduler** – Controls execution of processes  
     2. **Memory Manager** – Allocates and frees memory  
     3. **Virtual File System (VFS)** – Interface for different file systems  
     4. **Device Drivers** – Connect kernel with hardware  
     5. **Network Stack** – TCP/IP handling  
     6. **System Call Interface (SCI)** – API for user apps to interact with kernel



 BACKUP & RECOVERY:
 -----------------

    -- Backup: A copy of data stored elsewhere to protect against data loss due to  
    -- hardware failure, human error, malware, or accidental deletion.



 TYPES OF BACKUPS:
 -----------------

     | Type                | Description                                                    |
     |---------------------|----------------------------------------------------------------|
     | Full Backup         | Backs up all data every time. Time-consuming, storage-heavy.   |
     | Incremental Backup  | Backs up changes since last backup (full or incremental).      |
     | Differential Backup | Backs up changes since last full backup.                       |
     | Remote Backup       | Backup to remote server/cloud (e.g., rsync, scp).              |



 COMMON BACKUP TOOLS:
 --------------------

    | Tool         | Use Case                 | Description                                |
    |-------------|-------------------------|--------------------------------------------|
    | cp          | Simple copies           | Copy files/directories                     |
    | rsync       | Sync/backup             | Fast incremental backup                    |
    | tar         | Archiving               | Create compressed archives                |
    | dd          | Disk imaging            | Bit-by-bit disk backup                    |
    | scp/sftp    | Remote backups          | Copy files over SSH                       |
    | cron+script | Automation              | Schedule backups                          |
    | dump/restore| Ext filesystem backups  | Backup ext2/ext3/ext4                     |
    | Timeshift   | System restore          | Desktop backup utility                    |
    | Bacula, Amanda, BackupPC | Enterprise backup software | Advanced solutions |



 BACKUP EXAMPLES:
 ----------------

 Using `tar`:
 ------------
 
     -- tar -cvpzf /backup/home_backup.tar.gz /home
     -- c=create, v=verbose, p=preserve perms, z=gzip, f=filename

Using rsync:
------------

      rsync -avh /home/ /backup/home/
      -- a=archive, v=verbose, h=human-readable

Remote Backup via scp:
---------------------

     -- scp -r /var/log user@192.168.1.10:/backup/logs/

RECOVERY EXAMPLES:
-------------------
Restore using tar:
-----------------

    -- tar -xvpzf /backup/home_backup.tar.gz -C /

Restore using rsync:
--------------------

    -- rsync -avh /backup/home/ /home/

BACKUP BEST PRACTICES:
----------------------

-- Use incremental/differential backups to save space.
-- Store backups in multiple locations (local + cloud).
-- Automate backups using cron and scripts.
-- Secure backups with encryption.
-- Test backups regularly.


