Command:
--------
    To display the login history of users with full login and logout date and time information.
    EX:-
        last -F

Sticky Bit:
------------
    Sticky Bit is a special permission in Linux that is set on directories to prevent users from deleting files owned by other users inside that directory.
    
    chmod +t directory_name
    chmod 1777 directory_name

What is SUID:
--------------
      SUID is a special permission that allows a user to execute a file with the permissions of the file owner instead of the user who runs it.

How to Identify SUID:
---------------------  
      ls -l file_name

If you see:
------------
     -rwsr-xr-x
     The s in the user execute position indicates SUID.

How to Set SUID
----------------
Numeric method:
---------------
        chmod 4755 file_name

Symbolic method:
----------------
        chmod u+s file_name

What is SGID:
-------------
        SGID is a special permission that allows a file to be executed with the permissions of the file's group.

For directories:
----------------
         Files created inside the directory inherit the group ownership of the directory.
         
How to Identify SGID:
---------------------
        -rwxr-sr-x
         The s in the group execute position indicates SGID.
         
For directories:
----------------
        drwxr-sr-x
        
How to Set SGID:
----------------
Numeric method:
--------------
        chmod 2755 directory_name
        
Symbolic method:
----------------
        chmod g+s directory_name

What is load Average:
---------------------
        load avg is a metric that shows the avg no.of process in the system run queue over 1, 5 and 15min.

What is Swap Memory:
--------------------
        swap memory is a space on the hard disk that is used as virtual memory. when the physical RAM is full. It is as over flow area for RAM.

What is Absolute path:
----------------------
        An absolute path specifies the exact location of a file or directory from the root (/) directory, regardless of the current working directory.

        Ex:-
        ----
            /home/ummar/documents/file.txt


what is Relative Path:
----------------------
        A relative path specifies the location of a file or directory with respect to the current working directory.

       Ex:-
       ---
           /home/ummar

