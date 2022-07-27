# Unix/Linux

## Concepts

- **Command Prompt**: Short text at the start of the command line followed by a prompt symbol. The first part is the username followed by the hostname and last the prompt symbol.
- `Ctrl + C` : Brings your prompt back if stuck.
- Linux has a super-user account call **root**. The root has permission to modify everything.
- Linux is **case sensitive**.
- Avoid using spaces when creating files and directories.
- _Linux filesystem_ store information in a hierarchy of directories and files.
- Absolute path: always starts with a "/". This idicates that the path starts at root directory.
- Relative path: It identifies a location relative to your position.
- Wild cards:
  - \* - represents zero or more characters.
  - ? \- represents a single character.
  - [] \- represents a range of characters.
- Inode = Pointer or number of a file on the hard disk.
- Soft Link = Link that will be removed if file is removed or renamed.
- Hard Link = Deleting renaming or moving the original file will not affect the hard link.
- Note about links: You cannot create soft or hard links within the same directory with the same name.
- Commands typically have syntax:
  - Command option(s) argument(s).
- UNIX is a multi-user system. Every file and directory in your account can be protected from or made accesible to other users by changing its access permissions. Every user has responsability for controlling access to their files.
- Permission for a file or directory may be restricted to by types.
- There are 3 types of permission:
  - r \- read
  - w \- write
  - x \- execute
- Each permission (rxw) can be controlled at 3 levels:
  - u \- user = yourself
  - g \- group = can be people in the same project.
  - o \- other = everyone in the system.
- Access Control List (ACL) provides an additional, more flexible permission mechanism for file systems.
- ACL allows you to give permissions for any user or group to any disc resource.
- **Evniroment Variables** are a set of defined rules and values to build an environment.
- NIC = Network interface card.
- Network Manager = Service that provides set of tools designed specifically to make it easier to manage networks.
- FTP = File Transfer Protocol is a standard newtwork protocol used for the transfer of files between client and server. Default port 21.
- SCP = Secure Transfer Protocol. Port 22.
- rsync = Utility for efficiently transferring and synchronizing files within the same computer or to a remote computer by comparing the modification time and size of files.
- DNS = Domain Name System.
- NTP = Network Time Protocol.
- Chronyd = Time Sync Protocol better than NTP.
- Timedatectl = Time Sync Protocol better than Chronyd (**Actual One**).
- Sendmail = send and receive mail through your server.
- httpd = Web Server.
- rsyslog = Generate logs or collect logs from other servers.
- OS Hardening
  - User Account
  - Remove un-wanted packages
  - Stop un-used services
  - Check on listening ports
  - Secure SSH configuration
  - Enable Firewall
  - Enable SELinux
  - Change Listening Port Numbers
  - Keep OS up to date.

## Network Commands

| Command             | What it does                           |
| ------------------- | -------------------------------------- |
| `ip a`              | List all available ip's or interfaces. |
| `ping <server>`     | Ping to a specific ip or server.       |
| `ping <server>`     | Ping to a specific ip or server.       |
| `netstat -rnv`      | Shows info about your network.         |
| `tcpdump -i <port>` | Shows incoming and outgoing traffic.   |
| `ethtool <port>`    | Shows information about your NIC.      |
| `nmtui`             | Network Manager tool.                  |

## File System Navigation Commands

