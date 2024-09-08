## 1. What is a Computer Network? Explain types of Computer Networks in brief.

**Answer:**

A **computer network** is a collection of interconnected computing devices that can communicate and share resources. These devices can be computers, servers, smartphones, printers, or any other device capable of sending and receiving data. The connections between them can be wired (using cables like Ethernet) or wireless (using technologies like Wi-Fi or Bluetooth). 

**Types of Computer Networks:**

**1. LAN (Local Area Network):**
* **Scope:**  Limited to a small geographical area like a home, office building, school, or campus.
* **Ownership:** Typically privately owned and managed by a single organization.
* **Technologies:** Uses Ethernet (wired) and Wi-Fi (wireless) as common technologies.
* **Characteristics:**
    * High data transfer rates (bandwidth).
    * Relatively low cost to set up and maintain.
    * Easy to manage and troubleshoot. 
* **Examples:** A home network, office network, school computer lab.

**2. MAN (Metropolitan Area Network):**
* **Scope:** Covers a larger geographical area than a LAN, such as a city or town. 
* **Ownership:** Can be owned by a single organization (like a large company) or a service provider.
* **Technologies:**  Often uses a combination of technologies, including fiber optic cables, high-speed wireless links, and leased lines.
* **Characteristics:**
    * Provides higher bandwidth than LANs.
    * Can connect multiple LANs within a metropolitan area.
* **Examples:** A network connecting different branches of a company within a city, a city-wide Wi-Fi network.

**3. WAN (Wide Area Network):**
* **Scope:** Spans a very large geographical area, often connecting different countries or continents.
* **Ownership:** Typically owned and operated by telecommunication companies or large service providers.
* **Technologies:** Uses a variety of long-distance technologies, including satellites, fiber optic cables, undersea cables, and microwave links.
* **Characteristics:** 
    * Covers vast distances.
    * Lower bandwidth compared to LANs and MANs due to longer distances and the use of shared resources.
    * More complex to manage and troubleshoot.
* **Example:**  The **Internet** is the largest and most well-known WAN.

## 2. Answer the following Questions.

### i) For n devices in a network, what is the number of cable links required for a mesh topology?

**Answer:** In a **mesh topology**, every device has a point-to-point connection with every other device in the network. The formula to calculate the number of cable links needed is:

**n * (n-1) / 2**

where 'n' is the number of devices. 

**Example:** If you have 5 devices (n=5), you would need 5 * (5-1) / 2 = **10 cable links**.

### ii) Source to Destination delivery of packet is responsibility of which layer?

**Answer:** The **Network Layer** (Layer 3 of the OSI model) is responsible for delivering packets from the source host to the destination host, potentially across multiple networks.  This layer handles:

* **Logical Addressing:** Using IP addresses to identify source and destination hosts.
* **Routing:** Determining the best path for packets to travel through the network.

### iii) Which layer in the OSI model is responsible for end-to-end communication over a network?

**Answer:** The **Transport Layer** (Layer 4 of the OSI model) is responsible for end-to-end communication. This means it ensures reliable data transfer between the application processes running on the source and destination hosts.  The transport layer:

* **Segments and Reassembles Data:** Breaks larger messages into smaller segments for transmission and reassembles them at the destination.
* **Provides Reliability:**  Uses mechanisms like acknowledgements and retransmissions (in protocols like TCP) to ensure data is delivered without errors and in the correct order.
* **Manages Flow Control:** Prevents a fast sender from overwhelming a slow receiver.

## 3. What is topology or Network Topology? Explain different types of topologies.

**Answer:**  A **Network Topology** describes the arrangement or physical layout of devices and connections in a network.  It defines how the devices are interconnected and how data flows between them.

**Types of Topologies:**

* **Bus Topology:**
    - All devices are connected to a single shared cable (the bus).
    - Simple and inexpensive, but a single cable failure can bring down the entire network.
