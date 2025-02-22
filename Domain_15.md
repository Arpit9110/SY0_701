# Security Infrastructure

### Ports and Protocols

Ports

 These are the logical communication endpoints on a computer or server. It is classified as either Inbound (Listening for connections) or Outbound (Used to connect to a server). Example SSH connection with an inbound port 22 and an outbound port on the client.

Port Classification

 - Well-Known Ports (0-1023): Assigned by IANA, commonly-used protocols.

 - Registered Ports (1024-49151): Vendor-specific, registered with IANA.

 - Dynamic and private Ports (49152-65535): Temporary outbound connections.

Protocols

 These are the rules that governing device communication and data exchange.

 For Example: HTTPS (port 443) uses the HTTPS protocol for secure web communication.

List Of Ports and Protocols

  - Port 21: FTP (File Transfer Protocol) - TCP

  - Port 22: SSH, SCP, SFTP - TCP

  - Port 23: Telnet - TCP

  - Port 25: SMTP (Simple Mail Transfer Protocol) - TCP

  - Port 53: DNS (Domain Name System) - TCP/UDP

  - Port 69: TFTP (Trivial File Transfer Protocol) - UDP

  - Port 80: HTTP (Hypertext Transfer Protocol) - TCP

  - Port 88: Kerberos - UDP

  - Port 110: POP3 (Post Office Protocol) - TCP

  - Port 119: NNTP (Network News Transfer Protocol) - TCP

  - Port 135: RPC (Remote Procedure Call) - TCP/UDP

  - Ports 137, 138, 139: NetBIOS - TCP/UDP

  - Port 143: IMAP (Internet Message Access Protocol) - TCP

  - Port 161: SNMP (Simple Network Management Protocol) - UDP

  - Port 162: SNMP Trap - UDP

  - Port 389: LDAP (Lightweight Directory Access Protocol) - TCP

  - Port 443: HTTPS (HTTP Secure) - TCP

  - Port 445: SMB (Server Message Block) - TCP

  - Ports 465, 587: SMTPS (SMTP Secure) - TCP

  - Port 514: Syslog - UDP

  - Port 636: LDAPS (LDAP Secure) - TCP

  - Port 993: IMAPS (IMAP over SSL/TLS) - TCP

  - Port 995: POP3S (POP3 over SSL/TLS) - TCP

  - Port 1433: Microsoft SQL - TCP

  - Ports 1645, 1646: RADIUS (Remote Authentication) - TCP

  - Ports 1812, 1813: RADIUS UDP - UDP

  - Port 3389: RDP (Remote Desktop Protocol) - TCP

  - Port 6514: Syslog TLS - TCP

### Firewalls

Firewall

  A network security device or software that monitors and controls network traffic

based on security rules. Protects networks from unauthorized access and potential threats.

Screened Subnet (Dual-homed Host)

  Acts as a security barrier between external untrusted networks and internal trusted networks using a protected host with security measures like a packet-filtering firewall

Types of Firewalls

 - Packet Filtering Firewalls: This firewall inspects packet headers for IP addresses and port numbers. This is limited in inspection, and it operates at Layer 4 (Transport Layer).

 - Stateful Firewalls: This firewall track connections and requests, allowing return traffic for outbound requests. This operates at Layer 4, with improved awareness of connection state

 - Proxy Firewalls: This firewall makes connections on behalf of endpoints, enhancing security

    These are of two Types of Proxy Firewalls:

       - Circuit level (Layer 5)

       - Application level (Layer 7)

 - Kernel Proxy Firewalls: This firewall has a minimal impact on network performance, full inspection of packets at every layer. They are placed close to the system they protect.

Firewall Evolutions

 Next Generation Firewall (NGFW)

 This type of firewall is Applucation aware which means it can distinguish between different types of traffic. It can conduct deep packet inspection and use signature-based intrusion protection. It operates fast with minimal network performance impact. It offers full-stack traffic visibility. It Can be a problem if organizations become reliant on a single vendor due to firewall configurations tailored to one product line.

 Unified Threat Management (UTM) firewall

  It combines multiple security functions in a single device. Its functions include firewall, intrusion prevention, antivirus, and more. It has a single point of failure but it uses separate and individual engines.

 Web Application Firewall (WAF)

  It focuses on inspecting HTTP traffic. It helps in preventing common web application attacks like cross-site scripting and SQL injections.

  It can be deployed in different ways:

    In-line (live attack prevention): These devices sit between the network firewall and the web servers.

    Out of band (detection): These devices received a mirrored copy of a web server traffic.

 Layer based Firewalls

  Layer 4 Firewall: These operates at the application layer. It filters the traffic based on port number and protocol data.

  Layer 7 Firewall: It operates at the application layer. It inspects, filter and controls traffic based on content and data characteristics.

### Configuring Firewalls

Firewalls and Access Control Lists (ACLs)

  Firewalls: These are dedicated devices for using Access Control Lists (ACLs) to protect networks.

  Access controls Lists (ACLs): This very Essential list for securing networks from unwanted traffic. It Consist of permit and deny statements, often based on port numbers, it rules sets placed on firewalls, routers, and network infrastructure devices. It Control the flow of traffic into and out of networks. It may define quality of service levels inside networks but are primarily used for network security in firewalls.

Configuring ACLs

 A web-based interface or a text-based command line interface can be used. The order of ACL rules specifies the order of actions taken on traffic (top-down). The first matching rule is executed, and then no other ACLs are checked. Always place the most specific rules at the top and generic rules at the bottom. Some devices support implied deny functions, while others require a "deny all" rule at the end. Actions taken by network devices should be logged, including deny actions.