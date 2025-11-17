Network Vulnerabilities - 
	Remote access - hosts from potentially anywhere within the network (attack can be organized to pass through many hosts to conceal origin)
	Multiple points of attacks - targets and origins (networked file will pass multiple nodes to storage device, security of file depends on control mechanism of all nodes)
	Unknown perimeter - every network node must be able to react to threats from new hosts that may join the network
	Unknown routing path - no control over routing for users and applications


TCP Session Hijacking 
	hacker takes over TCP session to read what's between the two or manipulate the content
	spoof your IP to match the client

Man-in-the-Middle Hijack
	when attacker is on the same network segment as target machine
	attacker can sniff all back/forth tcp packets and know  the seq/ack numbers
	can inject packet with correct seq/ack with spoofed IP
	![[Pasted image 20251117093055.png]]

SYN Spoofing Denial of Service Attack
	source address in the SYN packet 1 is spoofed
	SYN-ACK packet 2 is sent to random destination
	step 3 never happens
	server is then flooded with SYN requests without getting ACK


Attacks on IP
	Source Spoof - nothing is enforced in IP to show your address is really YOURS
	Payload eavesdrop/tamper - IP provides no protection to the payload or header


DDoS
	attack is from multiple compromised PC's
	capable of impacting the availability
	typically using 'ping' ICMP or SYN flooding

Network Defence
	Firewall - device that filters all traffic between a protected network or "inside" network and less and less trustworthy "outside" network
	keep bad things outside a protected environment 
		Stateless packet filtering - internal network connected to internet via router firewall and router filters packet-by-packet to drop or forward packet based on
			Source and dest IP
			TCP/UDP source and dest port number
			ICCMP message type
			TCP SYN and ACK bits
	Honeypot
		Decoy system filled with fabricated sensitive data
		instrumented with monitors/event loggers
		