* **Ring Topology:**
    - Devices are connected in a closed loop (ring).
    - Data travels in one direction, passing through each device until it reaches its destination.
    - Less susceptible to a single point of failure than a bus, but can be slow for large networks. 
* **Star Topology:** 
    - All devices connect to a central hub or switch.
    - Easy to install, manage, and troubleshoot, as each device has its own dedicated connection.
    - The most common topology used today.
* **Mesh Topology:**
    - Every device has a direct connection to every other device.
    - Highly reliable and redundant, but very expensive to implement.
* **Tree Topology:**
    - A hierarchical structure with a root node and branches.
    - Combines aspects of star and bus topologies.
    - Good for large networks, but can be complex to manage. 
* **Hybrid Topology:**
    - Combines two or more of the above topologies. 
    - Allows flexibility in network design to meet specific requirements. 

## 4. Explain following terms:

### i) Processing Delay

**Answer:**  **Processing delay** is the time a router takes to examine a packet's header, decide where to forward the packet, and perform any other necessary processing. It also includes the time to check for bit-level errors. It's usually a very short delay, on the order of microseconds or less.

### ii) Transmission Delay

**Answer:**  **Transmission delay** is the time it takes to push all the bits of a packet onto the transmission link. It's calculated as **L/R**, where **L** is the length of the packet (in bits) and **R** is the transmission rate of the link (in bits per second). Transmission delay can range from microseconds to milliseconds depending on packet size and link speed. 

### iii) Propagation Delay

**Answer:** **Propagation delay** is the time it takes for a signal (a single bit) to travel from the beginning of the transmission link to the other end.  It's calculated as **d/s** where **d** is the distance of the physical link and **s** is the propagation speed of the signal in the medium.  Propagation delay depends on the physical medium (fiber, copper, etc.) and is usually on the order of milliseconds.

### iv) Queuing Delay 

**Answer:** **Queuing delay** is the time a packet spends waiting in the queue at the output link of a router before it can be transmitted. This delay depends on the amount of congestion at the router.  If there is no congestion, the queuing delay is zero. If the queue is full, the delay can be very significant (milliseconds or even longer). 

## 5. What is Transmission Media? Explain different types of Transmission Media.

**Answer:** **Transmission Media** is the physical path through which data signals are transmitted between network devices.

**Types of Transmission Media:**

**Guided (Wired) Media:**
* **Twisted-Pair Cable:**
    - Two insulated copper wires twisted together to reduce interference.
    - Common in telephone lines and Ethernet LANs.
    - **UTP (Unshielded Twisted Pair):** Most common, less expensive, used for shorter distances.
    - **STP (Shielded Twisted Pair):**  Better protection from interference, used for longer distances and higher speeds.
* **Coaxial Cable:**
    - A central conductor surrounded by an insulator and a braided shield. 
    - Good for high bandwidth and resistance to interference. 
    - Used in cable TV and some high-speed networks.
* **Fiber Optic Cable:**
    - Transmits data as light pulses through thin glass fibers.
    - Very high bandwidth, low attenuation (signal loss), and immune to electromagnetic interference.
    - Used in long-distance, high-speed networks, and high-performance computing.

**Unguided (Wireless) Media:**
* **Radio Waves:**
    - Omnidirectional signals that travel through the air.
    - Used in Wi-Fi, cellular networks, and radio broadcasting.
* **Microwaves:**
    - High-frequency radio waves that travel in straight lines.
    - Used in satellite communication and long-distance terrestrial links. 
* **Infrared:**
    - Short-range signals used in TV remotes, data transfers between devices in close proximity.

## 6. Differentiate between connection-oriented versus connectionless services in Networks.

**Answer:**

| Feature             | Connection-Oriented Service                                       | Connectionless Service                                    |
|---------------------|------------------------------------------------------------------|-----------------------------------------------------------|
| **Connection Setup**|  Requires a connection setup phase (like a phone call)             | No connection setup needed (like sending a letter)        |
| **Data Flow**       | Data transmitted as a continuous stream                         | Data transmitted as individual packets (datagrams)       |
| **Packet Order**    | Guaranteed in-order delivery of packets                            | Packets may arrive out of order                           |
| **Reliability**     | Generally more reliable due to error control and retransmissions | Less reliable, some packets may be lost                   |
| **Examples**        | TCP, Virtual Circuit Networks                                 | UDP, Datagram Networks                                 |

