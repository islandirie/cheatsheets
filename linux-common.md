# Linux Commands Cheatsheet

## 1. Navigation

- **Change Directory:**
  - `cd directory_name`
  - `cd /absolute/path`

- **List Files and Directories:**
  - `ls`
  - `ls -l` (long format)
  - `ls -a` (show hidden files)

- **Copy Files or Directories:**
  - `cp source_file destination`
  - `cp -r source_directory destination` (recursive)

- **Move (Rename) Files or Directories:**
  - `mv source destination`

- **Remove Files or Directories:**
  - `rm file_name`
  - `rm -r directory_name` (recursive)
  - `rm -f file_name` (force)

## 2. File Operations

- **Create a File:**
  - `touch filename`

- **Create a Directory:**
  - `mkdir directory_name`

- **View File Content:**
  - `cat filename`
  - `less filename` (paginated view)

- **Edit a File:**
  - `nano filename`
  - `vim filename`

## 3. System Information

- **Display System Information:**
  - `uname -a`

- **Show Disk Usage:**
  - `df -h`

- **Show Memory Usage:**
  - `free -m`

## 4. Process Management

- **List Running Processes:**
  - `ps aux`

- **Kill a Process:**
  - `kill process_id`

- **Kill a Process Forcefully:**
  - `kill -9 process_id`

- **Check Process Resource Usage:**
  - `top`

## 5. User Management

- **Show Current User:**
  - `whoami`

- **Switch User:**
  - `su username`

- **Change User Password:**
  - `passwd`

## 6. Network

- **Show Network Interfaces:**
  - `ifconfig`

- **Ping a Host:**
  - `ping hostname`

- **Check Open Ports:**
  - `netstat -tulpn`

## 7. Package Management

- **Update Package Lists:**
  - `sudo apt update` (Debian/Ubuntu)
  - `sudo yum update` (Red Hat/CentOS)

- **Install a Package:**
  - `sudo apt install package_name` (Debian/Ubuntu)
  - `sudo yum install package_name` (Red Hat/CentOS)

- **Remove a Package:**
  - `sudo apt remove package_name` (Debian/Ubuntu)
  - `sudo yum remove package_name` (Red Hat/CentOS)

## 8. File Permissions

- **Change File Permissions:**
  - `chmod permissions filename`

- **Change Ownership of a File:**
  - `chown new_owner:new_group filename`

- **Change Group of a File:**
  - `chgrp new_group filename`

## 9. Searching and Finding

- **Find Files and Directories:**
  - `find /path/to/search -name "filename"`

- **Search for Text in Files:**
  - `grep "search_text" filename`
  - `grep -r "search_text" /path/to/search` (recursive)

## 10. Compression and Decompression

- **Create a Tar Archive:**
  - `tar -cvf archive_name.tar files/directories`

- **Extract from a Tar Archive:**
  - `tar -xvf archive_name.tar`

- **Create a Zip Archive:**
  - `zip archive_name.zip files/directories`

- **Extract from a Zip Archive:**
  - `unzip archive_name.zip`

## 11. System Shutdown and Reboot

- **Shutdown the System:**
  - `sudo shutdown now`

- **Reboot the System:**
  - `sudo reboot`

## 12. Miscellaneous

- **Display Manual Page:**
  - `man command_name`

- **Display Calendar:**
  - `cal`

- **Check System Uptime:**
  - `uptime`

- **Edit File Permissions Interactively:**
  - `chmod +x filename` (add execute permission)
  - `chmod -x filename` (remove execute permission)
