
To display the login history of users with full login and logout date and time information.

Command:
-------
    last -F

Sticky Bit:
-----------
    Sticky Bit is a special permission in Linux that is set on directories to prevent users from deleting files owned by other users inside that directory.
    
    chmod +t directory_name
    chmod 1777 directory_name

What is SUID:
------------
      SUID is a special permission that allows a user to execute a file with the permissions of the file owner instead of the user who runs it.

How to Identify SUID:
---------------------
      
      ls -l file_name


If you see:
-----------

     -rwsr-xr-x


The s in the user execute position indicates SUID.

How to Set SUID:
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
