# Linux Cheatsheet for Ubuntu Server

This cheatsheet is a quick reference for common Linux commands on Ubuntu Server. It covers basic operations, system administration, networking, and more. Use it as a handy reference when working with Linux commands on Ubuntu Server.

## Navigation

- `pwd`: Display the name of the current working directory.
- `cd <directory>`: Change the current working directory.
- `ls`: List the files and directories in the current working directory.

## File management

- `touch <file>`: Create a new, empty file.
- `rm <file>`: Remove a file.
- `rm -r <directory>`: Remove a directory and all of its contents.
- `cp <source> <destination>`: Copy a file or directory.
- `mv <source> <destination>`: Move a file or directory.

## File content

- `cat <file>`: Display the contents of a file.
- `less <file>`: Display the contents of a file one page at a time.

## Process management

- `top`: Display real-time information about the processes running on the system, including the CPU and memory usage of each process.
- `ps`: Display information about the processes running on the system.
- `kill <pid>`: Terminate the process with the specified process ID (PID).

## Package management

- `apt update`: Update the list of available packages and their versions.
- `apt upgrade`: Upgrade installed packages to their latest versions.
- `apt install <package>`: Install a new package.
- `apt remove <package>`: Remove an installed package.

## Text editing

- `nano <file>`: Edit the specified file using the Nano text editor.
- `vi <file>`: Edit the specified file using the Vi text editor.

## Archive management

- `tar -cvf <archive>.tar <files>`: Create a tar archive containing the specified files.
- `tar -xvf <archive>.tar`: Extract the files from a tar archive.
- `gzip <file>`: Compress a file using gzip.
- `gunzip <file>.gz`: Decompress a file that was compressed using gzip.

## Network configuration

- `ifconfig`: Display the network configuration for all network interfaces.
- `ping <host>`: Send a test packet to a network host to see if it is reachable.

## System information

- `uname -a`: Display information about the current system, including the kernel version and machine hardware name.
- `uptime`: Display the amount of time that the system has been running.
- `free -m`: Display the amount of free and used memory in the system, in megabytes.
- `df -h`: Display the amount of free and used space on the system's disk drives, in human-readable format.

## Users and groups

- `whoami`: Display the current user's username.
- `id`: Display information about the current user, including the user's UID and primary group.
- `groupadd <group>`: Create a new group.
- `useradd <user>`: Create a new user.
- `usermod -a -G <group> <user>`: Add a user to a group.

## Permissions

- `chmod <permissions> <file>`: Change the permissions of a file.
- `chown <user>:<group> <file>`: Change the owner and group of a file.

## Searching

- `grep <pattern> <files>`: Search for a pattern in one or more files.
- `find <path> <expression>`: Search for files matching a specified expression.

## Environment variables

- `echo $<variable>`: Display the value of an environment variable.
- `export <variable>=<value>`: Set the value of an environment variable.

## Compression

- `bzip2 <file>`: Compress a file using bzip2.
- `bunzip2 <file>.bz2`: Decompress a file that was compressed using bzip2.
- `xz <file>`: Compress a file using xz.
- `unxz <file>.xz`: Decompress a file that was compressed using xz.

## Printing

- `lpr <file>`: Print a file.
- `lpq`: Display the status of the print queue.

## System log

- `tail -f /var/log/syslog`: Display the contents of the syslog in real time.

## Archiving and backup

- `dd if=<input_file> of=<output_file>`: Create an exact copy of a file.
- `tar -czvf <archive>.tar.gz <files>`: Create a tar archive and compress it with gzip.
- `tar -czvf <archive>.tar.bz2 <files>`: Create a tar archive and compress it with bzip2.

## Remote access

- `ssh <user>@<host>`: Connect to a remote host using SSH.
- `scp <source> <user>@<host>:<destination>`: Copy a file to a remote host using SCP.

## Text processing

- `sort <file>`: Sort the lines of a file.
- `uniq <file>`: Remove duplicate lines from a file.
- `wc <file>`: Count the number of lines, words, and characters in a file.

## Systemd service management

- `systemctl start <service>`: Start a Systemd service.
- `systemctl stop <service>`: Stop a Systemd service.
- `systemctl restart <service>`: Restart a Systemd service.
- `systemctl status <service>`: Display the status of a Systemd service.

## Networking

- `ip link`: Display information about the system's network interfaces.
- `ip addr`: Display information about the system's network addresses.
- `ip route`: Display the system's routing table.
- `ip neigh`: Display the system's neighbor cache (i.e., the mapping of IP addresses to MAC addresses).

## Processes

- `nice <command>`: Run a command with a lower priority.
- `renice <priority> -p <pid>`: Change the priority of an existing process.

## Scheduling tasks

- `at <time>`: Schedule a command to be executed at a specified time.
- `crontab -e`: Edit the current user's crontab file (used to schedule recurring tasks).

## System monitoring

- `vmstat`: Display information about the system's memory, processes, and swap space.
- `mpstat`: Display information about the system's processors.
- `iostat`: Display statistics about the system's input/output performance.
- `sar`: Collect and display system activity information.

## Text manipulation

- `cut -d <delimiter> -f <field> <file>`: Extract a field from a file that is delimited by a specified character.
- `sed 's/<pattern>/<replacement>/' <file>`: Replace a pattern in a file with a specified string.

## Security

- `ssh-keygen`: Generate a new SSH key pair.
- `chpasswd`: Change the password for a user.

## Performance monitoring

- `uptime`: Display the system's uptime (i.e., the amount of time it has been running).
- `top`: Display information about the processes running on the system, including the CPU and memory usage of each process.
- `ps aux`: Display a detailed list of processes running on the system.
- `free -m`: Display information about the system's memory usage, including the amount of free and used memory.
- `iostat -x`: Display extended statistics about the system's input/output performance.
- `mpstat -P ALL`: Display information about the utilization of each CPU on the system.
- `sar -u`: Collect and display information about the CPU utilization on the system.

## System configuration

- `dpkg -l`: List the packages installed on the system.
- `dpkg -L <package>`: List the files installed by a package.
- `update-alternatives --config <name>`: Select a configuration for an alternative (i.e., a program that provides multiple versions of a command).

## File system

- `fsck <device>`: Check a file system for errors and repair any that are found.
- `tune2fs <device>`: Modify the parameters of an ext2 or ext3 file system.
- `mount`: Display the currently mounted file systems.
- `umount <device>`: Unmount a file system.
- `fdisk -l`: Display the partition table for the system's disk drives.

## Miscellaneous

- `alias <alias>='<command>'`: Create an alias for a command.
- `history`: Display a history of recently executed commands.
- `cal`: Display a calendar.
- `nohup <command> &`: Run a command in the background and allow it to continue running after the terminal is closed.
- `tar -czvf <archive>.tar.xz <files>`: Create a tar archive and compress it with xz.
- `time <command>`: Measure the amount of time it takes to run a command.
- `whois <domain>`: Look up information about a domain name.
- `tee <file>`: Redirect the output of a command to both the terminal and a file.
- `watch <command>`: Execute a command repeatedly and display the output.
- `which <command>`: Display the path of the executable file associated with a command.
- `time <command>`: Measure the amount of time it takes to run a command.