| Command                                               | What it does                                                                                               |
| ----------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| `cd <directory>`                                      | Change directory.                                                                                          |
| `pwd`                                                 | Print working directory.                                                                                   |
| `ls`                                                  | List contents of current directory.                                                                        |
| `touch`                                               | Creates an empty file.                                                                                     |
| `cp`                                                  | Copy file.                                                                                                 |
| `cp -R <directory>`                                   | Copy directory recursively.                                                                                |
| `mkdir`                                               | Create directory.                                                                                          |
| `find <directory> -name "<name>"`                     | Find directory.                                                                                            |
| `locate <directory> -name "<name>"`                   | Locate directory. Almost same as find.                                                                     |
| `passwd <user>`                                       | Change password for specified user.                                                                        |
| `ln <file>`                                           | Creates hard link.                                                                                         |
| `ln -s <file>`                                        | Creates soft link.                                                                                         |
| `man <command>`                                       | Shows the manual for a specific command.                                                                   |
| `ls -l`                                               | File or directory permission.                                                                              |
| `chmod <permission> <file>`                           | Command to change permission.                                                                              |
| `chown <permission> <file>`                           | Changes the ownership of a file (`-R` flag for recursive).                                                 |
| `chgrp <permission> <file>`                           | Changes the group onwership of a file (`-R` flag for recursive).                                           |
| `setfacl -m <user/group>:<user>:<permissions> <file>` | Gives special permission to a file for a user group.                                                       |
| `setfacl -rm "entry" <file>`                          | Allow files/directories to inherit ACL.                                                                    |
| `setfacl -x <user/group>:<user> <file>`               | Removes special permission to a file for a user.                                                           |
| `setfacl -b <file>`                                   | Removes special permission to everyone.                                                                    |
| `whatis <command>`                                    | Tells you what the command does.                                                                           |
| `echo "<message>"`                                    | Echoes back that message.                                                                                  |
| `echo "<message>" > <file>`                           | Echoes back that message to a file.                                                                        |
| `echo "<message>" >> <file>`                          | Appends that message to a file.                                                                            |
| `cat <file>`                                          | Reads the content of a file.                                                                               |
| `tee <file>`                                          | Store and view (both at the same time) the output of any command.                                          |
| `tee -a <file>`                                       | Append and view (both at the same time) the output of any command.                                         |
| `wc -c <file>`                                        | Counts how many words are in a file.                                                                       |
| `<command> \| <commnand>`                             | A pipe is used by the shell to connect the output of one command directly to the input of another command. |
| `<command> \| <commnand>`                             | A pipe is used by the shell to connect the output of one command directly to the input of another command. |
| `rm <file>`                                           | Removes a file.                                                                                            |
| `rm -r <file>`                                        | Removes a directory.                                                                                       |
| `mv <file> <path to file>`                            | Moves a file to specified path.                                                                            |
| `head -<number> <file>`                               | Show only the top number of results.                                                                       |
| `tail -<number> <file>`                               | Show only the bottom number of results.                                                                    |
| `systemctl <service>`                                 | Control system services.                                                                                   |
| `ps`                                                  | Display all the current processes in the linux system.                                                     |
| `top`                                                 | Display system information.                                                                                |
| `kill <option> <PID>`                                 | Terminate processes manually.                                                                              |
| `crontab <option>`                                    | Schedule tasks.                                                                                            |
| `set <option>`                                        | Schedule tasks only once.                                                                                  |
| `df -h`                                               | Disk partition information and usage.                                                                      |
| `dmesg`                                               | Outputs system warnings or failures.                                                                       |
| `iostat`                                              | Input and output statistics.                                                                               |
| `netstat`                                             | Information about the computer.                                                                            |
| `free`                                                | Information about the memory.                                                                              |
| `cat /proc/cpuinfo`                                   | Information about the cpu.                                                                                 |
| `cat /proc/meminfo`                                   | Information about the memory.                                                                              |
| `ll /var/log`                                         | See all the logs.                                                                                          |
| `hostnamectl set-hostname <name>`                     | Changes the hostname of a machine.                                                                         |
| `script <filename>`                                   | Records every command in the specified file.                                                               |
| `printenv`                                            | Prints environment variables.                                                                              |
| `wget <url>`                                          | Download something from the web.                                                                           |
| `curl <url>`                                          | Show the specified url content (web).                                                                      |
| `ftp <ip>`                                            | Connect to server for file transfer.                                                                       |
| `scp <file> <ip>:<folder>`                            | Connect to server for secure file transfer.                                                                |
| `rsync -azvh <options> <source> <destination>`        | Sync files between computers.                                                                              |
| `nslookup`                                            | Information about a server.                                                                                |
| `ntpq`                                                | Sync local time with server.                                                                               |
| `cronyd`                                              | Sync local time with server.                                                                               |
| `timedatectl`                                         | Sync local time with server.                                                                               |
| `mail -s <subject line> <email>`                      | Send a mail.                                                                                               |

## Text Processor Commands

