# Project Description
I work as a security analyst for a travel agency that advertises sales and promotions on the company’s website. The company employees regularly access the company’s sales webpage to search for vacation packages that their customers might like. 
One afternoon, I received an automated alert from the monitoring system indicating a problem with the web server. I suspect the server is under attack by a malicious actor. This event could be a type of DoS attack called SYN flooding.

## Project Scope

**Incident Detection:** One afternoon, an automated alert from the monitoring system indicated a problem with the web server. I attempt to visit the company’s website, but I receive a connection timeout error message in the browser.

**Packet Capturing:** I use a packet sniffer to capture data packets in transit to and from the web server. I notice a large number of TCP SYN requests coming from an unfamiliar IP address. The web server is overwhelmed by the volume of incoming traffic and is losing its ability to respond to the abnormally large number of SYN requests.

**Immediate Mitigation:** I take the server offline temporarily so that the machine can recover and return to a normal operating status. 

**Configure the firewall:** l to block the IP address that was sending an abnormal number of SYN requests. I alerted  my manager about this problem quickly and discussed the next steps to stop this attacker and prevent this problem from happening again.

**Incident Report:** 
Incident Report: I prepared a report about the attack I discovered and how it was  affecting the web server, employees, and the immediate response actions taken.

### **Project Impact**

This project demonstrates the critical importance of network security controls in maintaining the availability and reliability of web services. The incident specifically highlighted how a SYN flooding attack—a type of DoS attack targeting the TCP handshake can overwhelm a server by exhausting its connection resources, ultimately preventing legitimate users from accessing the website.

From a **business perspective**, the attack caused a disruption in service availability, which can negatively impact user experience, customer trust, and overall reputation. Even short periods of downtime can result in lost engagement and potential revenue, especially for client-facing services.

From a **technical perspective**, this project significantly strengthened practical cybersecurity skills in several key areas:

* **Immediate Mitigation:**
  Identifying the attack pattern and taking rapid action to reduce its impact, such as limiting incoming traffic and stabilizing network performance.

* **Firewall Configuration:**
  Implementing and refining firewall rules to filter malicious traffic, including protections against SYN flood attacks.

* **Incident Analysis & Reporting:**
  Documenting the attack, analyzing packet behavior, and clearly communicating findings through a structured incident report.

* **Future Risk Reduction:**
  Proposing security improvements such as intrusion detection/prevention systems (IDS/IPS), traffic monitoring, and stronger network configurations to prevent similar attacks.

This work is documented in the **Cybersecurity Incident Report**, which is included in my portfolio under the **Network Analysis and Security** section. The project reflects hands-on experience in analyzing real-world network attacks and applying practical solutions to enhance overall security posture.




