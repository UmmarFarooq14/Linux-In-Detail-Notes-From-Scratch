To Display Hostname with Ip Address:-
------------------------------------
Command:-
--------
    hostname -i
    hostname -I

To Display only IP Address:-
---------------------------
    if config
        
If u want to display since how many weeks ur logging in server:-
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
    The symbol for a pipe is the vertical bar (|). The command syntax is:
    
    command [argument1] | command2 [argument2]
    
Execution of multiple commands:
-------------------------------
    Execution of multiple commands in a single line using semi-colon (;) 
commands:
---------
    echo "Hello" ; echo "World"
    mkdir test_dir; cd test_dir; touch "test file.txt"

Trunacate file size:
--------------------

    The Linux truncate command is often used to shrink or extend the size of a file to a specified size.
    
    command:
    --------
    truncate -s 20 filename

Combining & Spliting files:
---------------------------
    Multiple files can be combined into one and one file can be split into multiple files.

    cat file1 file2 file3 > file4
    split file4 
    split -l 2 file4 newcreated-filename
