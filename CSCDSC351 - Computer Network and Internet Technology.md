
# Section A

## Q1. Explain the structure of the Internet. Discuss the client-server concept, Internet protocols, and Internet addressing (IP address) in detail.

### Answer:

### Structure of the Internet

The Internet is a **global network of interconnected networks (network of networks)**. It consists of:

- **End Systems (Hosts)** – PCs, servers, smartphones
- **Access Networks** – DSL, Cable, Wi-Fi, Fiber
- **Routers** – Forward packets between networks
- **ISPs (Internet Service Providers)** – Provide connectivity
- **Backbone Networks** – High-speed core networks

### Client-Server Concept

The **Client-Server model** is a distributed architecture in which:

- **Client** requests services
- **Server** provides services

#### Characteristics:
- Centralized control
- Request-response mechanism
- Supports scalability and resource sharing

**Example:**  
Web Browser (Client) communicates with Web Server (Server).

### Internet Protocols

Communication over the Internet is governed by protocols:

- **IP (Internet Protocol)** – Logical addressing and routing
- **TCP (Transmission Control Protocol)** – Reliable, connection-oriented
- **UDP (User Datagram Protocol)** – Fast, connectionless
- **HTTP** – Web communication
- **FTP** – File transfer
- **SMTP** – Email transmission
- **DNS** – Domain name resolution

### Internet Addressing (IP Address)

An IP address uniquely identifies a device on a network.

#### IPv4:
- 32-bit address
- Dotted decimal notation (e.g., 192.168.1.1)

#### IPv6:
- 128-bit address
- Hexadecimal notation

---

## Q2. Describe the basic structure of an HTML document. Explain different HTML tags and illustrate how to create lists, hyperlinks, and tables with suitable examples.

### Answer:
#### 1. Basic Structure of an HTML Document

Every standard HTML5 document begins with a document type declaration followed by the root `<html>` element.


```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>My First Webpage</title>
</head>
<body>
    <h1>Welcome to My Website</h1>
    <p>This is a simple paragraph of text.</p>
</body>
</html>
```

#### Essential Tags

- **`<!DOCTYPE html>`**: Tells the browser that the document is an HTML5 file.
    
- **`<html>`**: The root element that wraps all content on the page.
    
- **`<head>`**: Contains metadata (information about the document), such as the title and character set, which aren't displayed on the page itself.
    
- **`<title>`**: Sets the text shown in the browser’s title bar or tab.
    
- **`<body>`**: Contains the visible content of the webpage (text, images, links, etc.).

#### 2. Creating Lists

HTML supports two primary types of lists: **ordered** (numbered) and **unordered** (bulleted).

##### Unordered List (`<ul>`)

Used when the order of items doesn't matter. Each item is wrapped in an `<li>` (list item) tag.

```html
<ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ul>
```

##### Ordered List (`<ol>`)

Used for sequences or rankings.

```html
<ol>
    <li>Open the editor</li>
    <li>Write the code</li>
    <li>Save as .html</li>
</ol>
```

#### 3. Hyperlinks (`<a>`)

Hyperlinks allow users to navigate between pages. They are created using the **anchor** tag (`<a>`) with the `href` (hyperlink reference) attribute.


```html
<a href="https://www.google.com" target="_blank">Visit Google</a>
```

- **`href`**: The URL or destination path.
    
- **`target="_blank"`**: An optional attribute that opens the link in a new tab.

#### 4. Tables (`<table>`)

Tables are used to display data in a grid format consisting of rows and columns.
##### Table Components

- **`<table>`**: The wrapper for the entire table.
    
- **`<tr>`**: Represents a **Table Row**.
    
- **`<th>`**: Represents a **Table Header** (bold and centered by default).
    
- **`<td>`**: Represents **Table Data** (a standard cell).


##### Example Table


```html
<table border="1">
    <tr>
        <th>Language</th>
        <th>Year Released</th>
    </tr>
    <tr>
        <td>HTML</td>
        <td>1991</td>
    </tr>
    <tr>
        <td>JavaScript</td>
        <td>1995</td>
    </tr>
</table>
```
---

## Q3. Explain HTML Forms and Multimedia in HTML. Discuss the commonly used form elements and attributes with examples.

### Answer:

### HTML Forms

