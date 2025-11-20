 IMPORTANT PORT NUMBERS:
 ------------------------
 

 | Port Number | Protocol/Service                 | Description                                   |
 |------------|---------------------------------|-----------------------------------------------|
 | 20         | FTP (Data)                      | File Transfer Protocol (Data Channel)         |
 | 21         | FTP (Control)                   | File Transfer Protocol (Control Channel)      |
 | 22         | SSH                             | Secure Shell for remote login                 |
 | 23         | Telnet                          | Remote login (insecure)                       |
 | 25         | SMTP                            | Simple Mail Transfer Protocol                 |
 | 53         | DNS                             | Domain Name System                            |
 | 67, 68     | DHCP                            | Dynamic Host Configuration Protocol           |
 | 80         | HTTP                            | Web traffic                                   |
 | 110        | POP3                            | Post Office Protocol (Receiving mail)         |
 | 123        | NTP                             | Network Time Protocol                         |
 | 143        | IMAP                            | Internet Message Access Protocol              |
 | 161, 162   | SNMP                            | Simple Network Management Protocol            |
 | 389        | LDAP                            | Lightweight Directory Access Protocol         |
 | 443        | HTTPS                           | Secure web traffic                            |
 | 465        | SMTPS                           | SMTP over SSL                                 |
 | 993        | IMAPS                           | IMAP over SSL                                 |
 | 995        | POP3S                           | POP3 over SSL                                 |
 | 3306       | MySQL                           | MySQL database service                        |
 | 3389       | RDP                             | Remote Desktop Protocol                       |
 | 5432       | PostgreSQL                      | PostgreSQL database service                   |
 | 6379       | Redis                           | Redis database                                |
 | 8080       | HTTP (Alternate)                | Alternate HTTP port                           |
 | 9000       | SonarQube, PhpMyAdmin (custom)  | Web-based services                            |
 ------------------------------------------------------------------------------------------------

 DISK MANAGEMENT:
 ----------------

    Disk management includes partitioning, mounting, checking disk usage, and managing storage.



 VIEW DISK INFORMATION:
 ---------------------

    lsblk          # Show all block devices
    fdisk -l       # List all partitions
    parted -l      # Show disk partitions
    df -h          # Check disk usage in human-readable format
    du -sh *       # Check directory/file sizes
    mount          # List mounted filesystems

CREATE A PARTITION:
-------------------
    fdisk /dev/sdb        # Create a partition on /dev/sdb

Steps inside fdisk:
-------------------
-- n  -> New partition
-- p  -> Primary partition
-- 1  -> Partition number
-- +10G -> Size
-- w  -> Write changes

FORMAT PARTITION:
-----------------
-- mkfs.ext4 /dev/sdb1

MOUNT A PARTITION:
------------------

-- mkdir /mnt/data
-- mount /dev/sdb1 /mnt/data

MAKE MOUNT PERMANENT:
---------------------

Edit /etc/fstab:
---------------
-- /dev/sdb1   /mnt/data   ext4   defaults   0   0

SWAP MANAGEMENT:
----------------

-- mkswap /dev/sdb2   # Create swap area
-- swapon /dev/sdb2   # Enable swap
-- swapoff /dev/sdb2  # Disable swap
-- free -m            # Check swap usage





