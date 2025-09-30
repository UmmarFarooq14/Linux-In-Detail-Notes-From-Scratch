
# LINUX DOCUMENTATION
  -------------------

    There are two essential tools for finding help and understanding how commands work in detail.

1) Manual Pages (man)
   -----------------   
   

  Syntax:
  -------
     man [command name]
Example:
--------
    Copy code
    man ls     # Shows the manual for the 'ls' command
    
Common Manual Page Sections:
----------------------------

    NAME - What the command does
    
    SYNOPSIS - How to use it (Syntax)
    
    DESCRIPTION - Detailed explanation
    
    OPTIONS - List of flags/switches
    
    EXAMPLES - Sample usage
    
    SEE ALSO - Related commands

 ## 2) --help:
-------------

    Prints a quick summary of options and usage for a command.

Syntax:
-------

    command --help
    
Example:
-------

    ls --help   # Shows all available flags for 'ls'

Difference Between man & help

|Feature	          | man (manual)	             | --help (quick help)      |
|-------------------------------------------------------------------------  |
|Detail	             Very detailed (official)	    Quick & concise           |
|                                                                           |
|Internet Needed	    No	                        No                          |
|                                                                           |
|Formatting	         Paginated,                  organized	Plain text      |
|                                                                           |
|Ideal Use Case	     Deep understanding	        Quick usage/flag reference  |
----------------------------------------------------------------------------
