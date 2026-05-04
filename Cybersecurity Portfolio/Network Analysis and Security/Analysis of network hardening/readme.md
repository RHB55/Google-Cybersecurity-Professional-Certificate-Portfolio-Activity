# Project Overview

I am a security analyst working for a social media organization. The organization recently experienced a major data breach, which compromised the safety of their customers’ personal information, such as names and addresses. The organization wants to implement strong network hardening practices that can be performed consistently to prevent attacks and breaches in the future. 

## Inspecting the organization’s network
I discovered four major vulnerabilities. The four vulnerabilities are as follows:
1. The organization’s employees share passwords.
2. The admin password for the database is set to the default.
3. The firewalls do not have rules in place to filter traffic coming in and out of the network.
4. Multifactor authentication (MFA) is not used.

## Undetected vulnerabilities Risks
**Employees Sharing Passwords**
* Loss of Accountability: If a malicious action occurs, you cannot prove who did it because multiple people use the same credentials.
* Expanded Attack Surface: If one employee’s computer is compromised via phishing, the attacker effectively gains the keys to every department that employee shares passwords with.
* Insider Threat Escalation: It becomes impossible to restrict access based on the "Principle of Least Privilege," as everyone has access to everything.

**Default Database Admin Password**
* Immediate Data Breach: Default passwords are listed in public databases used by hackers. An attacker can use automated scripts to gain full control of your database in seconds.
* Data Ransom/Exfiltration: Once inside the database, an attacker can encrypt your data for ransom or steal sensitive customer information to sell on the dark web.

**Lack of Firewall Traffic Filtering**
Unrestricted Malware Communication: Without "Egress" filtering, malware on an internal computer can freely "phone home" to an attacker’s server to receive commands or upload stolen data.

**No Multi-Factor Authentication (MFA)**
Credential Stuffing Vulnerability: If an employee's password is leaked in a third-party breach, an attacker can log into your organization's network immediately.

## Network hardening tools
* **Password policies:** are used to prevent attackers from easily guessing user passwords, either manually or by using a script to attempt thousands of stolen passwords (commonly called a brute force attack).
* **Configuration checks:** Updating the encryption standards for data that is stored in databases. to see if there are any unauthorized changes to the system.
* **Firewall maintenance:** Firewall maintenance entails checking and updating security configurations regularly to stay ahead of potential threats.
* **Multifactor authentication (MFA):**	A security measure that requires a user to verify their identity in two or more ways to access a system or network. MFA options include a password, pin number, badge, one-time password (OTP) sent to a cell phone, fingerprint, and more.



