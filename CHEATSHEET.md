# Bash Cheatsheet for Ubuntu Server

This cheatsheet is a quick reference for common Bash commands on Ubuntu Server. It covers basic operations, system administration, networking, and more. Use it as a handy reference when working with Bash on Ubuntu Server.

## Basic Commands
- `cd <directory>`: Change the current directory to `<directory>`
- `ls [-alh] <directory>`: List directory contents, including hidden files (`-a`), long format (`-l`), and human-readable sizes (`-h`)
- `pwd`: Print the current working directory
- `echo <message>`: Display the `<message>`
- `cat <file>`: Concatenate the contents of `<file>` and print to standard output
- `touch <file>`: Create an empty file or update the timestamp of `<file>`
- `cp <source> <destination>`: Copy `<source>` to `<destination>`
- `mv <source> <destination>`: Move `<source>` to `<destination>`
- `rm <file>`: Remove `<file>`
- `mkdir <directory>`: Create a new directory `<directory>`
- `rmdir <directory>`: Remove the empty directory `<directory>`
- `ln [-s] <source> <destination>`: Create a link to `<source>` at `<destination>`, with a symbolic link (`-s`)

## System Administration
- `sudo <command>`: Execute `<command>` with superuser privileges
- `apt-get <command>`: Package manager for installing, updating, and removing software
- `systemctl <command>`: Control the system manager, including starting and stopping services (`start`, `stop`, `restart`), enabling and disabling services on boot (`enable`, `disable`), and checking the status of services (`status`)
- `top`: Display top users of system resources
- `df [-h]`: Display free disk space, with human-readable sizes (`-h`)
- `free [-h]`: Display amount of free and used memory, with human-readable sizes (`-h`)
- `uptime`: Display how long the system has been running
- `ps [-aux]`: Display active processes, including all processes
- `kill <pid>`: Terminate the process with the specified process ID (`<pid>`)
- `killall <process>`: Terminate all processes with the specified name (`<process>`)
- `shutdown [-h] [-r] [-k] [-t sec] <time>`: Shut down the system, with options for halting (`-h`), rebooting (`-r`), only sending a warning (`-k`), waiting a specified number of seconds (`-t`) before shutdown, and specifying the time of shutdown (`<time>`)
- `reboot`: Reboot the system

## Networking
- `ifconfig`: Display network interface configurations
- `ip <command>`: Display and manipulate IP address and routing information
- `ping <host>`: Test connectivity to `<host>`
- `traceroute <host>`: Trace the path to `<host>`
- `host <name>`: Query DNS name servers for `<name>`
- `nslookup <name>`: Query DNS name servers for information about `<name>`
- `telnet <host> <port>`: Connect to `<host>` on `<port>` using the Telnet protocol
- `ssh <user>@<host>`: Connect to `<host>` as `<user>` using the Secure Shell (SSH) protocol
- `ftp <host>`: Connect to `<host>` using the File Transfer Protocol
- - - `wget <url>`: Download a file from `<url>`
- `curl <url>`: Transfer data from or to a server using `<url>`

## Process Management
- `fg <job>`: Bring a background job to the foreground
- `bg <job>`: Send a background job to the background
- `jobs`: List all jobs in the current shell

## Shell Features
- `history`: Display command history
- `!!`: Execute the previous command
- `!<number>`: Execute the command with the specified history number
- `!<string>`: Execute the most recent command starting with `<string>`
- `<command> | <command>`: Pipe the output of `<command>` to `<command>`
- `<command> && <command>`: Execute `<command>` if `<command>` is successful
- `<command> || <command>`: Execute `<command>` if `<command>` is unsuccessful
- `<command> &`: Run `<command>` in the background
- `<command> > <file>`: Redirect output of `<command>` to `<file>`
- `<command> < <file>`: Redirect input of `<command>` from `<file>`
- `<command> >> <file>`: Append output of `<command>` to `<file>`
- `alias <name>='<command>'`: Create an alias for `<command>` called `<name>`
- `unalias <name>`: Remove the alias `<name>`
- `source <file>`: Execute the commands in `<file>` in the current shell
- `. <file>`: Same as `source <file>`
- `exec <command>`: Execute `<command>` in place of the current shell
- `exit`: Exit the current shell

## Variables
- `<variable>=<value>`: Set the value of `<variable>` to `<value>`
- `echo $<variable>`: Display the value of `<variable>`
- `export <variable>`: Mark `<variable>` for export to child processes
- `unset <variable>`: Remove the value of `<variable>`
