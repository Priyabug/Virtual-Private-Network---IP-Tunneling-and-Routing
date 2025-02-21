<h1>Virtual Private Network - IP Tunneling and Routing</h1>

<h2>Description</h2>

• <b> A private network constructed on top of a public network, typically the Internet, is called a virtual private network, or VPN. Even though their communication may pass through a public network, computers inside a VPN can connect securely, exactly like if they were on a true private network that is physically isolated from the outside world. With the use of a VPN, staff members may safely access their company's intranet while on the go. Businesses can also use VPNs to extend their private networks domestically and internationally.</b>


• <b> The goal of this lab implementation is to understand how a VPN operates. We concentrate on a particular kind of VPN (the most popular one), which is constructed on top of the transport layer. We are going to construct a basic VPN from the ground up.</b>
<br />

![image](https://github.com/user-attachments/assets/6e2f1fb3-cbd2-46da-ac63-ee55d799403b)


<h2> Lab topics covered</h2>

- <b>Network Setup.</b>
- <b>Create and Configure TUN Interface</b><br>
          2.a: Name of the Interface<br>
          2.b: Set up the TUN Interface<br>
          2.c: Read from the TUN Interface<br>
          2.d: Write to the TUN Interface<br>
- <b>Send the IP Packet to VPN Server Through a Tunnel</b>

<h2>Shell scripts commands</h2>

- `./dc-build.sh` - Build the docker images, it can take one additional parameter to be used in the build process.
- `./dc-up.sh` - Start the docker containers in the foreground.
- `./dc-up-d.sh` - Start the docker containers in the background.
- `./dc-stop.sh` - Stop the docker containers, it can take one additional parameter to be used in the stop process.
- `./dc-down.sh` - Stop and remove the docker containers, it can take one additional parameter to be used in the stop and remove process.
- `./dc-unittest.sh` - Utility script to aid in running a specific unit test class.

<h2>Program walk-through:</h2>
This lab provides hands-on experience with the foundational concepts of VPNs, including TUN/TAP interfaces, tunneling, and routing. By implementing both unidirectional and bidirectional tunnels,

- <b>Virtual Private Network:</b><br>

   • The TUN/TAP virtual interface<br>
   • IP tunneling<br>
   • Routing<br>

