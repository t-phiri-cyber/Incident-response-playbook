\# Security Incident Severity Assessment



\## 1. Purpose



This document establishes the criteria used to assess and classify cybersecurity incidents. The classification determines escalation priority, response urgency and the level of management involvement required.



\## 2. Severity Levels



\### SEV 1 – Critical



\*\*Indicators:\*\*

\- Active ransomware affecting critical infrastructure.

\- Widespread unauthorised access.

\- Confirmed large-scale sensitive data exposure.

\- Destructive malware affecting multiple systems.

\- Critical business services unavailable due to a cyberattack.



\*\*Required response:\*\*

\- Immediately escalate to senior management and the incident lead.

\- Initiate emergency containment procedures.

\- Engage relevant technical and legal personnel.

\- Preserve evidence.

\- Maintain an incident timeline.

\- Assess business continuity requirements.



\### SEV 2 – High



\*\*Indicators:\*\*

\- Confirmed administrator account compromise.

\- Malware execution on a corporate endpoint.

\- Unauthorised access to sensitive information.

\- Multiple compromised user accounts.

\- Suspected data exfiltration.



\*\*Required response:\*\*

\- Notify the incident lead immediately.

\- Restrict affected accounts or devices.

\- Preserve authentication and endpoint logs.

\- Investigate the extent of compromise.

\- Review access permissions and credentials.



\### SEV 3 – Medium



\*\*Indicators:\*\*

\- Employee interacts with a suspicious phishing email.

\- Repeated failed login attempts.

\- Suspicious account activity without confirmed compromise.

\- Isolated security alerts requiring investigation.



\*\*Required response:\*\*

\- Record the incident.

\- Investigate relevant logs and activity.

\- Determine whether containment is necessary.

\- Escalate if evidence indicates further compromise.



\### SEV 4 – Low



\*\*Indicators:\*\*

\- Phishing email successfully blocked.

\- Suspicious attachment quarantined before execution.

\- Isolated unsuccessful login attempt.

\- Security alert confirmed as benign.



\*\*Required response:\*\*

\- Record the event.

\- Validate the detection.

\- Document the outcome.

\- Close the event or continue monitoring where appropriate.



\## 3. Severity Assessment Factors



Analysts must consider:



1\. Scope – How many users, systems or services are affected?

2\. Impact – What damage has occurred or could occur?

3\. Data sensitivity – Is personal, financial or confidential information involved?

4\. Privilege – Does the incident involve administrator access?

5\. Persistence – Is the threat still active?

6\. Business continuity – Are essential services disrupted?



\## 4. Escalation Requirements



Severity must be reassessed whenever new evidence changes the understanding of the incident.



An incident may be upgraded or downgraded following investigation.



When classification is uncertain, escalate to the incident lead rather than assuming the lowest severity.



\## 5. Classification Principle



Severity is determined by the overall risk and impact of the incident, not simply by the type of alert generated.



A blocked phishing email may be SEV 4, while successful credential theft through phishing may become SEV 2 or higher depending on access and impact.

