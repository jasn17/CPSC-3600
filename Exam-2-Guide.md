# *Exam 2 Expectations* 

---

- Chapters 4, 5, 6
- Documentary + YY videos
- TCP echo server and UDP echo server code + in-class activity
- ~35 Questions give or take, Multiple choice, Free response, Coding, Choose all that applies
- 50 minutes

---
- Different layers and their packaging units
- Application layer addressing unit (port number)
- Know all units for all layers
- What services are provided in the network layer
- Difference between a switch and a router
- True/False questions about TCP and UDP headers
- Header fields and their lengths
- Unix file system
- Types of switching fabrics and how they work
- Classification of IP addresses
- Class A, B, C, D
- CIDR scheme: What is the prefix?
- IP address, subnet mask, broadcast address, network address, loopback address, number of hosts in the network (activity)
- Dijkstra's algorithm
    - How it works: Given a graph, find the shortest path
    - Optimization vs. greedy algorithm: How does it apply to Dijkstra's algorithm?
- Code questions: Some snippets from TCP and UDP
    - Write a piece of code during the exam
    - "Show me how to do X"
- Select all true statements about sockets, network byte order, and Chapter 4/5 concepts
- Different frequencies
    - Wi-Fi, Bluetooth, NFC, AM/FM, wireless standards (not high frequency)
    - Range, pros and cons, and use cases (activity)
- Parity questions
    - Odd and even parity
    - Similar to quiz questions: Find the error
- Channel partitioning protocols
    - Frequency and time
- Random access protocols
    - CSMA, collision avoidance/detection
- Taking turns protocols
- Interference: Red and yellow overlap (refer to textbook picture for understanding each part of what that diagram mean)
- MAC addresses
    - What does broadcasting mean? What is a broadcast address?
    - Linux command to find the broadcast address
- Documentary
    - Rumble (4 major threats)
    - Underwater cable video
    - Ted Talk
- Technical questions (simple facts): Differences between some examples
- Exam format: Paper or lockdown
- Material: PowerPoint + Chapters

---

### How to Improve Memory
- Similar to working out
- Practice brain exercises
- Muscle memory: Use your brain more often
- Memory games
- The more you use your brain while young, the later the onset of dementia

---

### **Linux File System**
- All Linux file systems start at the root `/` directory.
- `/` (root directory)
    - `bin/`: Contains "binary" (executable code)
        - Any program that is executable (aka "binary")
        - All commands are applications (e.g., `ls`, `make`, `cd`)
    - `sbin/`: Superuser applications
        - Requires privileged user access to use these binaries
    - `home/`: User directories
        - Contains everything related to users in the system
    - `dev/`: Physical devices connected to the system
        - Pseudo-devices: Every file is associated with a device
        - Device driver: A program that allows access to a device
        - `stderr`, `stdin`, `stdout`:
            - `/proc/self/fd/2`, `/proc/self/fd/0`, and `/proc/self/fd/1` respectively
    - `proc/`: Running processes
        - Each process has an associated ID, represented as the folder name
    - `etc/`: Configuration files
    - `opt/`: Optional software
        - Software made for Linux but not by Linux (e.g., Skype, Zoom, Chrome)
    - `var/`: Variable-length files
        - `mail/`: System mail (can grow or shrink)
        - `logs/`: Logs system activity (e.g., failed login attempts)
    - `boot/`: Files that boot the OS, loading the kernel into memory
        - Linux kernel: `vmlinuz` (points to the latest kernel version)
