
# Q1] What is Computer Network? Explain Types of Computer Network in brief. 

**Answer:**

A **computer network** is a system that connects multiple computing devices, enabling them to communicate and share resources. These devices can be connected using various methods, including wired cables (like Ethernet) and wireless technologies (like Wi-Fi). 

## Types of Computer Networks

Computer networks are categorized based on their geographical coverage (size) and purpose. Here's a breakdown of the common types:

### 1. Local Area Network (LAN)

* **Coverage:**  Covers a small area, such as a home, office, or school building. 
* **Ownership:** Typically privately owned.
* **Characteristics:** 
    * High data transfer speeds due to short distances.
    * Easier to manage and maintain than larger networks.
* **Examples:**  A home Wi-Fi network, a network in a computer lab.

### 2. Metropolitan Area Network (MAN)

* **Coverage:** Spans a larger geographical area, such as a city or town.
* **Ownership:** Can be private or public.
* **Characteristics:**
    * Connects multiple LANs together within a metropolitan area.
    * Offers moderate data transfer speeds.
* **Examples:** A network connecting different branches of a company within a city, a city-wide cable TV network.

### 3. Wide Area Network (WAN)

* **Coverage:** Covers a vast geographical area, often connecting networks across countries or continents.
* **Ownership:** Typically involves a combination of private and public ownership.
* **Characteristics:**
    * Connects LANs and MANs over long distances.
    * Lower data transfer speeds due to larger distances and complex infrastructure.
* **Example:** The **Internet** is the largest and most well-known WAN.

Here's a table summarizing the key differences:

| Feature       | LAN              | MAN                          | WAN                                 |
|---------------|-------------------|-------------------------------|---------------------------------------|
| **Area**       | Small (building)  | Medium (city)                 | Large (country, continent)          |
| **Speed**      | High             | Moderate                      | Low                                  |
| **Ownership** | Private          | Private or Public             | Private and Public                     |
| **Examples**    | Home network     | University campus network     | The Internet                        | 

# Q2] Answer the following Questions.

## Q2. i) For n devices in a network, what is the number of cable links required for a mesh topology?

**Answer:** In a mesh topology, every device is directly connected to every other device. The number of cable links required for a mesh topology with *n* devices is calculated using the following formula: 

**Number of cable links = n * (n - 1) / 2**

## Q2. ii) Source to Destination delivery of packet is responsibility of which layer?

**Answer:**  The **Network Layer** is responsible for the source-to-destination delivery of packets. It determines the best path for packets to travel across the network from the source host to the destination host, a process known as **routing**.

## Q2. iii) Which layer in the OSI model is responsible for end-to-end communication over a network?

**Answer:**  The **Transport Layer** is responsible for end-to-end communication over a network. It ensures that data is delivered reliably and in the correct order between the sending and receiving applications, regardless of the underlying network infrastructure. 

# Q3] What is topology or Network Topology? Explain different types of topologies.

**Answer:**

**Network Topology** refers to the physical or logical arrangement of nodes (devices like computers, routers, etc.) and the connections (links) between them within a computer network. It defines how the devices are interconnected and how data flows between them. 

## Types of Network Topologies:

There are various types of network topologies, each with its own advantages and disadvantages:

### 1. Bus Topology

* **Structure:** All devices are connected to a single central cable called the "bus" or "backbone."
* **Data Flow:** Data travels in a single direction along the bus.
* **Advantages:**
    * Simple and inexpensive to implement.
    * Easy to add or remove devices.
* **Disadvantages:**
    * A single point of failure (if the bus fails, the entire network fails).
    * Performance degradation with heavy traffic or a large number of devices.
* **Best Suited for:** Small networks with low traffic.

### 2. Ring Topology

* **Structure:** Devices are connected in a closed loop or ring, where each device has exactly two neighbors.
* **Data Flow:** Data travels in a single direction around the ring.
* **Advantages:**
    * Data transmission is relatively efficient.
    * Better performance than a bus topology under heavy traffic.
