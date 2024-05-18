# Network-Security - Labs & Projects

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

<html>
	<body>
		<h1>Configuring a VPN Server with pfSense</h1>
			<h2>Overview</h2>
				<p>
				This lab was a practical demonstration of how theoretical knowledge can be applied to deploy and configure security measures for a networked environment.
				By using a combination of theoretical concepts and practical tools, we were able to establish a robust defense system. The lab involved setting up virtual machines with various operating systems and implementing firewall rules, 
				intrusion detection systems, and VPN configurations. These tasks were not just theoretical exercises but real-world scenarios aimed at enhancing the network's security posture and ensuring the integrity, confidentiality, and availability of the data transmitted across it.
				</p>
				<p>
				The initial phase involved configuring the firewall using pfSense, an open-source firewall solution based on FreeBSD. I could control inbound and outbound traffic by creating specific firewall rules,
				thereby restricting unauthorized access and mitigating potential threats. This involved setting up NAT (Network Address Translation) rules to map private IP addresses to public ones, essential for securing internal network traffic from external threats. 
				Additionally, I configured port forwarding to allow specific services to be accessible from outside the network, ensuring that only necessary services were exposed while minimizing the attack surface.
				</p>
				<p>
				Following the firewall configuration, the next step was to deploy an Intrusion Detection System (IDS) using Snort, a widely used open-source IDS tool. Installing Snort on a designated network segment allowed me to monitor and analyze network traffic for suspicious activities and potential intrusions. 
				The IDS was configured with a set of predefined rules to detect common attack patterns, such as port scans, malware traffic, and exploitation attempts. This real-time monitoring and alerting mechanism enabled the early detection and response to potential security incidents, enhancing the overall network security.
				</p>
				<p>
				The final aspect of the lab involved setting up a Virtual Private Network (VPN) to ensure secure remote access to the network. By configuring OpenVPN on pfSense, I established a secure encrypted tunnel between the remote user and the internal network.
				This VPN setup allowed secure communication over untrusted networks, protecting sensitive data from eavesdropping and man-in-the-middle attacks. The configuration included generating cryptographic keys, setting up user authentication, and defining secure encryption protocols,
				ensuring that only authorized users could access the network resources securely.
				</p>
				<p>
				The lab provided hands-on experience with critical network security tools and techniques, reinforcing the theoretical concepts learned. By configuring firewalls, deploying intrusion detection systems, and setting up VPNs, I gained a comprehensive understanding of protecting and managing a secure network infrastructure.
				This practical application of security measures demonstrated the importance of a multi-layered defense strategy in safeguarding network environments from a wide range of cyber threats.
				</p>
			<h2> Tools & Technologies Used</h2>
				<p>
				In Configuring a VPN Server with pfSense, a range of advanced tools and technologies were utilized to enhance the security of a networked environment. The focus was configuring firewalls, 
				deploying intrusion detection systems, and setting up virtual private networks. These activities provided practical insights into securing network infrastructure against various cyber threats. Below is a detailed list of the tools and technologies and their technical summaries.
				</p>
				<ul>
				<li><strong>pfSense:</strong>An open-source firewall and router software distribution based on FreeBSD. It includes many features, such as stateful packet filtering, VPN support, and traffic shaping. pfSense allows for granular control over network traffic by creating custom firewall rules and network address translation (NAT) settings. 
				It is highly extensible with packages that can add additional security and networking capabilities.</li>
				<li><strong>Snort:</strong>An open-source network intrusion detection system (IDS) is capable of real-time traffic analysis and packet logging. It uses a rule-driven language to perform protocol analysis, content searching, and various forms of attack detection. 
				Snort can be configured to operate in multiple modes, such as sniffer, packet logger, and network intrusion detection, providing flexibility in managing and monitoring network security.</li>
				<li><strong>OpenVPN:</strong>An open-source software application that implements virtual private network (VPN) techniques to create secure point-to-point or site-to-site connections. It uses custom security protocols to establish encrypted tunnels, ensuring secure data transmission over untrusted networks. OpenVPN supports various authentication methods,
				including pre-shared keys, certificates, and username/password combinations, making it versatile for different security requirements.</li>
				<li><strong>Virtual Machines (VMs):</strong>Software-based emulations of physical computers. They allow for the creation of isolated environments on a single physical host, enabling the deployment of multiple operating systems and applications for testing and development. In this lab, VMs were used to simulate different network nodes and services,
				providing a controlled environment for implementing and testing security configurations.</li>
				<li><strong>Windows Server 2019:</strong>A robust server operating system developed by Microsoft. It provides a comprehensive platform for network management, data storage, application hosting, and enterprise-level security. Features include advanced threat protection, hybrid cloud support, and extensive management tools for both on-premises and cloud-based environments.</li>
				<li><strong>Ubuntu Linux:</strong>A popular open-source operating system based on Debian. It is known for its ease of use, stability, and security. Ubuntu provides a flexible platform for deploying various network services and security tools, making it suitable for server and desktop environments. It supports extensive networking capabilities and a wide range of security tools.</li>
				</ul>
				<p>
				By leveraging these tools and technologies, the lab provided a practical and comprehensive approach to network security. Configuring firewalls, deploying intrusion detection systems, and setting up secure VPN connections were key activities that enhanced my understanding of protecting and managing secure network infrastructures.
				</p>
	</body>
</html>

