Requirements Any Linux distro

## File System Navigation

**Command Description**<br/>
```bash
ls	    => List all the files in a directory
ls -l	    => List all files and their details (owner, mtime, size, etc)
ls -a	    => List all the files in a directory (including hidden files)
pwd	    => Show the present working directory
cd	    => Change directory to some other location
file	    => View the type of any file
```
 

## View, Create, Edit, and Delete Files and Directories
**Command Description**<br/>
```bash
mkdir          => Create a new directory  
touch          => Create a new, empty file, or update the modified time of an existing one  
cat > file     => Create a new file with the text you type after  
cat file       => View the contents of a file  
grep           => View the contents of a file that match a pattern  
nano file      => Open a file (or create new one) in nano text editor  
vim file       => Open a file (or create new one) in vim text editor  
rm or rmdir    => Remove a file or empty directory  
rm -r          => Remove a directory that isn’t empty  
mv             => Move or rename a file or directory  
cp             => Copy a file or directory  
rsync          => Synchronize the changes of one directory to another

```
 

## Search for Files and Directories
**Command Description**<br/>
```bash
locate name                                   => Quickly find a file or directory that has been cached by its name  
find                                          => Search for a file or directory based on name and other parameters  
find /home/john -name 'prefix*' -size 100M+   => Find files in /home/john that start with "prefix" and are larger than 100MB


```
 

## Basic Administration Commands
**Command	Description**<br/>
```bash
whoami      	 => See which user you are currently logged in as
sudo	         => Execute a command with root permissions
sudo apt install => Install a package on Debian based systems
sudo dnf install => Install a package on Red Hat based systems
sudo apt remove	 => Remove a package on Debian based systems
sudo dnf remove	 => Remove a package on Red Hat based systems
reboot	         => Reboot the system
poweroff	 => Shut down the system
```
 

## Hard Drive and Storage Commands
**Command	Description**<br/>
```bash
df or df -h           => See the current storage usage of mounted partitions  
sudo fdisk -l         => See information for all attached storage devices  
du                    => See disk usage of a directory’s contents  
tree                  => View the directory structure for a path  
mount and umount      => Mount and unmount a storage device or ISO file

```
 

## Compression Commands
**Command	Description**<br/>
```bash
tar cf my_dir.tar my_dir        => Create an uncompressed tar archive
tar cfz my_dir.tar my_dir	=> Create a tar archive with gzip compression
gzip file	                => Compress a file with gzip compression
tar xf file	                => Extract the contents of any type of tar archive
gunzip file.gz	                => Decompress a file that has gzip compression
```
 

## Networking Commands
**Command	Description**<br/>
```bash
ip a	                => Show IP address and other information for all active interfaces
ip r	                => Show IP address of default gateway
cat /etc/resolv.conf	=> See what DNS servers your system is configured to use
ping	                => Send a ping request to a network device
traceroute	        => Trace the network path taken to a device
ssh	                => Login to a remote device with SSH
 ```

## File Permissions and Ownership
**Command	Description**<br/>
```bash
chmod	=> Change the file permissions for a file or directory
chown	=> Change the owner of a file or directory
chgrp	=> Change the group of a file or directory
 ```

## User Management Commands
**Command	Description**<br/>
```bash
useradd  => Low level utility for adding new user accounts
adduser	 => High level utility for adding new user accounts
deluser	 => Delete a user account
usermod	 => Modify a user account
groupadd => Create a new group
delgroup => Delete a group
 ```

## System Resource Management Commands
**Command	Description**<br/>
```bash
free -m                    => See how much memory is in use and free  
top                        => See a list of processes and their resource usage  
htop                       => A more human readable and interactive version of top  
nice                       => Start a new process with a specified priority  
renice                     => Change the nice value of a currently running process  
ps aux OR ps -ef           => View all of the currently running processes  
kill or killall            => Terminate a process  
kill -9 or killall -9      => Terminate a process with SIGKILL signal  
bg                         => Send a task to the background  
fg                         => Bring a task to the foreground

 ```

## Environment Variable Commands
**Command	Description**<br/>
```bash
uname -a                       => Output detailed information about your kernel version and architecture
lsmod                          => Find what modules are currently loaded
modinfo module_name            => Get information about any particular module
modprobe --remove module_name  => Remove a module
modprobe module_name           => Load a module into the kernel

 ```

## Kernel Information and Module Management
**Command	Description**<br/>
```bash
uname -a                       => Output detailed information about your kernel version and architecture  
lsmod                          => Find what modules are currently loaded  
modinfo module_name            => Get information about any particular module  
modprobe --remove module_name  => Remove a module  
modprobe module_name           => Load a module into the kernel  

 ```

## Hardware Information Commands

**Command	Description**<br/>
```bash
lspci                            => See general information about host bridge, VGA controller, ethernet controller, USB controller, SATA controller, etc.  
dmidecode                        => See some information about BIOS, motherboard, chassis, etc.  
cat /proc/cpuinfo                => Retrieve processor type, socket, speed, configured flags, etc.  
x86info or x86info -a            => See information about the CPU  
cat /proc/meminfo                => See detailed information about system RAM  
lshw                             => List all hardware components and see their configuration details  
lshw -C memory -short            => Detect number of RAM slots used, speed, and size  
hwinfo                           => List details for all hardware, including their device files and configuration options  
biosdecode                       => Get some general information about your system’s BIOS  
dmidecode -s bios-vendor         => Retrieve the name of your BIOS vendor with this simple command  
lsusb                            => Get a list of USB devices plugged into your system  
ls -la /dev/disk/by-id/usb-*     => Retrieve a list of USB device files  
hdparm -I /dev/sdx               => Get information about your hard drive’s make, model, serial number, firmware version, and configuration  
hdparm -tT /dev/sdx              => Show the speed of an installed hard drive – including cached reads and buffered disk reads  
wodim --devices                  => Locate CD or DVD device file  

```