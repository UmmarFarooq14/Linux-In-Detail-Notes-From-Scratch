 FILE SYSTEMS:
 -------------

      You can create files in Linux using two main commands:  
      1. `touch`  
      2. `vim` or `vi` Editor  



  touch Command:
  --------------

       Create files quickly without opening an editor.

Syntax:
-------

    touch filename                   # Create a single file
    touch filename1 filename2        # Create multiple files
    touch filename{1..5}             # Create multiple numbered files

 cat Command
 ------------

   Insert/view content in files.
   
Syntax:
------
   cat > filename1               # Insert single-line data
   cat >> filename1              # Insert multiple lines
   cat filename1                 # View content
   cat file1 > file2             # Overwrite file2 with file1
   cat file1 >> file2            # Append file1 content to file2


3) VI / VIM EDITOR
   ----------------
vi or vim allows creating and editing large files.

Syntax:
--------
vim filename

Steps:
--------

> Open file: vim filename
> Press i to enter INSERT mode.
> Type your content.
> Press Esc to exit INSERT mode.
> Save and exit: :wq!

Useful vi/vim Commands:
------------------------

> :set num      # Show line numbers
> :set nonum    # Hide line numbers
> :645          # Go to line 645
> dd            # Delete current line
> :%d           # Delete all lines
> :/word        # Search word (top to bottom)
> :?word        # Search word (bottom to top)
> :3s/old/new   # Replace in line 3
> :%s/old/new   # Replace all


CREATE DIRECTORIES
-------------------

> mkdir dir1              # Create a directory
> mkdir -v dir1           # Verbose mode
> mkdir -p parent/child   # Create nested directories
> ls -lrth dir1/          # Show contents


TREE COMMAND
-------------

> To see directory structure:

> yum install tree -y
> tree
