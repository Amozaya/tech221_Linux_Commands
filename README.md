## Linux Commands
* `clear` - clears the terminal window
* `exit` - exits Linux environment
* `ls` - gives the list of files and folders inside the current directory
* `ls -a` - same as `ls` but also shows hidden files/folders
* `whoami` - tells which OS is used
* `pwd` - shows present working directory
* `uname` - tells the username
* `uname -a` - tells all the information such as version of OS, IP address, timezone etc
* `mkdir <name>` - creates directory called <name>
* `cd <name>` - change directory to <name>
* `cd ..` - go one step back inside the directory
* `touch <name>.txt` - creates a file with <name> and extension <.txt>
* `nano <name>.txt` - opens `.txt` file with `nano` editor
* `cat <name>.txt` - shows the content of the file inside the CLI
* `cp <file_name>.txt <directory_path>` - copy the `<file_name>.txt` into the directory specified
* `rm <file_name>.txt` - deletes the file
* `mv <file_name>.txt <directory_path>` - move the `<file_name>.txt` into the directory specified
* `ll` - lists the details of all the files inside the folder
* `chmod 700 <file_name>.txt` - change access permission of the file
* `top` - open "task manager"
* `history` - history of all commands used
* `rm -rf <file_name>` - `-rf` forces file removal in case it's open or needs permission
* `sudo <command>` - `sudo` grants admin permission 
* `head -1 <file_name>` - prints the first line from the file
* `nl <file_name>` - asigns numbers to each line of text
* `tail -1 <file_name>` - prints the last line from the file
* `sort <file_name>` - sort the content in alphabetical order
* `cat <file_name> |grep <content>` - searches file for specific content and prints it out
* `sudo su` - enters into Admin mode
* `apt ....` - package manager
* `sudo systemctl stop/start nginx` - used to stop/start process
* `sudo apt install nginx` - install nginx
* `sudo apt update/upgrade -y` - used to update/upgrade services. `-y` will automate responce "Yes"
* `service nginx status` - check the status of nginx service
* script to automate update/upgrade, installation and enabling of nginx:
  * `sudo touch provision.sh` - create a scipt file
  * `sudo nano provision.sh` - open the file with nano
  * use follwing to add to your script:
  
    `#!/bin/bash`
    
    `sudo apt update -y`

    `sudo apt upgrade -y`

    `sudo apt install nginx -y`

    `sudo systemctl restart nginx`

    `sudo systemctl enable nginx`
    
   * `sudo chmod +x provision.sh` - make file executable
   * `sudo ./provision.sh` - execute file