An HTML form is defined using the `<form>` element. It acts as a container for different types of input elements, such as text fields, checkboxes, and radio buttons.

```html
<form action="submit.php" method="post">
  Name: <input type="text" name="username"><br>
  Password: <input type="password" name="pass"><br>
  <input type="submit" value="Submit">
</form>
```

---

### Common Form Elements

- `<input>`
- `<textarea>`
- `<select>`
- `<option>`
- `<button>`

### Common Attributes

- action  
- method  
- name  
- value  
- required  
- placeholder  

---

### Multimedia in HTML
Multimedia refers to content that combines different forms such as text, audio, images, animations, and video
#### Audio

```html
<audio controls>
  <source src="song.mp3" type="audio/mpeg">
</audio>
```

#### Video

```html
<video controls width="400">
  <source src="video.mp4" type="video/mp4">
</video>
```

---

## Q4. What is XML? Explain the need for XML and discuss its advantages over HTML.

### Answer:

### What is XML?

XML (Extensible Markup Language) is a markup language designed to store and transport structured data.


### Need for XML

- Platform-independent data exchange  
- Structured data representation  
- Data sharing between applications  
- Self-descriptive format  

### Advantages of XML over HTML

| XML | HTML |
|-----|------|
| Designed to store data | Designed to display data |
| User-defined tags | Predefined tags |
| Strict syntax rules | Flexible syntax |
| Self-descriptive | Not self-descriptive |

---

# Section B

## Q5. Discuss different network topologies with diagrams. Give advantages and disadvantages.

### Answer:
## 1. Mesh Topology

In a mesh topology, every device has a dedicated **point-to-point link** to every other device. "Dedicated" means the link carries traffic only between the two devices it connects.
![[Pasted image 20260215112108.jpg]]

- **Number of Links:** For n devices, the number of physical links is 2n(n−1)​.
    
- **Advantages:**
    
    - **Robustness:** If one link fails, it does not affect the entire system.
        
    - **Privacy/Security:** Dedicated lines ensure only the intended recipient receives the message.
        
    - **Fault Identification:** Problems are easily isolated and traced.
        
- **Disadvantages:**
    
    - **Cost:** High amount of cabling and number of I/O ports required.
        
    - **Installation:** Physical implementation is difficult due to the bulk of wiring.

## 2. Star Topology

Each device has a dedicated point-to-point link only to a **central controller**, usually called a **hub** or switch. The devices are not directly linked to one another.

