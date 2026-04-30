# Project Description 
As a cybersecurity analyst working at a company that specializes in providing IT services for clients. Several customers of clients reported that they were not able to access the client company website www.yummyrecipesforme.com, and saw the error “destination port unreachable” after waiting for the page to load. I was tasked with analyzing the situation and determining which network protocol was affected during this incident.

### Solution Strategy Followed  :
**Step 1: Identify the Issue**

I received reports that users could not access the website and were seeing the error **“destination port unreachable.”** I reproduced the issue by attempting to visit the website myself and observed the same error.

**Step 2: Begin Troubleshooting**

To investigate further, I used a network analysis tool (`tcpdump`) to capture and analyze network traffic while trying to load the website.

**Step 3: Observe Network Behavior**

I observed that:
* The browser sends a DNS query using UDP to resolve the domain name into an IP address
* This query is sent to port 53, which is used by DNS services
  
**Step 4: Analyze the Error Response**

The network analyzer showed that instead of receiving a valid DNS response, the system received an ICMP error message stating: “UDP port 53 unreachable.”
  
**Step 5: Determine the Root Cause**

This indicates that:
* The DNS service (UDP port 53) is not reachable
* The issue is likely caused by a blocked or misconfigured DNS service, firewall rule, or DNS server being down

**Step 6: Identify the Affected Protocol**

Based on the analysis, the affected protocol is:
UDP (User Datagram Protocol), specifically used by the DNS protocol

**Step 7: Conclusion**

The website is inaccessible because the system cannot resolve the domain name due to a failure in DNS communication over UDP (port 53). Without DNS resolution, the browser cannot proceed with the HTTPS request to load the website.

### **Project Impact**

This project highlights the critical role of network protocols in ensuring reliable access to web services. The incident demonstrated how a failure in the DNS resolution process over UDP (port 53) can completely prevent users from accessing a website, even when the web server itself is operational.

From a technical perspective, the project improved the team’s ability to:
* Diagnose network issues using tools like packet analyzers
* Identify protocol-level failures (UDP, DNS, ICMP)
* Understand how different network protocols interact in real-world scenarios

Overall, this project strengthened incident analysis skills, reinforced the importance of proactive monitoring and configuration management, and contributed to improving the organization’s network reliability and resilience.


