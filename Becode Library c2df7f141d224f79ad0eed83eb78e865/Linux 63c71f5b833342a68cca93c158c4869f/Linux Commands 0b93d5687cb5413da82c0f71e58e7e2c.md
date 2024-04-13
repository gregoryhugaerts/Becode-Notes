# Linux Commands

Deploying Linux Machine through SSH
"ssh usernameofaccount@ipofmachine"

`ssh [admin123@10.10.244.14](mailto:admin123@10.10.244.147)`

## Help

---

- `man`: display system documentation
- `whatis`: prints manual page description
- `info`: read info documents
- `—help / -h / -?`  : shows all options that a command accepts

## Navigation

---

- `cd`: change current directory
- `ls`: list directory content
    
    `-a`: list all files, including hidden ones
    
    `-l`: show permissions, ownership, size, and modification dates
    
    `-h`: show file sizes in kiB, MiB, GiB, etc
    
    `-d`: only show directories
    
- `pwd`: print the current directory
- `pushd`: go to a folder while keeping old location on *"cache"*
- `popd`: go back to an old location on *"cache"*
- `locate`: find filenames quickly
- `find`: searches the system for a file
    
    `-name “file name”`: searches for a specific file based on its name
    
    `-name *.txt`: searches for all files with .txt extention
    
    `-iname`: same as -name, but case insensitive
    
- `which`: locate a program in the user's path
    
    `-a`: display all matches
    
- `grep`: allows to search the content of files for specific values

## File Operation

---

- `cat`: concatenate and print files
- `touch`: create a file or update timestamps
- `cp`: copy a file
    
    `-r`: copy directories recursively
    
    `-n`: do not overwrite an existing file
    
    `-i`: prompt before overwrite
    
    `-f`: if an existing destination file cannot be opened, remove it and try again (redundant if the **-n** option is used)
    
    `-l`: link files instead of copying
    
- `mkdir`: create a directory
    
    `-p`: no error if existing, make parent directories as needed
    
- `mv`: move or rename a file
    
    `-f`: do not prompt before overwriting
    
    `-n`: do not overwrite an existing file
    
- `rm`: remove a file or directory
    
    `-r`: remove directories and their contents recursively
    
    `-f`: ignore nonexistent files, never prompt
    
    `-rf`: forcefully and recursively remove files and directories
    
    `--interactive`: ask before removing each file
    
- `rmdir`: remove an empty directory
- `ln`: link files
    
    `-s`: make a symbolic link instead of a hard link
    
- `head`: output the first part of files
- `tail`: output the last part of files
- `file`: determine the type of a file
- `scp`: allows us to transfer files between two computers using SSH

## System

---

- `date`: print the date and time
- `cal`: display a calendar
- `lsblk`: list connected drives

## Users

---

- `passwd`: change user password
- `usermod`: modify a user account
- `groupadd`: create a new group
- `whoami`: print current logged user

## Permissions

---

- `sudo`: execute a command as another user
- `su`: change the current user
- `chmod`: change file permissions
- `chown`: change the owner of a file
- `chgrp`: change the group of a file

## Compression

---

- `tar`: archive files
- `gzip`: compress and expand files

## Remote

---

- `ssh`: remote login
- `rsync`: remote file copying tool

## Process management

---

- `ps`: displays list of running processes
    
    `-aux`: provides a list of running processes run by others
    
    `-x`: show active processes of the current user
    
    `-u <username>`: show processes from <username>
    
- `kill`: terminates a process
    
    `-9`: really kill the process if it’s stuck
    
- `top`: displays list of running processes
- `htop`: improved version of `top`
- `bg`: puts a process to the background
- `fg`: brings a process to the foreground
- `systemctl`: allows us to interact with the systemd process
- `crontab`: used to create, view, edit, and delete crontab entries
    
    `-e`: used to edit the current user's crontab file
    

## Package Manager

---

- `apt` : package manager for debian based linux systems
- `pacman` : package manager for arch based linux systems
- `pip` : python package manager
- `npm` : nodejs (javascript) package manager
- `composer` : php package manager
- `wget`: allows us to download from the web via HTTP

---

## Text Manipulation

---

- `cat` : display the contents of one or more files
- `less` : open a file for interactive reading
- `head` : show the first lines in a file or input
    
    `-n <count>`: show first <count> lines 
    
- `tail` : show the last lines in a file or input
    
    `-n <count>`: show last <count> lines
    
- `watch` : execute a command repeatedly, and monitor it’s output
- `split` : split a file into sub-files
    
    `-n <count>`: split into <count> pieces
    
    `-b <size>` : split into files with size <size> or smaller
    
    `-l <count>` : split into files of <count> or less lines
    
- `nl` : add line numbers to it’s input

---

## Text Editor

---

- `vim` : highly configurable modal text editor
- `nvim` : fork of vim that can be configured with both vimscript and lua
- `nano`: creates a file.
- `emacs` : An extensible file editor, configured with emacs lisp

---

## Web Tools

---

- `wget` : download files from the web
    
    `—continue`: continue an incomplete download
    
- `curl` :  Transfers data from or to a server.
Supports most protocols, including HTTP, FTP, and POP3.
    
    `—output <filename>`: output to a file instead of STDOUT 
    
    `—header <name:value>`: add a header to the request
    
    `—request <NAME>`: use a custom http method
    

---

## Operators

- `&`: allows to run commands in the background of your terminal
- `&&`: allows to combine multiple commands in one line of your terminal
- `>`: this is a redirector. We can take the output of a command with this and direct it elsewhere
- `>>`: same function as above, but appends the output rather than replacing. Nothing is overwritten
- `|`:  send output from one command to the input stream of another command
- `2>`:  redirect the standard error stream of a command to a file

---

TO DO

- Join
- Paste
- Wildcards (add link to wildcard website)
- RE (add link to RE website)
- Metacharacters  (link?)
- add grep switches
- cut, sort, wc, uniq, diff
- sed (add links to sed page)
- awk
- printenv
- add = operator
- export
- wait
- jobs
- add services like nginx, vsftpd, telnetd, samba and tft-hpa

## SHORTCUTS

CTRL + L= cleans up terminal

---

## FLAGS AND SWITCHES

-a / --all = shows all folders including hidden ones
--help or -h = shows all options that a command accepts.
-l = start a shell to loginls

---

## COMMON DIRECTORIES

/etc = place where system files are stored by your OS.
/var = directory where variable data is stored.
/root = home for root system user
/tmp = temporary directory that stores data that only needs to be accessed once or twice.

## SIGNALS

send with kill -s $SIGNAL pid

SIGTERM = Kill the process, allow it to do some cleanup tasks beforehand.
SIGKILL = Kill the process - doesn't do any cleanup after the fact
SIGSTOP = stop/suspend a process