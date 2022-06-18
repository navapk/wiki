# Introduction to TCP/IP Networking

- Protocols are agreements of a particular part of how a network should work.
- Networking models define a structure and different categories (layers) of standards and protocols.
- The IT world refers to a network created by one corporation, or enterprise, for the purpose of allowing its employees to communicate as an _enterprise network_.
- The smaller network at home, when used for business purposes, often go by the name small office/home office (SOHO) networks.
- A _networking model_, sometimes called either a _networking architecture_ or _networking blueprint_, refers to a comprehensive set of documents. Individually, each documents describe one small function required for a network; collectively, these documents define everything that should happen for a computer network to work.
- Some documents define a _protocol_, which is a set of logical rules that devices must follow to communicate.
- ISO created a networking model **Open Systems Interconnection** (OSI), which had a noble goal: to standardize data networking protocols to allow communication among all computers across the planet.
- US Department of Defense created another open networking model called **TCP/IP**.
- The TCP/IP model defines and references a large collection of protocols that allow computers to communicate.
- TO define a protocol, TCP/IP uses documents called _Requests for Comments_ (RFCs).
- The vendors that created the hardware and software implemented TCP/IP.
- TCP/IP Model:
    | Application |
    | Transport   |
    | Network     |
    | Data Link   |
    | Physical    |
- Example Protocols:
    | TCP/IP Layer         | Protocols               |
    |----------------------|-------------------------|
    | Application          | HTTP, POP3, SMTP        |
    | Transport            | TCP, UDP                |
    | Internet             | IP, ICMP                |
    | Data Link & Physical | Ethernet, 802.11 (WiFi) |
- **Application Layer**: Provide services to the application running software on a computer. The application layer does not define the application itself, but it defines services that application need. For ex, application protocol HTTP defines how web browsers can pull the contents of a web page from a web server. In short, the application layer provides an interface between software running on a computer and the network itself.
- Generally, protocols use headers as a place to put information used by that protocol.
- **Transport Layer**: The transport layers include a smaller number of protocols compared to application layer. The two most commonly used transport layer protocols are **Transmission Control Protocol** (TCP) and **User Datagram Protocol** (UDP). This layer provide services to the application layer that reside one layer higher in TCP/IP model.
- _Adjacent Layer Interaction_: which refers to the concepts of how adjacent layers in a networking model, on the same computer, work together.
- _Same Layer Interaction_: when a particular layer on one computer wants to communicate with the same layer on another computer, the two computers use headers to hold the information that they want to communicate. [Summary](https://postimg.cc/WqRRhLL3)
- **Network Layer**: The TCP/IP network layer includes a small number of protocols, but only one major protocol: the **Internet Protocol** (IP). IP provides several features, most importantly, addressing and routing.
- The TCP/IP application and transport layer act like the person sending letters through the postal service. These upper layers work the same way regardless whether the endpoint host computers are on the same LAN or are separated by the entire Internet. To send a message, these upper layers ask the layers below them, the network layer to deliver the message.
- The lower layers of the TCP/IP model act more like the postal service to deliver those messages to the correct destinations.
- The network layer of the TCP/IP model, primarily defined by the Internet Protocol (IP), works much like the postal service. IP defines that each host computer should have a different IP address, just as postal service defines addressing that uniquely identifies each house
- Similarly IP defines the process of routing so that devices called routers can work like the post office, forwarding packets of data so that they are delivered to the correct destinations.
- Routers are networking devices that connect parts of the TCP/IP network together for the purpose of routing (forwarding) IP packets to the correct destination.
- The term _IP Host_ refers to any device, regardless of size or power that has an IP address and connects to any TCP/IP network.
- **Data Link and Physical Layer**: The data link and physical layer define the protocols and hardware required to deliver data across some physical network. They two work together quite closely. The physical layer defines the cabling and energy that flow over the cables. Some rules and conventions exist when sending data over the cable; however those rules exist in the data link layer of the TCP/IP model.
- The term _encapsulation_ refers to the process of putting headers (and sometimes trailers) around some data.
- Steps in TCP/IP model:
    - Create and encapsulate the application data with any required application layer headers.
    - Encapsulate the data supplied by the application data inside a transport layer header.
    - Encapsulate the data supplied by the transport layer inside a network layer (IP) header.
    - Encapsulate the data supplied by the network layer inside a data-link layer header and trailer.
    - Transmit the bits.
    - [Summary](https://postimg.cc/ygcYKJxZ)
- [Names of TCP/IP Messages](https://postimg.cc/jDHnbdgm)
- [OSI vs TCP/IP](https://postimg.cc/7Jxc9NsX)
- OSI uses a more generic term to refer to messages, rather than frame, segment, packet. OSI uses the term _protocol data unit_ (PDU). A PDU represents the bits that include headers and trailers for that layer, as well as encapsulated data. [Summary](https://postimg.cc/rzKYVK6D)
