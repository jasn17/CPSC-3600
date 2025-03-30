## Input: Slide content copy and paste
## Prompt: Ask me 10 detailed exam-like questions about the content including multiple choice, 1 short answer, true/flase, and choose all that applies. Make sure to make the questiosn as specific as possible and throw curveballs. 

1. Multiple Choice:
Which statement best distinguishes between the network layer’s two main functions?
A. Forwarding is implemented in software for flexibility, while routing is implemented in hardware for speed.
B. Forwarding involves moving packets between router ports using hardware, and routing involves computing end-to-end paths using software-based algorithms.
C. Forwarding computes the best path through the network, whereas routing only queues packets for delivery.
D. Both forwarding and routing are performed exclusively by a centralized controller in every router.

# B, Forwarding is done by hardware (moving packets between ports) and routing computes the end-to-end path via software.

2. Multiple Choice:
When an IP datagram exceeds the MTU of a link and is fragmented, which of the following is true?
A. Each fragment carries a complete IP header with identical checksum values as the original datagram.
B. The fragment offset is measured in bytes, and reassembly can occur at any intermediate router.
C. The fragment offset field indicates the position of the fragment’s data in units of 8 bytes, and reassembly is done only at the destination.
D. The "More Fragments" flag is set to 0 for all fragments except the first one.

# C, The fragment offset field is measured in 8-byte units, and reassembly happens only at the destination.

3. True/False:
NAT (Network Address Translation) is often criticized for violating the end-to-end principle because it changes packet headers, which can interfere with end-to-end communications.
• True
• False

# True, NAT does change packet headers, which is one reason it’s seen as violating the end-to-end principle.

4. Short Answer:
Explain the role of DHCP in a network and list at least two additional pieces of information (other than the IP address) that a DHCP server can provide to a client.

# The role of DHCP in dynamically assigning IP addresses, The process of broadcasting, receiving offers, and acknowledgments, Additional configuration details (first-hop router, DNS server, network mask)

5. Multiple Choice:
One of the improvements in IPv6 over IPv4 is its header format. What is the primary benefit of the fixed-length IPv6 header?
A. It increases the header size, which allows more options and error-checking.
B. It removes the need for fragmentation by intermediate routers.
C. It simplifies and speeds up processing/forwarding at each hop by having a fixed and smaller header size.
D. It eliminates the need for routing protocols such as OSPF and BGP.

# C, Removing the need for fragmentation by intermediate routers (option B) is not one of the benefits; fragmentation is handled differently in IPv6.

6. Choose All that Apply:
Select all characteristics that correctly describe switching fabrics in routers:
☐ They determine the speed at which packets are copied from an input port to an output port.
☐ Memory-based switching involves copying the entire packet to system memory, which is limited by memory bandwidth.
☐ Bus-based switching uses a shared bus, which can become a bottleneck if multiple packets contend for the bus simultaneously.
☐ Interconnection network switching, such as crossbar switches, eliminates the need for input and output buffers.

# Memory-based switching involves copying the entire packet to system memory, which is limited by memory bandwidth, Bus-based switching uses a shared bus, which can become a bottleneck if multiple packets contend for the bus simultaneously.

7. Multiple Choice:
Which scheduling mechanism is designed to always transmit the highest-priority packet available from a queue?
A. First-In-First-Out (FIFO)
B. Round Robin (RR)
C. Priority Scheduling
D. Weighted Fair Queuing (WFQ)

# C, Priority Scheduling is used to always send the highest-priority packet from the queue.

8. Multiple Choice:
In an OpenFlow flow table entry, which of the following components is NOT typically included?
A. A match field that specifies header values.
B. An action field that determines what to do with matching packets.
C. A counter that records the number of packets and bytes matched.
D. A memory address pointer for dynamically storing packet payloads.

# D, A memory address pointer for storing packet payloads is not typically part of an OpenFlow flow table entry.

9. True/False:
IP fragmentation can occur at any router along the path if a datagram exceeds the MTU of a link, and reassembly is performed incrementally at each router.
• True
• False

# False, While IP fragmentation can occur along the path, reassembly is performed only at the final destination—not incrementally at each router.

10. Choose All that Apply:
Select all fields that are part of the fixed IPv6 header:
☐ Version
☐ Header Length
☐ Priority
☐ Flow Label
☐ Payload Length
☐ Next Header
☐ Hop Limit

# Version, Flow Label, Payload Length, Next Header, and Hop Limit.