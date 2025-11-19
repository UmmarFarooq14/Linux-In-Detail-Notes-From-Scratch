To Display Hostname with Ip Address:
------------------------------------
Command:
--------
    hostname -i
    hostname -I

To Display only IP Address:
---------------------------
    if config
        
If u want to display since how many weeks ur logging in server:
--------------------------------------------------------------
    uptime -p

If u want to display in date format since loggingin server:
-----------------------------------------------------------
    uptime -s


If I want to see the live crontab generate result:
--------------------------------------------------

    watch cat filename

Tee Command:
------------
    Tee command is used to store and view (both at the same time) the output of any command.
    
command:
--------
    echo "enter the content" | tee filename
    
Scenario:
---------
    If we want to append multiple lines into the file using a tee command the we use command
    
    command:
    --------
    echo "enter the content" | tee -a filename
    
Pipes:
------
    Pipes is used by the shell to connect the output of one command dircetly to the input of the another command.
