<!-- Headiing -->

 # LINUX 

> Kernel : Linux kernel is the core part of the operating system. It establishes communication between the devices.  It basically acts as an interface between user applications and hardware. 

>Shell :  A shell is a user program which providing us to interface to use operationg system.

<!-- images -->
<p align="center"/><img src="Images\linux_1.jpg" width="70%" />




## Linux Commands

<!-- Tables -->
| COMMANDS        |     SYNTAX               |    EXPLNATION     
| -------------   | -------------            | --------------
| cd              | cd "Directory"name       | Changes the directory from one to other. 
|                 | cd /                     | Changes to previous directory.
|                 | cd ..                    | Moves Directory one step back.
|                 | cd ~                     | Takes us to the home directory.
| pwd             | pwd                      | Print working directory or present working directories.
| ls              | ls "directory name"      |  List all things which are present inside current directory.
|                 | ls -l                    |  Display all the file details in detaied format.
|                 | ls -a                    | It shows us all hidden files and folders.
|                 | ls -h    -h = Human Readable                | Memory we can see in thhe human readable format like 4.0k,1.0k.
|                 | ls -t                     |  It basically display in asending order.The file which is created very first disply on the top.
|                 |  ls -r                    | It will display exactly opposite of '-t' i.e. in reverse order.
|                 | ls -f                     | When there is directory ,it automatically add '/' after that.
|                 | ls -lahtrf                | We can do all commands at once.
| man             | man                       | It it manual ,it gives us the detailed description of command.
| who             | wh0                       | Its shows who are logged in.
| whoami          | whoami                    | Represents the user.
| touch           | touch "filename"          | Create a new file . 
| clear           | clear                     | clears the screen.
| ping            | ping                      | to check the internet speed and connectivity.
| history         | history                   | Show all commands that we have run before.
| echo            | echo "value"              | It takes the value and display it.
| ps              | ps                        | It shows the running applications.
| cp              | cp 'flie1' 'file2'        | Copy one file to another.
| mkdir           | mkdir 'directory-name'    | It makes a new directory.
| rm              | rm 'filename'             | Remove the file.
|                 | rm -r                     | It only removes files.
|                 | rm -rf                    | It only removes directories.
|                 | rm -rf*                   | It removes both files and directories.
| mv              | mv 'f1' 'f2'              | Moves one file to another file.
|                 | mv 'dir' 'dir'            | Moves one directory to other.
|                 | mv 'f2' 'dir'             | Moves directory into file.
| ipconfig(windows)    | ipconfig             | Gives the network information and addresses.
| ifconfig(Apples OS)  | ifconfig             | Gives the network information and addresses.
| exit            | exit                      | Exits from the terminal.
| cat             | cat > 'file1'             | It is used to write or read the data from file. when we use '>' we write into file. and without'>' we can read from file.
|                 | cat >> 'file1'            | '>" by using we can write he data but it overwriiten data .So we use '>>' it will add the data .
| less            | less 'filename'            | It basically gives the more information.
| more            | more 'filename'            | It gives the less data.
| top             | top                        | Gives us the system information.
| ssh             | ssh '@host_ip_address'     | It helps to login to a specific/another server.
|                 |                            |





<!-- ---------------------------------------------------------------------- -->


## Linux File System

<p align="center"/><img src="Images\file system_1.jpg" />

| Directory     | Explanation           |
| ------------- | -------------         |
| /root         | Every single file & directories starts from root directory.                              |
| /boot         | System Kernel is stored in boot. It contains boot loader related files. And grub files are come under the /boot. |
| /bin          | All binary files are stored. Commands use by the users of the system are in /bin. for eg., ps,ls,ping.          |
| /sbin         | Just like /bin it also contains the binary files.This directory used by system admin.                           |
| /home         | It is for all the users who stores their personal files. for e.g /home/poonam                                    |
| /usr          | all the user related resources and supportig software of an OS stored here. It contains binary files for user pprograms.                                                     |
| /var          | Variables files.                             |
| /dev          | It contains device files. These includes the terminal devices,mouse ,keyboard,USB attached to the system.   |
| /mnt          | Its is a temporary mount directory where system admin can mount files. It is designed for CD-ROM's.            |
| /opt          | Optional add on applications or pacakages.   |
| /lib          | System libraries  are stored in lib          |
| /media        | Temporary mount directory for removable devices |
| /proc         |  It conatains the information about system Kernel. Process files are stored inside proc.                            |
| /tmp          | Temporary files are saved here ,ut when system reboots these files will be deleted.                             |
| /etc          |  System configuration files are stored.        |
|               |                                                |
                 
 

