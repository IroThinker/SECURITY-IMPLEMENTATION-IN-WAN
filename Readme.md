# SECURITY-IMPLEMENTATION-IN-WAN
**NetworkSecurity Implementation In Wide Area Network**


I created this LAB environment for the assignment which is related to network security. So, in this scenario, I have configured the network using following implementations,  

**-Routing and Switching 
-SSH
-RIP 
-VLANs
-ACL 
-ZPF 
-FTP 
-WEB Servers 
-DNS 
-User control**


I created this scenario for the assignment which is related to network security. so, the scenario was implemented as follows,

Crumlin Computers Limited (CCL) is a Small Business Enterprise providing computing
services to local SMEs. They do not have a proper network infrastructure for the time
being & security is been neglected at all in the existing infrastructure. However, due to
the recent business growth, CCL has decided to revamp its Networking Infrastructure
in a Secure Manner. After several internal discussions, CCL has finalized its
Networking Requirement as follows.

- [ ] CCL has recently purchased a CLASS C subnet from an ISP as below. 210.211.212.0/24. All subnetworks in the new CCL Network Infrastructure shall be devised using the above IP Block
- [ ] In the main branch, there shall be three Networks namely Internal User, Conference Room & Internet
- [ ] Both the Internal User network & Conference Room network shall have two PCs in
- [ ] each.
- [ ] Marketing & Development units shall be separated from the main branch.
- [ ] The main branch shall have an External Firewall placed.
- [ ] The development branch Router shall be directly connected to the Firewall.
- [ ] The development branch shall have three networks comprising a Web Server, Development Unit & Dev_Admin Unit. Both Development & Dev_Admin Units shall have two PCs in each.
- [ ] The marketing Branch shall be connected to the Development branch router
- [ ] The marketing branch shall have three networks comprising an Artwork Server, Creative Teams & NW_Admin
- [ ] Creative Team Network shall have three VLANS (VLAN10, VLAN20 & VLAN30) comprising two PCs in each. VLAN10 & VLAN30 shall be able to communicate with each other but VLAN20 shall not be able to communicate with either VLAN10 or VLAN30
- [ ] Traffic between Development Unit & NW_Admin shall be encrypted via IPSec Tunnel
- [ ] Artwork Server shall be accessed by Dev_Admin Network only using FTP protocol via port 21

**Main Branch External Firewall shall be configured as follows:**

- No traffic initiated from the Internet should be allowed into the internal user or conference room networks.
- Returning Internet traffic (return packets coming from the Internet into the main site, in response to requests originating from any of the main sites networks) should be allowed.
- Computers in the main internal user network are considered trusted and are allowed to initiate any type of traffic (TCP, UDP, or ICMP-based traffic).
- Computers in the main conference room network are considered untrusted and are allowed to initiate only web traffic (HTTP or HTTPS) to the Internet.
- No traffic is allowed between the internal network and the conference room network. There is no guarantee regarding the condition of guest computers in the conference room network. Such machines could be infected with malware and might attempt to send out spam or other malicious traffic.

**All networking devices shall be Configured with Basic Device Settings:**

- Routers names
- IP addresses on routers
- Routing configuration (using RIP)
- Configure PC hosts/Servers' IP settings


**Further, it shall be Configured Secure Router Administrative Access on all routers in Main Branch ONLY as follows:**

- Configure encrypted passwords and login banners
- Configure the EXEC timeout value on console and VTY lines
- Configure a local database, the administrative user
- Configure Secure Shell (SSH) access and disable Telnet

