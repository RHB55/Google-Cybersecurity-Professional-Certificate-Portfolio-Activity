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

## Project Impact
This project highlights the critical role of network Security in ensuring reliable access to web services. The incident demonstrated how a type of DoS attack called a SYN flooding attack can completely prevent users from accessing a website.

From a technical perspective, the project improved the ability to:

* Immediate Mitigation 
* Configure the firewall
* Incident Report
* Suggest potential ways to secure the network so this attack can be prevented in the future.

You will find the **Cybersecurity-incident-report** file in my Cybersecurity Portfolio in the Network Analysis and Security folder, **Analyze network attacks**.




