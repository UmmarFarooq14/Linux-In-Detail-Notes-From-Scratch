Access Control List {ACL}:
--------------------------
    Access control provides an additional, more flexible permission mechanism for file systems.It is designed to assist with UNIX file permission.ACL allows you to give  permissions for any user to group to any disc resources.

USE:
----
    Think of a scenario in which a particular user is not a member of group created by you but still you want to give some read (or) write access, how can you do it without making user a member of group, here comes in picture access control lists, ACL help us to do the trick.
    
    Basically, ACLs are used to make a flexible permission mechanism in linux.

Commands to assign and  remove ACL Permission are:
--------------------------------------------------
    setfacl
    getfacl

List of commands for setting up ACL:
------------------------------------
    1) To add permission for user:
       setfacl -m u:user: rwx /path/to/file
       
    2) To add permission for group:
       setfacl -m g:group: rw /path/to/file

    3) To allow all files (or) dir to inherit ACL entries from the dir it is within:
       setfacl -dm "entry" /path/to/file
       
      
