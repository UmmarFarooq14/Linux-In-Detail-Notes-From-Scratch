 SECURITY & PERMISSIONS:
 -----------------------


UMASK (User Mask):
-----------------

        - umask sets default permissions for new files and directories.
        - Default umask: `0022`
        - Default permissions:  
          - Directories: `755` (rwxr-xr-x)  
          - Files: `644` (rw-r--r--)  

Calculation:
------------

     -- For Directories: 0777 - 0022 = 0755
     -- For Files: 0666 - 0022 = 0644



 PERMISSION TYPES:
 -----------------

    | Permission | Symbol | Value |
    |------------|--------|-------|
    | Read       | r      | 4     |
    | Write      | w      | 2     |
    | Execute    | x      | 1     |


 USER TYPES:
 ----------

    | Symbol | User Type |
    |--------|-----------|
    | u      | User      |
    | g      | Group     |
    | o      | Others    |


 CHANGE PERMISSIONS:
 -------------------


    -- chmod u+x filename   # Add execute permission for user
    -- chmod g-w filename   # Remove write for group
    -- chmod 755 myfile     # rwxr-xr-x

CHANGE OWNERSHIP:
-----------------

-- chown root file.txt          # Change owner
-- chown user:group file.txt    # Change owner and group

CRON JOBS & SCHEDULING:
-----------------------\

-- cron is used to schedule scripts or commands to run at specific times.

CRON JOB FORMAT:
----------------
* * * * * /path/to/command
│ │ │ │ │
│ │ │ │ └── Day of week (0-7) (Sunday=0 or 7)
│ │ │ └──── Month (1-12)
│ │ └────── Day (1-31)
│ └──────── Hour (0-23)
└────────── Minute (0-59)

MANAGING CRON JOBS:
-------------------
-- sudo yum install cronie       # Install cron service
-- crontab -l                    # List cron jobs
-- crontab -e                    # Edit cron jobs
-- crontab -r                    # Remove cron jobs

SPECIAL STRINGS:
-----------------

| String   | Meaning               |
| -------- | --------------------- |
| @reboot  | Run at system startup |
| @daily   | Run once a day        |
| @weekly  | Run once a week       |
| @monthly | Run once a month      |
| @yearly  | Run once a year       |





