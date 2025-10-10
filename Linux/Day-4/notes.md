 SYSTEM MONITORING & PERFORMANCE:
 ---------------------------------


    top          # Real-time process & resource usage
    htop         # Interactive version of top
    vmstat       # Memory, process, I/O stats
    sar          # CPU utilization, loads (System Activity Report)
    free -m      # RAM usage in MB
    df -h        # Disk usage in human-readable format
    who          # Show logged-in users
    whoami       # Show current user with date and time
    uptime       # System uptime
    last         # User login history since system start
    lscpu        # CPU information
    uname -r     # Kernel version

NETWORKING COMMANDS:
-------------------

    ip a                  # Check private IP address
    curl ipinfo.io        # Get public IP address
    curl ipconfig.io      # Get public IP address
    ping google.com       # Test network connectivity
    traceroute google.com # Trace path packets take
    nslookup google.com   # DNS resolution
    dig google.com        # Detailed DNS information
    netstat -tulnp        # List listening ports
    wget https://example.com # Download data from web
    curl https://example.com # View web content

GREP COMMANDS:
-------------

    grep -i "word" filename       # Search word (case-insensitive)
    grep -in "word" filename      # Search word, show line numbers
    grep -ic "word" filename      # Count matches
    grep -r "word" directory      # Search recursively in directory
    grep -iv "word" filename      # Show lines NOT matching
    grep -w "word" filename       # Match whole word
    grep -il "word" filename      # Show only filenames
    grep -iA5 "word" filename     # Show 5 lines after match
    grep -iB5 "word" filename     # Show 5 lines before match
    grep -iC5 "word" filename     # Show 5 lines before & after
    grep -iE "dog|cat" filename   # Match multiple patterns
    grep -i "^word" filename      # Match lines starting with "word"
    grep -i "word$" filename      # Match lines ending with "word"


WORD COUNT (wc):
---------------
    wc filename    # Count lines, words, characters
    wc -l filename # Count lines
    wc -c filename # Count characters
    wc -w filename # Count words


FIND COMMAND
-------------

-- The find command searches for files/directories recursively based on name, size, type, time, etc.

| Purpose                        | Command                         |
| ------------------------------ | ------------------------------- |
| Find all files                 | `find . -type f`                |
| Find all directories           | `find . -type d`                |
| Find by path                   | `find /path -name filename.txt` |
| Case-insensitive search        | `find . -iname readme.md`       |
| Find by extension              | `find . -name "*.log"`          |
| Find empty files               | `find . -type f -empty`         |
| Find empty directories         | `find . -type d -empty`         |
| Find files >10MB               | `find . -type f -size +10M`     |
| Modified in last 1 day         | `find . -mtime -1`              |
| Delete files older than 1 day  | `find . -mtime +1 -delete`      |
| Accessed more than 30 days ago | `find . -atime +30`             |
| Search entire system           | `find / -name filename`         |
