at command:
-----------
    at command is like crontab which allows you to schedule jobs buts only once.
    when the command is run it will enter interactive mode & you can get out by pressing ctrl + D.

Usage:
-----

    at HH:MM PM           ---> schedule a job.
    at q                  ---> list the at entries
    at rm #               ---> remove at entry
    at d                  ---> at daemon/service that manages scheduling.
    systemctl status atd  ---> To manage atd services.

Schedule at :
------------

    create at entry by scheduling a task:
       at 4:45 PM ---> enter
       echo "This is my first entry" > at_entry