**Connection-oriented services** are like having a dedicated phone call - you set up a connection, then talk continuously, and then hang up. **Connectionless services** are like sending letters - each letter (packet) is independent and may arrive in a different order.

## 7. Difference between Circuit Switching and Packet Switching.

**Answer:**

| Feature             | Circuit Switching                                        | Packet Switching                                  |
|---------------------|----------------------------------------------------------|-----------------------------------------------------|
| **Connection**       | Dedicated path established between source and destination | No dedicated path; packets share network resources |
| **Bandwidth**         | Fixed bandwidth allocated for the duration of the call      | Dynamic bandwidth sharing                          |
| **Delay**            |  Initial connection setup delay; less delay during data transfer |  Variable delay depending on network congestion   |
| **Efficiency**        | Less efficient, bandwidth wasted if not in constant use     | More efficient, better resource utilization        |
| **Applications**     | Traditional phone calls, applications requiring guaranteed bandwidth |  Internet, data transfer, most modern applications  |


**Circuit switching** is like having a dedicated physical line (like a phone line). **Packet switching** is like sending data in small packets that are routed independently through the network.

## 8. Define the following terms:

### i) Delay
**Answer:**  **Delay** is the time it takes for a data packet to travel from the source to the destination in a network.  It's a combination of processing delay, queuing delay, transmission delay, and propagation delay. 

### ii) Loss 
**Answer:** **Loss** refers to the situation when data packets transmitted over a network fail to reach their destination. It can be caused by network congestion, errors in transmission, or faulty equipment.

### iii) Throughput
**Answer:** **Throughput** is the actual rate at which data is successfully delivered from the source to the destination. It's usually measured in bits per second (bps).

### iv) Packet Delivery Ratio.
**Answer:** **Packet Delivery Ratio (PDR)** is a metric that shows the percentage of data packets that are successfully delivered to the destination.  It is calculated as:

**(Number of packets received) / (Number of packets sent) * 100%**

## CO1 
**(Assuming CO1 refers to a set of related questions):**

## 9. How long does it take to send a file of 640,000 bits from host A to host B over a circuit-switched network?
• All links are 1.536 Mbps
• Each link uses TDM with 24 slots/sec
• 500 msec to establish end-to-end circuit.

**Answer:** 

First, calculate the transmission time for the file on a single link: 

* Transmission Time = File size / Link rate = 640,000 bits / 1.536 Mbps = 0.416 seconds.

Now, consider the TDM: 
* Each slot duration = 1/24 seconds = 41.66 ms.

Since we need to fit the entire file into one slot, the transmission will take at least one slot duration. Therefore:

* Total Time = Connection setup time + Transmission time in one slot
               = 500 ms + 41.66 ms 
               = **541.66 ms**

## 10. How long does it take to send a file of 640,000 bits from host A to host B over a circuit-switched network?
• All links are 1.536 Mbps
• Each link uses FDM with 24 slots/sec
• 500 msec to establish end-to-end circuit.

**Answer:** In FDM (Frequency Division Multiplexing), each connection gets a dedicated portion of the bandwidth. So, the transmission time is not affected by the number of slots. We only need to consider the connection setup time and the time to transmit the entire file on a single link:

* Total Time = Connection setup time + Transmission time 
               = 500 ms + 0.416 seconds (calculated in the previous question)
               = **916 ms**

## 11. A network with a bandwidth of 10 Mbps can pass only an average of 12,000 frames per minute with each frame carrying an average of 10,000 bits. What is the throughput of this network? (Hint: Refer definition of throughput).

**Answer:**

**Throughput** is the amount of data successfully transmitted per unit of time.

