Application Requirements from Transport
	Data Integrity 
		- some files (e.g. web transactions) require 100% reliable data transfer 
		- audio for example can make do with some loss
	Timing 
		- some apps (e.g. interactive games) require low delay
	Security 
		- encryption
	Throughput 
		- some apps (e.g. multimedia) require a minimum throughput to be effective 
		- elastic apps on the other hand just use whatever they can 
![[Pasted image 20251110091834.png]]



| TCP                                                           | UDP                                                                                                                         |
| ------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
| Reliable                                                      | unreliable data transfer                                                                                                    |
| Flow Control: sender doesnt overwhelm the network             | doesnt provide: reliability, flow control, congestion control, timing, throughput, guarantee, security, or connection setup |
| Throttle sender when network overloaded                       |                                                                                                                             |
| Doesn't provide: timing, min throughput guarantee, sec        |                                                                                                                             |
| Connection-oriented: setup required between client and server |                                                                                                                             |

network layer: 
	logical communication between hosts
transport layer:
	logical between processes 
		relies on: enhances, network layer services
		this is primary purpose of the transport layer provided by all implementations of transport protocol


Sender:
	is passed an application layer msg
	determines segment header field values
	creates segments
	passes them through IP

Receiver:
	receives segment from IP
	checks header values
	extracts application-layer
	demultiplexes message up to application via socket

![[Pasted image 20251110093458.png]]
how demultiplexing works :
- host receives IP datagrams:
	- each datagram has source IP and destination IP
	- each datagram is carrying one transport-layer segment
	- each segment has source destination port number
- host uses IP addresses & port to direct segments 

connectionless demultiplexing:
sockets - when creating socket u must specify host port #
when creating datagram to send into UDP socket, must specify - destination IP and port #
	when receiving UDP segment - check destination port # in seg, direct UDP to seg with that port #

connection oriented 


UDP
connectionless:
	no handshake between sender and receiver 
	each segment is handled individually 
		WHY?
		no need connection establishment (which otherwise can add RTT delay)
		simple as no connection states
		small header size
		no congestion control (can blast quickly, and function in the face of congestion)

TCP
	point-to-point - one sender one receiver
	reliable, in order stream 
	cumulative ACKs
	full duplex data
		bi-directional data flow in same connection
		MSS: Maximum Segment Size
	Connection-oriented - handshaking (exchange of control messages) initializing sender, receiver state before data exchange
	![[Pasted image 20251110100825.png]]


network layer 
transport segment from sending to receiving
sender: encapsulates segments into datagram, passes to link layer
receiver: delivers segments to transport layer protocol
network layer protocols in evert internet device : hosts, routers

Data plane:
	local: per-router function 
	determines how datagram arriving on router input port is forwarded to router output port

Control plane:
	network-wide logic
	determines how datagram is routed among routers 
	two-control plane approaches:
		traditional routing algos: implemented in routers
		software defined networking: implemented in (remote) servers
		![[Pasted image 20251110104516.png]]

internet provides no guarantee delivery of message from A to which is why we dont just use IP without TCP

![[Pasted image 20251110105250.png]]
matches with 1 as its longer than 2 

