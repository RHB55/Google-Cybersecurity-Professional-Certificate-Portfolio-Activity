# Project Overview

I am a newly hired cybersecurity analyst for an e-commerce company. The company stores information on a remote database server, since many of the employees work remotely from locations all around the world. Employees of the company regularly query, or request, data from the server to find potential customers. The database has been open to the public since the company's launch three years ago, as a cybersecurity professional, I recognize that keeping the database server open to the public is a serious vulnerability.My task is completing a vulnerability assessment of the situation to communicate the potential risks to decision makers at the company.

### Project Scope

The scope of this vulnerability assessment relates to the current access controls of the system. The assessment will cover a period of three months, from June 2026 to August 2026. NIST SP 800-30 Rev. 1 is used to guide the risk analysis of the information system.

**1. Review information about the valuable server**

The System Description highlights the relevant components, architecture, and dependencies of the system being assessed. All of these parts and connections make up the attack surface of the vulnerable information system.The Scope specifies the focus and boundaries of the assessment.

### Perform the risk assessment

**1. Explain the purpose of information system**

The purpose section helps stakeholders understand the underlying objective and intended outcome of your analysis. A purpose statement also connects the technical objectives of your analysis with the organization's goals.

The purpose of conducting a security assessment is the database server valuable to the business, and the need for securing the server because it includes sensitive information and operations the company serves. If the server is disabled, it will affect the operation of the business and may affect the marketing operations.

**2. Identify potential threats source**

Using the threat sources section of the NIST SP 800-30 Rev. 1 resource. Using what I know about the vulnerable database server I identify three potential threats. I Choose the threats based on the information I have gathered from the system description, scope, purpose, and NIST SP 800-30 Rev. 1 resource.

**3. Identify potential threat events**

NIST SP 800-30 Rev. 1 provides a comprehensive list of possible security events that could compromise a vulnerable information system — labeled Threat events. based on the threat sources I identified before, I identified three threat events that could be initiated against the server.

**4. Calculate the risk of potential threats**

By questions about each threat that I identified earlier, I estimate a Likelihood score (1-3) and Severity score (1-3) for each threat and i add scores to the corresponding columns of the Risk Assessment table After that, I calculate an overall Risk score (1-9) for each threat using the formula (likelihood x severity = risk).

### Propose security recommendations

**1. Explain your approach**

I explain why I selected the 3 specific threat sources/events I chose and why I think they're significant business risks. Estimate how bad attacks could be by judging their chances based on my security knowledge. Qualitative vulnerability assessments are useful for identifying high-level risks facing an organization. This information helps organizations make informed decisions about resource allocation, project planning, and other aspects of their business operations.

**2. propose a remediation strategy**

By thinking about the risks that could be remediated or mitigated using security controls like:

- Principle of least privilege 
- Defense in depth
- Multi-factor authentication (MFA)
- Authentication, Authorization, Accounting (AAA) framework

I summarize specific security controls that could be implemented to remediate or mitigate the risks to the information system.
