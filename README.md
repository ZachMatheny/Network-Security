# Network-Security

<html>
	<body>
		<h1>Assessing the Network with Common Security Tools</h1>
			<h2>Overview</h2>
				<p>
				In the "Assessing the Network with Common Security Tools" lab, I comprehensively analyzed network traffic and configurations using an 					array of advanced tools within a virtualized environment. Utilizing Kali Linux, Windows Server 2019, and Ubuntu Linux as operating 					systems, I applied tools such as 
				ARP, ipconfig, ifconfig, hping3, ping, tcpdump, Nmap, and Wireshark to examine both local and wide area networks. The primary focus was 				gathering and interpreting network configuration details, capturing network traffic, and identifying potential security vulnerabilities.
				</p>
				<p>
				My analysis began with using ipconfig on Windows and ifconfig on Linux to obtain essential network parameters such as IP addresses, 					subnet masks, and default gateways. This was followed by the use of ARP to inspect the ARP cache, providing insights into the IP-to-MAC 				address mappings within the local network.
				This step is crucial for diagnosing connectivity issues and detecting possible ARP spoofing attacks. Next, I employed ping and hping3 					to test network reachability and latency, and tcpdump to capture and analyze raw packet data. This step facilitated the identification 					of network anomalies and performance bottlenecks, 
				providing a comprehensive view of the network's health.
				</p>
				<p>
				The lab also involved running comprehensive Nmap scans to discover live hosts, open ports, and services, which helped map the network 					topology and identify potential attack entry points. Using Wireshark, I performed deep packet inspection, filtering ICMP, ARP, and 					other protocol-specific traffic to uncover detailed information about network communications and detect suspicious activities. 
				This hands-on approach enabled a thorough understanding of network diagnostics, configuration troubleshooting, and security 						assessments, ultimately enhancing my capability to secure and manage complex network environments.
				</p>
			<h2>Tools & Technologies Used</h2>
				<p>
				During this lab, various tools and technologies were utilized to thoroughly analyze network traffic, configurations, and security 					postures. These tools enabled the identification of network anomalies, vulnerabilities, 
				and overall performance issues, enhancing my practical understanding of network diagnostics and security assessments. Below is a 					detailed list of the tools and technologies used and their technical descriptions.
				</P>
				<ol>
					<li><strong>ipconfig/ifconfig:</strong>ipconfig (on Windows) and ifconfig (on Unix-like systems) are command-line utilities 						that display and configure network interface parameters. They provide essential information such as IP addresses,
					subnet masks, default gateways, and MAC addresses, which are crucial for network troubleshooting and configuration.</li>
					<li><strong>ARP (Address Resolution Protocol):</strong>ARP is a protocol used for mapping IP network addresses to the hardware 						(MAC) addresses used by data link protocol. Commands like arp -a allow users to view and manage the ARP cache,
					which is instrumental in diagnosing network communication issues and detecting ARP spoofing attacks.</li>
					<li><strong>ping:</strong>The ICMP Echo Request command is used to test a host's reachability on an IP network. It sends ICMP 						Echo Request messages to the target host and listens for ICMP Echo Reply messages. This tool helps measure round-trip time and 						packet loss, thereby assessing network connectivity and performance.</li>
					<li><strong>hping3:</strong>A packet generator and analyzer for the TCP/IP protocol. It allows for custom TCP/IP packets and 						supports protocols like TCP, UDP, ICMP, and RAW-IP. It is often used for firewall testing, network auditing, scanning, and 						advanced traceroute operations.</li>
					<li><strong>tcpdump:</strong>A powerful command-line packet analyzer. It allows users to capture and display the contents of 						network packets transmitted or received over a network to which the computer is attached. Tcpdump is used for network 							troubleshooting and analysis.</li>
					<li><strong>Nmap/Zenmap:</strong>Nmap (Network Mapper) is a versatile open-source network discovery and security auditing tool. 					Zenmap is its graphical user interface (GUI) version. Nmap can scan for live hosts, open ports, and services and detect the 						operating system and version running on remote machines. 
					It's widely used for network inventory, managing service upgrade schedules, and monitoring host or service uptime.</li>
					<li><strong>Wireshark:</strong>A widely used network protocol analyzer enables users to capture and interactively browse the 						traffic running on a computer network. It provides deep inspection of hundreds of protocols, live capture, and offline 							analysis, making it indispensable for network troubleshooting, analysis,
					software and protocol development, and education.</li>
					<li><strong>pfSense:</strong>An open-source firewall and router software distribution based on FreeBSD. With its robust 						features, including stateful packet filtering, VPN support, and traffic shaping, pfSense is used for network security and 						management in enterprise and home networks.</li>	
					<li><strong>Kali Linux:</strong>a Debian-based Linux distribution aimed at advanced penetration testing and security auditing. 						It has numerous pre-installed tools for various information security tasks, including penetration testing, security research, 						computer forensics, and reverse engineering.</li>										
				</ol>
				<p>
				The lab exercises leveraged these tools and provided hands-on experience in network traffic analysis, configuration troubleshooting, 					and security vulnerability identification, reinforcing theoretical knowledge with practical application.
				</p>
	</body>
</html>