* **Disadvantages:**
    * A single point of failure (if one device or link fails, the entire network fails).
    * Adding or removing devices can disrupt the network.
* **Best Suited for:** Networks with moderate traffic and a need for fair data access for all devices.

### 3. Star Topology

* **Structure:** All devices are connected to a central hub or switch.
* **Data Flow:** Data flows through the central hub to reach the intended destination.
* **Advantages:**
    * Easy to install and manage.
    * A single device failure does not affect the entire network.
* **Disadvantages:**
    * The central hub is a single point of failure.
    * Can be more expensive than a bus or ring topology due to the central hub.
* **Best Suited for:**  Small to medium-sized networks where ease of management and reliability are important.

### 4. Mesh Topology

* **Structure:** Every device is connected directly to every other device.
* **Data Flow:** Multiple paths exist for data to travel between devices.
* **Advantages:**
    * Highly reliable (multiple paths for data, so a single failure doesn't disrupt the entire network).
    * High fault tolerance.
* **Disadvantages:**
    * Complex and expensive to implement (requires many cables and connections).
    * Difficult to manage.
* **Best Suited for:** Networks where high reliability and redundancy are critical.

### 5. Tree Topology

* **Structure:**  A hierarchical structure with a root node and branches connecting to other devices.
* **Data Flow:**  Data travels along branches to reach specific destinations.
* **Advantages:**
    * Can support a large number of devices.
    * Easier to manage than a mesh topology.
* **Disadvantages:**
    * The root node is a single point of failure.
    * Can be complex to configure.
* **Best Suited for:** Large networks with hierarchical data flow patterns.

### 6. Hybrid Topology

* **Structure:** A combination of two or more different topologies. 
* **Data Flow:** Depends on the specific topologies combined.
* **Advantages:**
    * Flexibility to meet specific network needs.
    * Can combine the advantages of different topologies.
* **Disadvantages:**
    * Can be complex to design and implement.
* **Best Suited for:**  Networks with diverse requirements where a single topology isn't sufficient.

# Q4] Explain the following terms:

These terms all relate to the various delays a data packet encounters as it travels across a network:

## Q4. i) Processing Delay

**Answer:** Processing delay is the time a network device (like a router) takes to examine the header of a data packet. The device will:

* Analyze the packet header to determine the destination.
* Perform error checking on the packet.
* Decide which output link to forward the packet to.

Processing delay is typically very short, measured in **microseconds** or less.

## Q4. ii) Transmission Delay

**Answer:** Transmission delay (also called serialization delay) is the amount of time it takes a device to push all the bits of a data packet onto the transmission link. It depends on two factors:

* **Packet size (L):** The number of bits in the packet.
* **Transmission rate (R):** The link's bandwidth (bits per second).

The formula to calculate transmission delay is:

**Transmission Delay (d<sub>tran</sub>) =  L / R**

Transmission delay is typically measured in **microseconds** or **milliseconds**.

## Q4. iii) Propagation Delay

**Answer:** Propagation delay is the time it takes for a single bit to travel across the physical medium from the sending device to the receiving device. It is determined by:

* **Distance (d):** The physical length of the transmission medium.
* **Propagation speed (s):** The speed at which signals travel through the medium (close to the speed of light in fiber optic cables).

The formula for propagation delay is:

**Propagation Delay (d<sub>prop</sub>) = d / s**

Propagation delay is often measured in **milliseconds**. 

## Q4. iv) Queuing Delay

**Answer:** Queuing delay is the time a packet spends waiting in a queue at a network device before it can be transmitted. It depends on the congestion level at that device:

* **No Congestion:** If the queue is empty, the queuing delay is zero.
* **Heavy Traffic:** If the queue is full or there is a lot of traffic, the queuing delay will be longer.

Queuing delay can vary significantly, ranging from **microseconds** to **milliseconds** or even longer in congested network conditions.


**In summary:** When a packet travels through a network, the total delay it experiences is the sum of these four delays:

**Total Delay = Processing Delay + Queuing Delay + Transmission Delay + Propagation Delay** 




