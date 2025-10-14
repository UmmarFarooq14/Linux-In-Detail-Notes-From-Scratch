USER & GROUP MANAGEMENT:
------------------------

    When joining a new organization, you often create users, add them to groups, and assign permissions.


## USER CREATION


useradd -c "role" username   # Create a user with a comment
passwd username              # Set password for a user


Example:
--------
useradd -c "software" suresh

DELETE A USER:
--------------
userdel -r username   # Delete a user and their home directory

VIEW USERS:
-----------
cat /etc/passwd

VIEW PASSWORDS (hashed):
------------------------
cat /etc/shadow

GROUP MANAGEMENT:
----------------
groupadd groupname

Delete a Group:
--------------
groupdel groupname

View Groups:
------------
cat /etc/group

ADD/REMOVE USER TO GROUP:
-------------------------
> usermod -aG groupname username   # Add user to group
> gpasswd -d username groupname    # Remove user from group


VIEW GROUP PASSWORDS:
---------------------
cat /etc/gshadow

LOCK/UNLOCK USER:
----------------
usermod -L username   # Lock user
usermod -U username   # Unlock user

ENABLE SSH LOGIN FOR USER:
--------------------------
vim /etc/ssh/sshd_config
# Go to line 63, set "PasswordAuthentication yes"
> :wq!

GIVE SUDO ACCESS:
-----------------
visudo
# Add the user under User Privileges
> username   ALL=(ALL)   ALL



