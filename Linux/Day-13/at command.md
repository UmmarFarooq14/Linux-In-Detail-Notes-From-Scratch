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

other future scheduling format:
-------------------------------

    at 2:45 AM 101621            ---> schedule a job to run on oct 16th, 2021 at 2:45 AM.
    at 4PM + 4 days              ---> schedule a job at 4PM four days from now.
    at now + 5 hours             ---> schedule a job to run five hours from now.
    at 8:00 AM Sun               ---> schedule a job at 8am on coming sunday.
    at 10:00 AM next month       ---> schedule a job to 10am on next month.

System Monitoring:
------------------
    Top
    df
    dmesg
    iostat
    netstat -ip & ss
    free
    cat /proc/cpuinfo
    cat /proc/meminfo
    htop
    vmstat
    sar

Log Monitoring:
---------------
    Another and most important way of system administration is log monitor.
    
    log directory = /var/log
    boot
    chronyd = NTP
    cron
    mailog
    secure
    messages
    httpd
    
SOS Report:
-----------
    what is sos report:
     collect and package diagnostic and support data.
     
    Package name:
     sos-version

    command:
     sosreport
     
Terminal Control Keys:
----------------------
