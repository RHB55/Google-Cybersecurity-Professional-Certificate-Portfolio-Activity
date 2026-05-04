# Project Overview
In this activity, I will take on the role of a cybersecurity analyst working for a company that hosts the cooking website, yummyrecipesforme.com. Visitors to the website experience a security issue when loading the main webpage. My job is to investigate, identify, document, and recommend a solution to the security problem. 

### Project Scope: 
**Incident Analysis and Remediation**

### Incident Summary
A former employee gained unauthorized access to the administrative panel of `yummyrecipesforme.com` by executing a brute force attack against an account still using default credentials. 

### Technical Investigation
I conducted the test in a controlled sandbox environment using `tcpdump` to capture network traffic.

### Packet Analysis Workflow
1.  **DNS Query:** Browser requests IP for `yummyrecipesforme.com`.
2.  **HTTP Request:** Browser fetches the compromised index page.
3.  **Payload Delivery:** The JavaScript function triggers the download of the executable.
4.  **Malicious Redirection:** The script initiates a second DNS/HTTP request to `greatrecipesforme.com`.

### Discovery & Impact
*   **Discovery:** The incident was identified after multiple customer reports to the helpdesk regarding slow computer performance and suspicious download prompts.
*   **Impact:** The legitimate business website was rendered unsafe, customer machines were potentially infected with malware, and administrative access was lost.
*   **Root Cause:** Failure to change default administrative credentials and a lack of account lockout policies.

*   **Server-Side Scan:** Run a malware scanner on the web host to ensure the hacker didn't leave any vulnerability
### Mitigation & Recommendations
To secure the environment and prevent a recurrence of this brute force event, the following controls are recommended:

*   **Password Complexity Policy:** Implement a policy requiring non-default, high-entropy passwords for all administrative accounts.
*   **Account Lockout Thresholds:** Configure the server to temporarily block IP addresses after a set number of failed login attempts.
*   **Multi-Factor Authentication (MFA):** Require a second form of verification for administrative access to the web host.
*   **File Integrity Monitoring (FIM):** Implement tools to alert administrators when unauthorized changes are made to the website’s source code.

Solving this security incident goes beyond just fixing a broken website; it restores the fundamental trust between the business and its customers while significantly hardening the organization's technical defenses.

**Document the incident:**
I summarize the incident. Provide as many details and facts as possible in documentation about the issue, including where the incident occurred, how it happened, whether anyone witnessed it, and how it was discovered

**projecte impact:**

### 1. Restoration of Brand Integrity
Before the fix, the website was a liability, actively infecting customers' computers. By removing the malicious code and regaining control, you transition the site back from a "threat vector" to a "trusted service." This stops the flow of helpdesk complaints and prevents further damage to the company’s reputation.

### 2. Elimination of Unauthorized Persistence
The most immediate technical impact is the removal of the hacker's "backdoor." By resetting the administrative credentials and regaining access from the hosting provider, you terminate the attacker’s ability to modify the site. This "cleans the slate," ensuring that no lingering JavaScript functions remain to redirect users.

### 3. Technical Hardening & Future Prevention
Implementing the recommended security controls changes the website's posture from **reactive** to **proactive**:
*   **Brute Force Immunity:** With account lockout thresholds, an attacker can no longer guess passwords thousands of times.
*   **Credential Security:** Moving away from default passwords eliminates the easiest entry point for hackers.
*   **Defense in Depth:** The addition of Multi-Factor Authentication (MFA) ensures that even if a password is leaked in the future, the account remains secure.

### 4. Improved User Safety and Performance
Customers will no longer be prompted to download suspicious files, and their browsing experience will return to normal. By stopping the redirection to `greatrecipesforme.com`, you prevent the further spread of malware that was causing customer computers to run slowly, effectively "quarantining" the threat.

You will find the **Security-incident-report-template** file in my Cybersecurity Portfolio in **Apply OS hardening techniques** folder.
