# *Exam 2 Expectations*
- Chapters 4, 5, 6
- DOcumetnaryr

 tcp echo server and udp echo server code, + in-class activity


 50 minutes

 - Differnt layes, packaging units
 - Application layer adddresses unit (port number)
    - KNow all unit for all layers
 - What servcies are provided in the networkk layer
 - Difference ebetwween siwthc an drouyter
 - True/Flase between TCP and UDP headers
    - Field
    - Length of the headers
- Unix file system
- Types of switching fabrics, how they work
- Classicifcation for IP address
    - Class A, B ,C , D
    - Slider scheme what is that prefix?
- IP address, mask, braodcast address, address of teh nw, lookback address, number of host in the nw (activity)
- Dijkastra algorithm
    - How does it work, given a graph, find shortest path
- Immun ization vs optimzation , what i greedy algo and how does rthat apply to dijktra
- COde questions some snippets from TCP adn some from UDP
    - Write a piece of code o this exam
    - "Show me how to do x"
- Select all true statmenets below about socket, nw byte order, chapter 4/5 stuff
- different frequncies
- wifi, blue tooth, nfc, AM/FM, wireless standard (not high frequency)
    - What is the range, pros and cons, where are they used (activity)
- Parity questions
    - Odd and even parity
    - Similar to parity questions on the quiz, find the error
- Channel partiitoning protocol 
    - Ffreqneucy, time
- Random access protocols
    - CSMA, collision advoidance/detection
- Taking turns protocols
    - Interference red and yellow overlap, look at the picture and understand what it means (textbook)
- Mac addresses
- What does borad casrtin mean, what is broadcast address
- What linux command to find that
- Documentary
    - rumble (4 major threats)
    - Underwater cable video
    - Ted Talk
    - technical questions (simple facts), Differnce ebetween sum emp 
- Paper or lockdown
- Material: Powerpoint + Chapter
- 

How to improve memory
- like working out
- practice brain stuff
- muscle memory, use your brain more often
- Memory games
- More your use your brain while young the later the onset dimentia

**Linux file system**
- All linux file system start at root/ directory
- "/" root directory
    - bin/, home/, boot/, dev/
        - boot/ files that boot your OS, loading kernal into memory
            - Linux kernal, vmlinuz (points to the latest version of the kernal)
        - bin/ contians "binary" (executbale code)
            - any program that is executbale (aka "binary")
            - all commands are applications (ls, make, cd) <- all names of applications
        - sbin/ superuser applications
            - you must be a privlage user to use these binary
        - home/
            - where the users live, folder for everything user in your system
        - dev/
            - physical devices connected to your laptop
            - Sudo devices, every file is associated with that device
            - Device driver, a prorgam that allows you to access that device
            - stderr stdin stdout
                - proc/self/fd/2, 0, and 1 respectively
        - proc/ runs processes
            - all process has a number associated with it, the name of the folder is the 
                id of teh processes running somewhere in teh system
        - etc/ mostly config files  
        - opt/ optional software
            - made for linux but not by linux
            - skype, zoom, chrome
        - var/ various lengths files
            - mail/ mail that arrives tot he system, mail can grow (get mail) or shrink (delete mail) so size is variable
            - logs/ logs the system activity, user has a failed login attempt
            - 