| Command                                          | What it does                                                                             |
| ------------------------------------------------ | ---------------------------------------------------------------------------------------- |
| `cut -c<number> <file>`                          | Allows you to cut parts of lines from specified file or piped data and print the result. |
| `cut -d<delimiter> -f <delimiter number> <file>` | Allows you to cut parts of lines from specified file or piped data and print the result. |
| `awk <arguments> <file>`                         | Exctract fields from a file or from an output.                                           |
| `grep <arguments> <file>`                        | Processes text line by line and prints any lines which match a specified pattern.        |
| `sort <file>`                                    | Sorts in alphabetical order.                                                             |
| `uniq`                                           | Filters out the repeated or duplicate lines.                                             |
| `diff`                                           | Compare two files line by line.                                                          |
| `cpm`                                            | Compare two files byte by byte.                                                          |
| `tar`                                            | Compress a file.                                                                         |
| `gzip`                                           | Compress a file.                                                                         |
| `gzip -d`                                        | Uncompress a file.                                                                       |
| `truncate <file>`                                | Shrink or extend the size of a file to the specified file.                               |
| `split <file>`                                   | Split to multiple files.                                                                 |
| `sed <regex> <file>`                             | Powerful string manipulation command.                                                    |
| `history`                                        | Display past shell commands.                                                             |
| `cat /home/users-dir-name/.bash_history`         | Display past shell commands by that user.                                                |

## User Account Commands

| Command             | What it does                                   |
| ------------------- | ---------------------------------------------- |
| `useradd <name>`    | Creates a user with name.                      |
| `id <name>`         | Shows id for that user.                        |
| `groupadd <name>`   | Creates a group with name.                     |
| `userdel -r <name>` | Deletes user with name.                        |
| `groupdel <name>`   | Deletes a group with name.                     |
| `usermod <name>`    | Modifies a user with name.                     |
| `chgrp -R <name>`   | Changes a user group with name.                |
| `chage`             | Sets an expiration date for the user password. |
| `su - <user>`       | Change user or become root.                    |
| `who`               | Shows how many people are logged in.           |
| `last`              | All the details from users.                    |
| `w`                 | Same as `who` but a little more info.          |
| `finger`            | A lot of details from users.                   |
| `users`             | Show which users are logged in.                |
| `wall`              | Broadcast message to all logged users.         |
| `write <user>`      | Write specific message to user.                |
| `date`              | Display actual date.                           |
| `uptime`            | How long has the system been up.               |
| `hostname`          | Display actual hostname.                       |
| `uname -a`          | Display all OS information.                    |
| `which <command>`   | Display the location file of that command.     |
| `cal`               | Display calendar.                              |
| `bc`                | Basic calculator.                              |

## Process Managment Commands

| Command                      | What it does                                |
| ---------------------------- | ------------------------------------------- |
| `Ctrl + z`                   | Put a process in the background.            |
| `sleep <number>`             | Sleep process for amount of time.           |
| `bg <command>`               | Run process on the background.              |
| `jobs`                       | Display processes on the background.        |
| `fg`                         | Bring process to the front.                 |
| `nohup`                      | Run the process even if terminal is closed. |
| `nice -n <number> <command>` | Give priority to a task.                    |

## System Maintenance Commands

| Command    | What it does                   |
| ---------- | ------------------------------ |
| `shutdown` | Shuts down the system.         |
| `reboot`   | Reboots the system.            |
| `halt`     | Forcely shuts down the system. |

## Shell Programing

- What is shell?
  - Interface between users and Kernel/OS.
  - CLI is a shell.
- What is a shell script?
  - A shell script is an executable file containing multiple shell commands that are executed sequentially.
  - Shell (`#!/bin/bash`)
  - Comments (`#`)
  - Commands
  - Statements
- Input/Output
  - read
  - echo
- If then

  ```bash
  if [statement]
    then
      # code
    else
      #code
  fi
  ```

- For loops

  ```bash
  for i in range
    do
      #code
  done
  ```

- Do while

  ```bash
  while [condition]
  do
    #code
  done
  ```

- Alias
  - `alias <name> = "<command>"`
  - `unalias <name>`
