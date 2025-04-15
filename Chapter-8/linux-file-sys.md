# What is a file system?
	- A file system is how a computer organizes its files. Files are often classified by type. 
	- inode, index node
		- keeps file metadata (who authored the file, when, size, type) 
		- every file has a inode
		- pointer to the location of the file in the hard drive 
		- to see inode, use the `-i` flag
		(pic1)

# Linux file sys
	- linux has no letter drive, the root directory is `\`
	- 
	(pic 2)

# Addin user
	- sudo adduser (username)
	- make sure you are in the root directory when you do this
	(Pic 3)
	- 1001 is the user ID

# Password
	- stored in the dictory `/etc/shadow`
		Use `sudo vim shadow`
	- You can see the password hash, but not the password its self
	- The system will compare this hash value with the hash value of the user input for the password
	(Pic 4)
	- Shows the user id, hash, and the login shell
		- `usr/sbin/nologin`
			- not a user cannot login
		- `bin/sh`, `bin/
	- 

# etc/group
	- Shows all the group in the system
	- Also privliageed

# etc/sudoers
	- Shows all authorized sudoers users (beyond standard users)
	- To promote standard to privilage user, just add their username to the `sudoers` file	
	- Can limit certain privilages that a newly added privilage user can do
	- Substitue user doers (Sudoers)
	- 

# Privlaage vs normal files
	- Privialage: shadow, sudoers
	- Normal: password

Executables files = binaries

# /bin
	- The green are binaries
	- (Pic 5)
	- They are terminal level exectuables
	- 

# /sbin
	- binareis that only privilaged users can execute
	- deleting and adding groups of users

# /boot
	- contains bootable kernal
	- vmlinux is the boot file of your kernal 
		- `vmlinuz-6.8.0-57-generic` is the latest and currently running kernal
	- The older version is always kept around, as a net just in case the main kernal is messed up
	- (Pic 6)

# /dev
	- device drivers, lets say you conntected a printer to the drectory, there will be a file for the printer
	- All devices (physicla or virtual) are in this file
	- stderr is in this directory

# /proc
	- stores the process of the kernal 
	- lets say you run a.out, that is a process
		- as soon as you finish running the process the process folder disappears
		- Store metadata about the process who ran it, what size, how long, etc. 
	- White files tell you informaiton about your system
	- (Pic 7)

# /usr
	- contains applications and libarires NOT user informaiton

# /opt
	- contains optional files
	- optional software, software that  is made for linux but not made by linux (Chrome, Zoom, Skype)
	- 

# /var
	- files that are variable in size (can change smaller and larger in real time)
	- auth.log a sudo command is logged here
	- kern.log
	- var = variable length, all files here changes in size
	
# /mnt
	- Lets say I have an external hard drive and I want to plug it in and edit files in the harddrive
		- `mnt` is attaching external file system to home file system
		- Cameras, external hard drives are showned in the mnt directory

# ls -a
	- `-a` shows hidden files

# Possible exam questions
	- Matching
	- which direcotry is populate dduring r untime
	- whifch file live sin which direcotry

# Which file will have acitvity when poweirng up youtr comptuer ?
	- /var, /log, /boot, /proc, 