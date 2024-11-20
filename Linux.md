# Linux Commands Cheat Sheet

This cheat sheet provides a collection of common Linux commands for managing your system and projects.

## System Management

| **Action**                           | **Command**                                          |
| ------------------------------------ | ---------------------------------------------------- |
| **Reboot system**                    | `sudo reboot`                                        |
| **Shutdown system**                  | `sudo shutdown`                                      |
| **Shutdown system immediately**      | `sudo shutdown now`                                  |
| **Reboot to runlevel 6**              | `sudo init 6`                                        |
| **Update and upgrade system**        | `sudo apt update && sudo apt upgrade -y`             |
| **Install Docker**                   | `sudo apt install docker.io`                         |
| **Install vim**                       | `sudo apt install vim`                               |
| **Install curl**                      | `sudo apt install curl`                              |
| **Install firewall**                  | `sudo apt install gufw`                              |
| **Install neofetch**                  | `sudo apt install neofetch`                          |
| **Install net-tools (ifconfig)**     | `sudo apt install net-tools`                         |
| **Install vsftpd (FTP)**             | `sudo apt install vsftpd`                            |
| **Install openssh-client (SSH)**     | `sudo apt install openssh-client`                    |
| **Install figlet**                   | `sudo apt install figlet`                            |
| **Install lolcat**                   | `sudo apt install lolcat`                            |
| **Install nethogs**                  | `sudo apt install nethogs`                           |
| **Install bmon**                     | `sudo apt install bmon`                              |
| **Install iptraf**                   | `sudo apt install iptraf`                            |
| **Install cbm**                      | `sudo apt install cbm`                               |
| **Install cowsay**                   | `sudo apt install cowsay`                            |
| **Install cmatrix**                  | `sudo apt install cmatrix`                           |
| **Clear terminal**                   | `clear` or `Ctrl + L`                                |
| **Install tmux**                     | `sudo apt install tmux`                              |

## File and Directory Management

| **Action**                           | **Command**                                          |
| ------------------------------------ | ---------------------------------------------------- |
| **Create a directory**               | `mkdir <dir_name>`                                   |
| **Remove a directory**               | `rmdir <dir_name>`                                   |
| **Remove a directory recursively**   | `rm -r <dir_name>`                                   |
| **Create a symbolic link**           | `ln -s <source_path> <link_name>`                     |
| **List files in a directory**        | `ls` or `ll` or `ls -lh` (list in human-readable format) |
| **Print working directory**          | `pwd`                                                |
| **Change directory**                 | `cd <path>`                                          |
| **Go to home directory**             | `cd`                                                 |
| **Go back one directory**            | `cd ..`                                              |
| **Go to root directory**             | `cd /`                                               |
| **Create a new file**                | `touch <file_name>`                                  |
| **Remove a file**                    | `rm <file_name>`                                     |
| **Rename a file**                    | `mv <old_name> <new_name>`                           |
| **Copy a file**                      | `cp <source> <destination>`                          |
| **Move a file**                      | `mv <source> <destination>`                          |

## Process Management

| **Action**                           | **Command**                                          |
| ------------------------------------ | ---------------------------------------------------- |
| **Start SSH service**                | `sudo service sshd start`                            |
| **Run a command in the background**  | `nohup <command> &`                                  |
| **Check system processes**           | `top`                                                |
| **Show all processes**               | `ps`                                                 |
| **Show detailed process info**       | `htop`                                               |
| **Terminate a process**              | `kill <PID>`                                         |
| **Kill all processes with a label**  | `killall <process_label>`                            |
| **Show process PID**                 | `pidof <process_name>`                               |
| **Tree-like diagram of processes**   | `pstree`                                             |
| **Show memory usage by process**     | `pmap <PID>`                                         |

## User Management