* Data transmitted per minute = 12,000 frames * 10,000 bits/frame = 120,000,000 bits
* Throughput = Data per minute / 60 seconds = 120,000,000 bits / 60 seconds = **2 Mbps**

Even though the network bandwidth is 10 Mbps, the actual throughput is only 2 Mbps, likely due to overhead and other network inefficiencies.

## 12. What is bit and byte stuffing? Explain with example.

**Answer:** 

**Bit Stuffing and Byte Stuffing** are techniques used in data link layer protocols for framing - distinguishing one frame from the next in a continuous bit stream. This is necessary because the data itself might contain bit patterns that could be mistaken for frame delimiters.

**Bit Stuffing:**
- **Problem:** If a flag bit pattern (e.g., 01111110) occurs within the data, it could be misinterpreted as the end of the frame.
- **Solution:**  After every sequence of five consecutive '1' bits in the data, an extra '0' bit is inserted (stuffed). The receiver removes this stuffed '0' bit to restore the original data.
- **Example:** 
    - **Original data:**  01111110111111110
    - **After bit stuffing:** 011111**0**1011111**0**110 

**Byte Stuffing (or Character Stuffing):**
- **Problem:** Similar to bit stuffing, but using special bytes as delimiters. If the delimiter byte appears within the data, it can cause problems.
- **Solution:** An escape byte (ESC) is inserted before every occurrence of the delimiter byte within the data. The receiver removes the escape byte to get the original data.
- **Example:**
    - **Flag byte (delimiter):**  DLE (Data Link Escape)
    - **Original data:**  Data DLE More Data
    - **After byte stuffing:** Data **ESC DLE** More Data 

## 13. Draw OSI Reference Model. Explain the functionality of each layer in brief. 

**Answer:** 

**(Drawing -  Please refer to the diagram of the OSI model in the provided material. You can easily find it online as well.)**

**OSI (Open Systems Interconnection) Reference Model:**

| Layer               | Functionality                                                           |
|---------------------|--------------------------------------------------------------------|
| **Application (7)**     | Provides services to user applications (e.g., email, web browsing)     |
| **Presentation (6)**   | Data formatting, encryption, compression                              |
| **Session (5)**       | Manages sessions between applications (dialog control, synchronization)  |
| **Transport (4)**     | Reliable end-to-end data transfer, segmentation, flow control         |
| **Network (3)**       | Routing of packets, logical addressing (IP addresses)                 |
| **Data Link (2)**      | Framing, error control, MAC addressing                                |
| **Physical (1)**      | Physical transmission of bits over the medium (cables, signals)      |


**Mnemonics to Remember the Layers:** 
* **Please Do Not Throw Sausage Pizza Away** (from top to bottom)
* **All People Seem To Need Data Processing** (from bottom to top) 

## 14. Draw the layered architecture of TCP/IP model and write at least two services provided by each layer of the model.

**Answer:** 

**(Drawing - Please refer to the diagram of the TCP/IP model in the provided material or search online.)**

**TCP/IP Model:**

| Layer              | Services                                                                                |
|---------------------|-------------------------------------------------------------------------------------------|
| **Application (5)**    | - Provides services like email (SMTP), web (HTTP), file transfer (FTP).              |
|                     | - Defines how applications interact with the transport layer.                               |
| **Transport (4)**    | - Provides end-to-end communication using TCP and UDP.                                   |
|                     | - TCP: Reliable, connection-oriented data transfer.                                    |
|                     | - UDP: Unreliable, connectionless data transfer.                                       |
| **Internet (3)**      | - Routing of packets across different networks.                                           |
|                     | - Logical addressing using IP addresses.                                                 |
| **Network Access (2)** | - Defines protocols for accessing the physical network (e.g., Ethernet, Wi-Fi).             |
|                     | - Handles physical addressing (MAC addresses) and error detection.                    |

**Note:** The TCP/IP model collapses the Presentation and Session layers of the OSI model into the Application layer.


Let me know if you have any more questions! 