<html>
	<body>
	<h1>Developing A Zero-Trust Network Architecture</h1>
		<h2>Overview</h2>
			<p>
			In the lab focused on developing a Zero-Trust Network Architecture (ZTNA) proposal, I created a comprehensive security strategy for Genco, an international olive oil company. 
			This involved a detailed review and application of several security frameworks, including the EU Cybersecurity Act, ISO 27001 standards, and the NIST Zero-Trust Architecture. 
			The proposal aimed to align Genco’s security posture with these frameworks to protect against sophisticated cyber threats and ensure compliance with relevant regulations.
			</p>
			<p>
			The proposal's cornerstone was the integration of Zero-Trust principles into Genco’s current network infrastructure. Zero-Trust architecture, a key proposal component,
			mandates that all internal and external network traffic be authenticated and authorized. This necessitated the implementation of strict identity and access management (IAM) protocols,
			ensuring that only verified users and devices could access network resources. I recommended the deployment of multi-factor authentication (MFA) and robust identity governance to manage access rights dynamically based on user roles and behavior.
			</p>
			<p>
			Another crucial aspect of the proposal was network segmentation. This process involved dividing the network into isolated segments, a measure aimed at limiting lateral movement within the network. Doing so contained potential breaches and minimized the impact of any security incidents. 
			To support this, I recommended updating network devices such as routers and servers to enable segmentation and Zero-Trust capabilities. Additionally, I suggested continuous monitoring and analytics to maintain visibility over network traffic, enabling the detection of anomalies and potential threats in real-time.
			</p>
			<p>
			Finally, I emphasized the importance of securing data-in-transit and data-at-rest through encryption and advanced data protection mechanisms. This included recommending secure communication protocols and updating software to ensure compliance with Zero-Trust standards. 
			The proposal underscored the need for an ongoing commitment to cybersecurity through regular updates, employee training on security best practices, and adherence to the Zero-Trust Maturity Model to achieve optimal security across all network dimensions. By adopting these measures,
			Genco could significantly enhance its defense against cyber threats and ensure robust protection for its digital assets.
			</p>
		<h2> Tools & Technologies Used</h2>
			<p>
			In the lab focused on developing a Zero-Trust Network Architecture (ZTNA) proposal, a range of advanced tools and technologies were utilized to enhance Genco’s network security in accordance with the Zero-Trust principles outlined by frameworks such as the EU Cybersecurity Act, ISO 27001, and NIST Zero-Trust Architecture. 
			Implementing these tools was crucial for ensuring comprehensive protection against cyber threats and compliance with industry standards. Below is a detailed list of the tools and technologies employed in the lab, directly linking their use to the lab’s objectives and frameworks.
			</p>
			<ul>
			<li><strong>pfSense:</strong>The lab used pfSense as a core component for implementing network segmentation and firewall configurations in line with Zero-Trust principles. Based on FreeBSD, this open-source firewall and router software distribution provided the necessary stateful packet filtering and network address translation (NAT) capabilities. 
			By setting up custom firewall rules and secure VPNs, pfSense enabled granular control over network traffic and protected sensitive data in transit, aligning with ISO 27001 standards for network security.</li>
			<li><strong>Snort:</strong>It was deployed to enhance Genco's network intrusion detection capabilities, directly supporting the NIST Zero Trust Architecture framework's emphasis on continuous monitoring and analysis. This open-source network intrusion detection system (IDS) provided real-time traffic analysis and packet logging.
			By employing a rule-based language to identify and alert suspicious activities such as port scans and malware traffic, Snort ensured the network was monitored for potential threats, adhering to the EU Cybersecurity Act’s requirements for proactive threat detection.</li>
			<li><strong>OpenVPN:</strong>It was Utilized in the lab to establish secure remote access to Genco’s network, ensuring encrypted communication channels in accordance with Zero Trust principles. This open-source VPN software created secure point-to-point or site-to-site connections through encrypted tunnels.
			By supporting various authentication methods and robust encryption protocols, OpenVPN facilitated secure and authenticated remote access, protecting data-in-transit and meeting the stringent requirements of ISO 27001 for secure communication.</li>
			<li><strong>Virtual Machines (VMs):</strong>They were integral to the lab, providing isolated environments for testing and implementing the Zero Trust Network Access configurations. These VMs simulated different network nodes and services, enabling a controlled setup to deploy and verify security measures.
			The use of VMs ensured a flexible and scalable testing environment, essential for adhering to the NIST Zero-Trust Architecture’s guidelines on network security testing and validation.</li>
			<li><strong>Windows Server 2019:</strong>It was employed in the lab to manage and secure Genco’s network infrastructure. This server operating system from Microsoft provided advanced features for network management, data storage, and application hosting. By leveraging its comprehensive administrative tools and advanced threat protection capabilities, 
			the lab ensured the network configurations met the ISO 27001 standards for enterprise-level security and management.</li>
			<li><strong>Ubuntu Linux:</strong>It was used in the lab to deploy various network services and security tools, supporting the Zero-Trust Architecture framework’s focus on robust and secure network setups. Known for its stability and security, Ubuntu provided a reliable platform for implementing network security measures. 
			The lab utilized Ubuntu’s extensive package repository and strong community support to ensure continuous updates and maintain a secure environment, in line with the EU Cybersecurity Act’s requirements for ongoing security management.</li>			
			</ul>
	<body>
</html>
