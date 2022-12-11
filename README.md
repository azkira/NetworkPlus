# NetworkPlus 

## OSI Layer (Open Systems Interconnection Reference Model)

All People Seem To Need Data Processing

7 Layer => (7 to 1) Application, Presentation, Session, Transport, Network, Data Link, Physical

Physical Layer (Layer 1)

is about the signaling, talking about the cables that you're using, the fiber runs, or the ability to get signals.

Real-world to OSI model
Cables, fiber, and the signal itself

Physical: Electric signals

Data Link Layer (Layer 2)

the basic network "language". the foundation of communication at the data link layer. Also refer to Data Link Control (DLC) protocols. Also called the "switching" layer.

Real-world to OSI model
Frame, MAC address, Extended Unique Identifier (EUI-48, EUI-64), Switch

Data Link: Ethernet

Network Layer (Layer 3)

The "routing" layer, associated with IP address.

Real-world to OSI model
IP address, Router, Packet

Network: IP encapsulation

Transport Layer (Layer 4)

The "post office" layer. This layer describes how data is being delivered and where it is being delivered into the system. TCP and UDP is in this layer.

Real-world to OSI model
TCP segment, UDP datagram

Transport: TCP encapsulation

Session Layer (Layer 5)

Communication management between devices. Control protocols, tunneling protocols.

Real-world to OSI model
Control Protocols, tunneling protocols

Session: Link the presentation to the transport

Presentation Layer (Layer 6)

Anything dealing with encoding or encryption. Often combined with layer 7

Real-world to OSI model
Application encryption (SSL,TLS)

Presentation: SSL encryption

Application Layer (Layer 7)

The layer we're seeing on screen. HTTP, FTP, DNS, POP3

Real-world to OSI model
Your eyes

Application: https://mail.google.com

## PDU (Protocol Data Unit)

Transmission Units
a different group of data at different OSI layers

Ethernet operates on a frame of data
it doesn't care what's inside

IP operates on a packet of data
inside is TCP or UDP, but IP doens't really care

TCP ord UDP
TCP segment
UDP datagram

Encapsulation and Decapsulation
When a data is being transmitted. Encapsulation and Decapsulation process is happening

TCP flags
the header describes or identifies the payload

The TCP header contains important control information
includes a set of bits called TCP flags

The flags control the payload
SYN-synchronize sequence numbers
PHH-push the data to the application without buffering
RST-reset the connection
FIN-last packet from the sender

Maximun IP packet to transmit
but not fragment

fragmentation slows things down
losing a fragment loses an entire packet
requires overhead along the path

Difficult to know the MTU all the way through the path
Automated methods are often innacurate
Especially when ICMP is filtered
