# What is a File System?
![Diagram: Overview of File System Structure]
- A file system organizes and stores files on a computer.
- Files are often classified by type.
- **inode (index node)**
	- Stores file metadata such as owner, creation/modification dates, size, and type.
	- Contains pointers to the physical blocks where the file data is stored.
	- To view inode numbers for files, use commands like `ls -i`.

![](img/1.png)

# Linux File System Basics
- Linux does not use drive letters. The system is structured as a single hierarchical tree starting at the root directory `/`.

# Managing Users
- **Adding a User**
	- Command: `sudo adduser username`
	- This command creates a new user and sets up the home directory.

![](img/2.png)

- **Understanding User IDs**
	- User IDs (UIDs) are assigned automatically; for example, UID 1001 might be the next available ID.
	
# Passwords and Authentication
- **Password Storage**
	- Encrypted password hashes are stored in `/etc/shadow`.
	- Use a command like `sudo vim /etc/shadow` to view the file. This is an administrative-privileged file.
	- The system compares the hash in `/etc/shadow` with the hash of the entered password during login.
- **Related Files**
	- `/etc/passwd` stores user account information (no password is in here).

# Groups and Sudoers Configuration
- **/etc/group**
	- Lists all user groups in the system.
	![](img/6.png)
- **/etc/sudoers**
	- The /etc/sudoers file controls who can use sudo and how.
	- Defines which groups or users have administrative privileges.
	- Lists users permitted to execute commands as other users (typically the root).
	- Allows fine-grained control over which administrative privileges a user receives.
	![](img/7.png)

# Privileged vs. Normal Files
- **Privileged Files**
	- Examples: `/etc/shadow`, `/etc/sudoers`
	- These files are restricted and typically only accessible by the root user with sudo permissions.
- **Normal Files**
	- Examples: Files in `/etc/passwd` which provide public user account details (without passwords).

# Executable Files (Binaries)
- Binaries are compiled executable files.
- **/bin**
	- Contains essential user command binaries (e.g., `ls`, `cp`, `mv`).
	![](img/8.png)
- **/sbin**
	- Contains system binaries used primarily by the superuser for system administration.
	![](img/5.png)

# Boot-related Directories
- **/boot**
	- Contains boot loader files and the compressed Linux kernel images.
	- The kernel file (e.g., `vmlinuz-6.8.0-57-generic`) is the image used at boot time.
	- Older kernels 1 version behind may be kept as backups in case the current one fails.
![Image: Boot Directory Details]

# Device Files
- **/dev**
	- Contains device files that represent hardware devices (e.g., printers, disks) and virtual devices.
	- Examples include `/dev/null`, `/dev/tty`, and entries for connected devices.
![Image: Device Files Overview]

# Process and System Information
- **/proc**
	- A virtual filesystem providing process and kernel information.
	- Process directories appear here dynamically when a process is running and disappear when it ends.
	- Files and directories under `/proc` offer insights into system configuration and running processes.

![](img/3.png) 

# User Applications and Libraries
- **/usr**
	- Contains user applications, libraries, and documentation.
	- Typically includes most of the software installed on the system (excluding user data).

# Additional Software
- **/opt**
	- A directory reserved for optional or third-party software that does not adhere to the standard file hierarchy.
		- Zoom, Chrome, Skype
![Image: Optional Software Directory]

# Variable Data Files
- **/var**
	- Contains files that vary in size and content over time, such as logs files
	- Examples:
		- `/var/log`: Contains system log files like `auth.log` and `kern.log`.
![Image: Variable Data Files]

# Mount Points
- **/mnt**
	- A directory used as a mount point for temporarily attaching file systems (e.g., external hard drives, USB devices).
		- Mounting is connecting an external file system to your local file system
	- Often used for manual mounting of storage devices.
![Image: Mount Points Illustration]

# Useful Commands
- **ls -a**
	- The `-a` flag with `ls` shows all files, including hidden files (those beginning with a period).

# Possible Exam Questions
- Matching concepts (e.g., identifying directories like `/bin`, `/sbin`, `/boot` and their roles).
- Questions on determining which directory contains dynamically changing files (e.g., `/var` or `/proc`).
- Examining file structure and hierarchical organization on Linux.

# System Activity at Boot

![](img/4.png)

- During system power-up, multiple directories are involved:
	- `/boot`: Provides the kernel and boot loader.
	- `/var`: Used for logging system events.
	- `/proc`: Contains processes and system information.
![Image: System Boot Process Diagram]

Note: Understanding the Linux file system hierarchy is crucial for system administration, troubleshooting, and security.

# Directories covered
```
/
├── bin
├── boot
├── dev
├── etc
├── home
├── mnt
├── opt
├── proc
├── sbin
├── usr
└── var
```
![Image: Directory Tree Diagram]