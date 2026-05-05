# Project overview
As a cybersecurity analyst, my organization experienced a DoS attack. My task is to create an incident report of this security event and create a plan to improve my company’s network security, following the National Institute of Standards and Technology (NIST) Cybersecurity Framework (CSF)
NIST cybersecurity framework responds to a security incident.

## Security Event Investigation:
The security team  investigated the security event. They found that a malicious actor had sent a flood of ICMP pings into the company’s network through an unconfigured firewall. This vulnerability allowed the malicious attacker to overwhelm the company’s network through a denial of service(DoS)attack.

## Security event Response: 
To address this security event, the network security team implemented: 
* A new firewall rule to limit the rate of incoming ICMP packets
* Source IP address verification on the firewall to check for spoofed IP addresses on incoming ICMP packets
* Network monitoring software to detect abnormal traffic patterns
* An IDS/IPS system to filter out some ICMP traffic based on suspicious characteristics
  
##  National Institute of Standards and Technology (NIST) Cybersecurity Framework (CSF)
* Identify security risks through regular audits of internal networks, systems, devices, and access privileges to identify potential security gaps. 
* Protect internal assets through the implementation of policies, procedures, training, and tools that help mitigate cybersecurity threats. 
* Detect potential security incidents and improve monitoring capabilities to increase the speed and efficiency of detections. 
* Respond to contain, neutralize, and analyze security incidents; implement improvements to the security process. 

## Incident report analysis using Cybersecurity Framework (CSF)
1. **Identify:** The cybersecurity team investigated the security event. They found that a malicious actor had sent a flood of ICMP pings into the company’s network through an unconfigured firewall
2.  **Protect:**	The network security team implemented a new firewall rule to limit the rate of incoming ICMP packets, and an IDS/IPS system to filter out some ICMP traffic based on suspicious characteristics.
3.  **Detect:**	To detect unauthorized access, the security team configured source IP address verification on the firewall to check for spoofed IP addresses on incoming ICMP packets and implemented network monitoring software to detect abnormal traffic patterns.
4.  **Respond:**	For future incidents, the cybersecurity team will contain threats by isolating affected systems, restoring critical services, and analyzing network logs to identify suspicious activity.
5.  **Recover:**	Recovery from an ICMP flood (DDoS) attack focuses on restoring normal network operations in a controlled and prioritized manner. First, block malicious ICMP traffic at the firewall to stop the attack. Then, reduce strain on the network by shutting down non-critical services. Critical services should be restored first to resume essential operations. Once the attack traffic subsides, all remaining non-critical systems can be safely brought back online.