| **Action**                           | **Command**                                          |
| ------------------------------------ | ---------------------------------------------------- |
| **Check current user**               | `whoami`                                             |
| **Show user info**                   | `finger <user_name>`                                 |
| **Add a new user with home directory**| `sudo useradd <username>`                            |
| **Add a new user without home directory** | `sudo adduser <username>`                          |
| **Delete a user**                    | `sudo userdel <username>`                            |
| **Add user to a group**              | `sudo usermod -aG <group_name> <username>`           |
| **Set password for user**            | `sudo passwd <username>`                             |
| **Add a new group**                  | `sudo groupadd <group_name>`                         |
| **Delete a group**                   | `sudo groupdel <group_name>`                         |
| **Change group name**                | `sudo groupmod -n <new_name> <old_name>`             |
| **Check user status**                | `sudo vi /etc/group`                                 |
| **More user information**            | `sudo vi /etc/passwd`                                |

## Networking

| **Action**                           | **Command**                                          |
| ------------------------------------ | ---------------------------------------------------- |
| **Check IP address**                 | `ifconfig` or `ip a`                                 |
| **Check routing table**              | `route`                                              |
| **Check traceroute**                 | `traceroute <IP>`                                    |
| **Ping a host**                      | `ping <IP>`                                          |
| **Check active users**               | `w`                                                  |
| **Show active user**                 | `who`                                                |
| **List users**                       | `id <username>`                                      |
| **Remote server sync**               | `rsync -a <source> <user>@<remote_host>:<destination>`|
| **Secure FTP**                       | `sftp <user>@<remote_host>`                           |
| **FTP transfer**                     | `ftp <remote_host>`                                  |
| **Check firewall status**            | `sudo ufw enable`                                    |
| **Allow SSH traffic through firewall**| `sudo ufw allow ssh`                                 |
| **Connect via SSH**                  | `ssh <username>@<hostname>`                           |

## Disk Management

| **Action**                           | **Command**                                          |
| ------------------------------------ | ---------------------------------------------------- |
| **Check disk usage**                 | `df -h`                                              |
| **Check memory status**              | `vmstat`                                             |
| **Check disk partition**             | `fdisk -l`                                           |
| **Check memory usage**               | `free`                                               |
| **Disk usage for files and directories** | `du -ah`                                           |
| **Find mounted filesystems**         | `mount`                                              |
| **Mount a device**                   | `mount <device_path> <mount_point>`                   |
| **Show bootup messages**             | `dmesg`                                              |
| **Show disk usage summary**          | `du -sh`                                             |
| **Generate SSH key pairs**           | `ssh-keygen`                                         |
| **Change file permissions**          | `chmod <permissions> <file_name>`                     |
| **Change file ownership**            | `chown <user>:<group> <file_name>`                    |

## Time Management

| **Action**                           | **Command**                                          |
| ------------------------------------ | ---------------------------------------------------- |
| **Change system time**               | `timedatectl`                                        |
| **Show current time**                | `date`                                               |
| **Show system uptime**               | `uptime`                                             |
| **Show calendar**                    | `cal`                                                |
| **Schedule shutdown**                | `shutdown <hh:mm>`                                   |
| **Show reboot history**              | `last reboot`                                        |

## Projects

### Project: Change MAC Address
1. `sudo su`
2. `macchanger -c`
3. `clear`

### Project: Install and Configure SSH
1. `sudo apt install openssh-client`
2. `sudo systemctl start ssh`
3. `sudo ufw allow ssh`
4. `sudo systemctl enable ssh`
5. `sudo useradd <username>`
6. Check with client: `ssh <username>@<hostname>`

### Project: Install Samba Server
1. `sudo apt install samba`
2. `sudo smbpasswd -a <username>`
3. `sudo ufw allow smbd`
4. `mkdir /home/<username>/Desktop`

### Project: Using tmux
1. `sudo apt install tmux`
2. `tmux new -s <session_name>`
3. `tmux ls` (to list sessions)
4. `tmux kill-session -t <session_name>`

### Project: Python on Terminal
1. `python3 <file_name.py>`

