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
	- 