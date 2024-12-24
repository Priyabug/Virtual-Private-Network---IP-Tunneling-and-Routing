<h1>Implementation of VPN Tunnel</h1>



<h2>Description</h2>
A private network constructed on top of a public network, typically the Internet, is called a virtual private network, or VPN. Even though their communication may pass through a public network, computers inside a VPN can connect securely, exactly like if they were on a true private network that is physically isolated from the outside world. With the use of a VPN, staff members may safely access their company's intranet while on the go. Businesses can also use VPNs to extend their private networks domestically and internationally.


This lab's goal is to assist students in comprehending how a VPN operates. We concentrate on a particular kind of VPN (the most popular one), which is constructed on top of the transport layer. We are going to construct a basic VPN from the ground up.
<br />


<h2> Lab topics covered</h2>

- <b>Network Setup.</b>
- <b>Create and Configure TUN Interface</b><br>
          2.a: Name of the Interface<br>
          2.b: Set up the TUN Interface<br>
          2.c: Read from the TUN Interface<br>
          2.d: Write to the TUN Interface<br>
- <b>Send the IP Packet to VPN Server Through a Tunnel</b>

<h2>Shell scripts commands</h2>

- `./dc-build.sh` - Build the docker images, it can take one additional parameter to be used in the build process, e.g. `./dc-build.sh --no-cache`.
- `./dc-up.sh` - Start the docker containers in the foreground.
- `./dc-up-d.sh` - Start the docker containers in the background.
- `./dc-stop.sh` - Stop the docker containers, it can take one additional parameter to be used in the stop process.
- `./dc-down.sh` - Stop and remove the docker containers, it can take one additional parameter to be used in the stop and remove process.
- `./dc-unittest.sh` - Utility script to aid in running a specific unit test class.

<h2>Program walk-through:</h2>

- <b> Using Scapy for Sniffing and Spoofing:</b>

     1. Sniffing packets with Scapy, including setting filters to capture specific types of packets (like ICMP or TCP).<br>
     2. Spoofing ICMP packets with arbitrary source IP addresses using Scapy.<br>
     3. Implementing a traceroute-like tool using Scapy by manipulating the TTL (Time-To-Live) field in IP packets.<br>
     4. Combining sniffing and spoofing techniques to create a program that automatically sends spoofed ICMP replies.<br>

- <b> Writing C Programs for Sniffing and Spoofing:</b>
 
     1. Tasks in this set involve writing programs in C to manually implement packet sniffing and spoofing, allowing students to understand the
          low-level implementation details of these techniques.<br>