![Image of Star Network Topology](https://encrypted-tbn1.gstatic.com/licensed-image?q=tbn:ANd9GcTjaYYNvRQaU0j78lLkAibzYSpSwM3J1t71A_wbsXzwLBLN9-UBX2ejOkf5DbzEgtQIqxlYeLVggenfG7-EfMUaP7WglqOBpwNSqCnTZd0c4RXKtqY)

- **Advantages:**
    
    - **Lower Cost:** Less expensive than mesh; each device needs only one link and one I/O port.
        
    - **Robustness:** If one link fails, only that device is affected.
        
    - **Easy Installation:** Adding or removing devices involves only one connection to the hub.
        
- **Disadvantages:**
    
    - **Dependency:** If the central hub goes down, the entire network fails.
        
    - **Cabling:** While less than mesh, it still requires more cable than bus or ring.

## 3. Bus Topology

A bus topology is **multipoint**. One long cable (the backbone) acts as a single communication line that links all the devices in the network.

![Image of Bus Network Topology](https://encrypted-tbn0.gstatic.com/licensed-image?q=tbn:ANd9GcTK_OjrjCTGrNTMETQ17qyDjVBeVP5LXjNkoqeGxIeYq-NxYzN76Abffg--yFyZbwkOeKq7caMSta51rVsgMVJWZutycDS5fQAYVS4619eTkUhnOTk)

- **Mechanism:** Nodes are connected to the bus cable by drop lines and taps.
    
- **Advantages:**
    
    - **Ease of Installation:** Uses the least amount of cabling among the topologies.
        
    - **Redundancy:** Simple to connect a new node to the backbone.
        
- **Disadvantages:**
    
    - **Difficult Reconfiguration:** Adding new devices may require modifying the backbone.
        
    - **Fault Isolation:** A fault or break in the bus cable stops all transmission.
        
    - **Signal Reflection:** Signal reflection at the taps can cause degradation.


## 4. Ring Topology

Each device has a dedicated point-to-point connection with only the **two devices on either side** of it. A signal is passed along the ring in one direction until it reaches its destination.

![Image of Ring Network Topology](https://encrypted-tbn1.gstatic.com/licensed-image?q=tbn:ANd9GcQ60eu1WaPlkFH41HCoRWv8D-afAEOk-eaEhKOGcl0ZMvO04tYVs3e8li4KHJj2ctLHJOE4gxupFvJBfwfZERN-wup6XgGpV-ClP_lbl4cd9JseGTM)


- **Mechanism:** Each device incorporates a repeater to strengthen the signal.
    
- **Advantages:**
    
    - **Simplified Installation:** Each device is linked only to its immediate neighbors.
        
    - **Fault Isolation:** Simplified; a signal usually circulates a pattern, and an alarm can alert the network operator to the break location.
        
- **Disadvantages:**
    
    - **Unidirectional Traffic:** A break in the ring (in a basic configuration) can disable the entire network.
        
    - **Latency:** Signals must pass through every intermediate node to reach the destination.


---

## Q6. Explain the OSI model. Describe all seven layers and their functions.

### Answer:
The **OSI (Open Systems Interconnection)** model, introduced by the ISO, is a theoretical framework used to understand and design network architecture. It divides the complex task of data communication into **seven distinct layers**, each with specific functions. *(Top Down Approach for the layers is given below:)*

### 7. Application Layer

The topmost layer provides the interface between the user and the network. It supports software applications like email, file transfers, and remote logins.

- **Functions:** Network virtual terminal, file transfer, access and management (FTAM), mail services, and directory services.


### 6. Presentation Layer

This layer acts as a translator for the network. It ensures that information sent by the application layer of one system is readable by the application layer of another.

- **Functions:** **Translation** (encoding/decoding), **Encryption/Decryption**, and **Compression**.

### 5. Session Layer

The session layer establishes, maintains, and synchronizes the interaction between communicating systems.

- **Functions:** **Dialog control** (half-duplex or full-duplex) and **Synchronization** (adding checkpoints to data streams to allow recovery from crashes).

### 4. Transport Layer

Responsible for the **process-to-process delivery** of the entire message. While the Network layer handles end-to-end delivery of individual packets, the Transport layer ensures the whole message arrives intact and in order.

- **Functions:** Service-point (port) addressing, segmentation and reassembly, connection control, flow control, and error control.

### 3. Network Layer

The network layer is responsible for the **source-to-destination delivery** of a packet across multiple networks (links).

- **Functions:** **Logical addressing** (IP addresses) and **Routing** (determining the best path for data).

### 2. Data Link Layer

This layer transforms the physical layer (a raw transmission facility) into a reliable link. It makes the physical layer appear error-free to the upper layers.

- **Functions:** Framing, **Physical addressing** (MAC addresses), flow control, error control, and access control.

### 1. Physical Layer

The lowest layer coordinates the functions required to carry a bit stream over a physical medium. It deals with the mechanical and electrical specifications of the interface and transmission medium.

- **Functions:** Physical characteristics of interfaces/medium, representation of bits (encoding), data rate, synchronization of bits, and line configuration.


---

## Q7. Discuss Frequency Division Multiplexing (FDM) and Time Division Multiplexing (TDM). Compare them with suitable examples.

### Answer:
### 1. Frequency Division Multiplexing (FDM)

FDM is an **analog** technique used when the bandwidth of a link is greater than the combined bandwidths of the signals to be transmitted.   

- **Mechanism:** Each sending device produces signals in different frequency ranges. these signals are modulated onto different **carrier frequencies**, which are then combined into a single composite signal.   
- **Example:** **AM/FM Radio Broadcasting**. The air is the common medium, and various stations travel simultaneously through it. Your receiver tunes into a specific frequency (channel) to "demultiplex" the signal.


### 2. Time Division Multiplexing (TDM)

TDM is a **digital** process that allows several connections to share the high bandwidth of a link by dividing the total time among them. Instead of sharing a portion of the frequency, each connection occupies the **entire bandwidth** for a fraction of the time.   

There are two main types:

1. **Synchronous TDM:** The multiplexer allocates a fixed time slot to each device, even if the device has no data to send. This can lead to "empty" slots and wasted bandwidth.   
- **Example:** **Digital Telephony (T-1 lines)**. Multiple voice calls are digitized and sampled, with samples from different calls interleaved into a single high-speed bitstream.

---

## Q8. Explain Circuit Switching and Packet Switching. Compare their working principles and applications.

### Answer:

### 1. Circuit Switching

Circuit switching creates a **dedicated physical path** between two nodes for the entire duration of the communication. This path is a connected sequence of physical links between nodes.   

#### Working Principle

1. **Setup Phase:** Before data can be sent, a dedicated circuit must be established from end to end.   
    
2. **Data Transfer:** Once the circuit is established, data flows in a continuous stream.   
    
3. **Teardown Phase:** When one of the parties needs to disconnect, a signal is sent to release the resources (dedicated bandwidth) along the path.   

### 2. Packet Switching

In packet switching, there is no resource reservation or dedicated path. Instead, messages are divided into smaller units called **packets**. Each packet is treated independently and contains source and destination addresses.   

#### Working Principle

Each packet is transmitted individually. A switch receives a packet, stores it briefly, and then forwards it to the next node based on its destination address. This is known as **Store-and-Forward** transmission.   

There are two approaches to packet switching:

1. **Datagram Approach:** Each packet is independent; different packets of the same message may take different routes and arrive out of order.   
    
2. **Virtual-Circuit Approach:** A logical path is planned before transmission, and all packets follow that same path, though resources are still not "reserved" exclusively.

####  Comparison Table

| Feature                  | Circuit Switching                     | Packet Switching                       |
| ------------------------ | ------------------------------------- | -------------------------------------- |
| **Path**                 | Dedicated physical path.              | No dedicated path (dynamic).           |
| **Resource Reservation** | Reserved in advance (Guaranteed).     | No reservation (On-demand).            |
| **Wastage**              | High (if the line is idle).           | Low (efficient use of bandwidth).      |
| **Delay**                | Initial setup delay, then negligible. | Per-packet delay (Store-and-Forward).  |
| **Congestion**           | Occurs during the setup phase.        | Occurs at each node (Buffer overflow). |
| **Application**          | Traditional Telephone (Voice).        | Internet, Data communication.          |
  
---

## Q9. Discuss different transmission media. Explain guided and unguided media with examples.

### Answer:
#### 1. Guided Media (Wired)

Guided media provide a physical conduit from one device to another. The signal is "guided" along a specific solid path.   

##### A. Twisted-Pair Cable

Consists of two insulated copper wires twisted together. Twisting helps reduce **crosstalk** and electromagnetic interference.   

- **Types:** Unshielded Twisted-Pair (UTP) and Shielded Twisted-Pair (STP).   
    
- **Applications:** Local telephone lines, DSL, and LANs (Ethernet).   


##### B. Coaxial Cable

Carries signals of higher frequency ranges than twisted-pair. It has a central core conductor (usually copper) enclosed in an insulating sheath, which is then encased in an outer conductor (braid/foil).   

- **Applications:** Cable TV networks and traditional Ethernet (Thinnet/Thicknet).   


##### C. Fiber-Optic Cable

Made of glass or plastic and transmits signals in the form of **light**. It uses the principle of **total internal reflection**.   

- **Advantages:** Extremely high bandwidth, immunity to electromagnetic interference (EMI), and low attenuation.   
    
- **Applications:** Backbone networks and high-speed internet.   


#### 2. Unguided Media (Wireless)

Unguided media transport electromagnetic waves without using a physical conductor. This is commonly referred to as **wireless communication**.   

##### A. Radio Waves

Electromagnetic waves ranging in frequencies between 3 kHz and 1 GHz. They are **omnidirectional**—when an antenna transmits radio waves, they are propagated in all directions.   

- **Applications:** AM/FM radio, television, and maritime radio.   
  

##### B. Microwaves

Electromagnetic waves with frequencies between 1 GHz and 300 GHz. Unlike radio waves, microwaves are **unidirectional**; the sending and receiving antennas must be aligned (Line-of-Sight).   

- **Applications:** Satellite networks and terrestrial microwave links.   

##### C. Infrared

High-frequency waves (300 GHz to 400 THz) used for short-range communication. They cannot penetrate walls, which prevents interference between systems in adjacent rooms.

- **Applications:** TV remote controls and wireless mice/keyboards.

---

