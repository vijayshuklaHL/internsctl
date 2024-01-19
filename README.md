**NOTE:
internsctl (bash script)
internsctl-man.gz (man file)**

# internsctl
internsctl command tool for linux
written By: Isha Atri


Usage: internsctl [OPTIONS]
Options:
    --help                   Display this help message
    --version                Display version information
    cpu getinfo              Display information about the CPU using lscpu
    memory getinfo           Display information about memory using free
    user create <username>   Create a new user
    user list                List all users
    user list --sudo-only    List only sudo users
    file getinfo [options]   Get information about a file
    --size, -s             Print file size
    --permissions, -p      Print file permissions
    --owner, -o            Print file owner
    --last-modified, -m    Print last modified time


## EXAMPLES
internsctl cpu getinfo
internsctl memory getinfo
internsctl user create john_doe
internsctl user list --sudo-only
internsctl file getinfo --size --permissions example.txt


----------------------------------------------------------
Put the internsctl-man file in /usr/share/man/man1
and run below command,
    $ man internsctl
----------------------------------------------------------

