
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
    Several key combinations on your keyboard usually have a special effect on the terminal.
    
    These "control" CTRL keys are accomplished by holding the CTRL key while typing the second key.

    Ex:-
        CTRL -c means to hold the CTRL key while you type the letter "c".
    
    The most common keys are listed below:
    
        * CTRL -u  --> erase everything you have typed on the command line.
        * CTRL -c  --> stop/kill a command.
        * CTRL -z  --> Suspend a command.
        * CTRL -d  --> exit from interactive program (signals end of data).

Environmental Variable:
-----------------------
    what is environment variables:
    ------------------------------
    
    An environment variable is a dynamic-named value that can affect the way running processes will behave on a cpomputer. They are part of the environment in which ta process runs.

    --> In Simple words, set of defined rules and values to build an environment.

    * To View all environment variables:
        . printenv (or) env

    * To view one environment varibales
        . echo $SHELL

    * To set the environment variables:
        . export Tes = 1
        . echo $Test

    * To set environment variable permanently:

        . vi .bashrc
        . Test = '123'
        . export Test
  
The Screen Command:
-------------------

    * To split the screen into two parts:
        . alt+a
          shift+|
    * To Split half into first first part:
        . alt+a
          shift+s
    * To move cursor from first half to second half:
        . alt +a
          tab
    * To get terminal & IP address:
        . alt+a
          c
    * screen -r ---> to display the how many screens.

Aliases:
-------
    Aliases is a popular command that is used to cut down on lengthy & repetitive commands.
    Ex:-
       * alias ls="ls -la"
       * alias pl="pwd; ls"
       * alias tell="whoami; hostname; pwd"
       * alias dir="ls -l | grep ^d"
       * alias lmar="la -l | gerp mar"
       * alias wpa="chmod a+w"
       * alias d="df -h | awk '{ print \$6 }' | cut -cl -u"

Creating User (or) Global aliases:
----------------------------------
      -->  User = Applies only to a specific user profile.
      --> Global = Applies to everyone who has account on the system.
      
          ==> User = /home/user/.bashrc
          ==> Global = /etc/bashrc
              ==> alias hh = "hostname"

To Display the Image:-
---------------------

    . Become root.
    . Yum install ImageMagick -y
    . display image -file.


Dynamic Host COnfiguration Protocal{DHCP}:-
-----------------------------------------
    Port:
    ----
    DHCP {server} = 67
    DHCP {Client} = 68

    => In order to communicate over the network, a computer needs to have an IP address.
    => DHCP server is responsible to automatically assign IP address to servers desktops, and other devices on the network.

    . How Ips are assigned in corporate world?
    => Dedicated routers run DHCP service to assign Tps on the network.

    Steps by step Instruction:-
    --------------------------
    -> Pick a server to be your DHCP and take a snapshot.
    -> Assign z static IP to the DHCP server.
        -> vi /etc/sysconfig/network/enp0s3.
        -> simply run nmtui command to use GUI based network tool.
    
    
 System Run Levels:-
 -------------------
     Main Run Level:
     ---------------
         0 --> shut down (or) halt of the system.
         1 --> Single-user mode, usually aliased as s/S.
         6 --> Reboot the system.

     Other run levels:
     -----------------
         2 --> Multi-user mode without Networking.
         3 --> Multi-user mode with Networking.
         5 --> Multi-user mode with Networking and GUI.
     

 Linux Boot Process:
 -------------------
    BIOS --> Basic I/p O/P system Executes MBR.
    MBR --> Master Boot Record Executes GRUB.
    GRUB --> Grand Unified BootLoader Execute Kernel.
    Kernel --> Kernel Executes /sbin/init.
    Init --> Init Executes the runlevel Programming.
    RunLevel --> RunLevel Programs are Executed.


Disk Partiiton:
---------------
    Commands for disk partiton:
        . df
        . fdisk
    
Add Disk & Create LVM Partition:
--------------------------------

    . File System 
    . Logical Volume
    . Volume Group
    . Physical Group
    . Partitions
    . Hard Links

What is Swap:
-------------
    Swap Space in Linux is used when the amount of physical memory (RAM) is full. If the system needs more memory resources and the (RAM) is full, inactive pages in memory are moved to the swap space. while swap space can help machines with a small amount of RAM.


Network File System{NFS}:
-------------------------
    -> NFS stands for Network File System, a file system developed by sun Microsystems Inc.
    -> Port number is 2049.
    -> It is a client/server system that allows user to access files across a network and treat them as if they resided in a local file directory.


Samba {136, 137, 138, 445}:-
---------------------------
    -> Samba is a linux tool (or) utility that allows sharing for linux resources such as files and printers to with other operating systems.
    -> It works exactly like NFS but the difference is NFS shares within linux (or) Unix like system whereas Samba with Other OS.
    Ex:- "A" Shares its filesystem with Computer "B" using samba than computer "B" will see that shared filesystem as if it is mounted as the local system.


SATA & SAS:
-----------
    SATA --> Serial Advanced Technology Attachment.
    SAS --> Serial Attachment SCSI { Small Computer System Interface }.
    Both SAS & SATA utilize serial communication.
    
    
    
    
