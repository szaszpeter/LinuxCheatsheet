# Linux Cheatsheet
An empty repo containing a list of useful Linux commands

## Navigating and Working with Files

- `cd` - change directory
- `ls` - list files, see list of options
- `touch` - create a file 
- `nano` - edit file
- `cp <origin> <destination>` - copy
- `mv <origin> <destination>` - move
- `rm <filename>` - remove
- `mkdir` - create directory
- `rmdir` - remove directory
- `cat` - display content of a file


## Saving Results to a File

- `output > filename` - wipes content and writes output
- `output >> filename` - adds output to the existing content of the file



## Searching and comparing files

- `grep keyword <filename>` - lists search results after the keyword in a specific file
- `diff file1 file2` - lists the differences between the 2 files


  
## Verifying Files Using Checksum

- `sha1sum <filename>`



## Compress and Extract tar and gz Files

- `gzip <filename>` - compress file
- `gunzip <filename>` - uncompress files

- `tar cvf <targetfilename> <list of files>` - compress a list of files into an archive
- `tar xvf <archivename>` - uncompresses the archive



## Install Software with APT apt-get

- `sudo apt-get update` - update the advance package manager

- `sudo apt-get install <packagename>` - install the specified package

- `bash <scriptname>` - run shell scripts



## Users

- `sudo useradd <username>` - create user
- `sudo passwd <username>` - set user password



## Groups

- `sudo groupadd <groupname>`
- `sudo usermod -a -G <groupname> <username>`
- `sudo userdel <username>`

## SSH

### Connect to Server

- `ssh <username>@<ip_address>` - connects to the specified address with username
  
### SSH Key Authentication

- `ssh-keygen -t rsa` - generate public / private rsa key pair
- `ssh-copy-id root@serveraddress` - adding ssh key to server


## SFTP

- `sftp <username>@<ip_address>` - connects to remote machine with SFTP enabled
- `put <path/filename>` - uploads a file to the working directory
- `put -r <foldername>` - uploads a folder to the working directory
- `get <filename>` - downloads a file from server 
- `get -r <foldername> <destination>` - downloads a folder from the server



## Processes & Jobs

- `ps` - list all your processes
- `ps ax` - list all system processes
- `<program_name> &` - runs the program in the background
- `jobs` - list of jobs running
- `fg %<job number>` - brings job to foreground
- `CTRL+C` - terminates a process
- `CTRL+Z` - pauses a process
- `kill PID` - kill process directly
- `kill -STOP PID` - stops a process
- `kill -CONT PID` - resumes a process


