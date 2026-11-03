\# Compromised Account Incident Response



\## 1. Purpose



This procedure establishes the steps required to identify, investigate, contain and recover from compromised user or administrator accounts.



Account compromise occurs when an unauthorised individual gains access to legitimate credentials, authentication sessions or account privileges.



\## 2. Identification Indicators



Potential indicators include:



\- Successful logins from unfamiliar locations or devices.

\- Multiple failed login attempts followed by a successful login.

\- Unexpected MFA approval requests.

\- Unauthorised password changes.

\- Suspicious account recovery activity.

\- Unexpected privilege escalation.

\- Unrecognised mailbox forwarding rules.

\- Unusual access to confidential files.

\- Suspicious OAuth application permissions.

\- Unusual activity outside normal working hours.



\## 3. Initial Assessment



The analyst must establish:



1\. Which account is affected?

2\. Is the account a standard user or administrator?

3\. When did suspicious activity begin?

4\. Which IP addresses and devices were involved?

5\. Were authentication credentials or MFA methods compromised?

6\. Were existing sessions or tokens accessed?

7\. What systems and information could the account access?

8\. Are other accounts showing similar activity?



Assign severity using the incident classification procedure.



\## 4. Investigation



\### Authentication Analysis



Review:



\- Successful and failed login records.

\- Source IP addresses.

\- Login timestamps.

\- Device and browser information.

\- MFA events.

\- Password reset history.

\- Session and token activity.



\### Account Configuration Review



Investigate:



\- Account permissions.

\- Administrator privileges.

\- Group memberships.

\- Mailbox forwarding rules.

\- Delegated access.

\- OAuth application permissions.

\- Registered authentication methods.



\### Lateral Movement Assessment



Determine whether the compromised account was used to:



\- Access additional systems.

\- Create or modify other accounts.

\- Obtain additional privileges.

\- Access shared folders or network resources.

\- Access remote administration services.

\- Attempt to compromise other users.



\## 5. Containment



1\. Notify the incident lead.

2\. Temporarily disable or restrict the compromised account through an authorised administrator.

3\. Revoke active sessions and refresh tokens where supported.

4\. Preserve relevant authentication and audit logs.

5\. Reset compromised credentials using a trusted device and communication channel.

6\. Review and secure MFA methods.

7\. Remove unauthorised application permissions and mailbox rules after preserving evidence.

8\. Investigate other potentially affected accounts.

9\. Restrict suspicious access to critical systems where necessary.



\## 6. Evidence Preservation



Preserve:



\- Authentication logs.

\- Source IP addresses.

\- Login timestamps.

\- MFA activity.

\- Session and token records.

\- Password reset events.

\- Account permission changes.

\- Group membership changes.

\- Mailbox and application audit records.

\- Relevant endpoint and network logs.



Record evidence references, collection timestamps and responsible personnel.



Never collect plaintext passwords as evidence.



\## 7. Eradication



1\. Identify the original compromise method.

2\. Remove unauthorised account permissions.

3\. Remove suspicious application grants and persistence mechanisms.

4\. Correct exploited vulnerabilities.

5\. Reset affected credentials and secrets.

6\. Review other accounts for reused credentials or related compromise.

7\. Confirm that unauthorised access has been removed.



\## 8. Recovery



1\. Verify the employee's identity.

2\. Restore account access only after security checks.

3\. Enforce appropriate MFA.

4\. Review account permissions.

5\. Confirm legitimate applications and devices.

6\. Monitor authentication activity.

7\. Confirm that business services are functioning normally.



\## 9. Escalation Criteria



Escalate immediately when:



\- An administrator account is compromised.

\- Multiple accounts show suspicious activity.

\- Sensitive information may have been accessed.

\- Evidence of lateral movement exists.

\- Privileges have been escalated without authorisation.

\- Financial systems or critical services are affected.



\## 10. Incident Closure



Before closing the incident, confirm:



\- The compromised account is secured.

\- Active unauthorised sessions have been revoked.

\- Unauthorised permissions have been removed.

\- Other affected accounts have been investigated.

\- Relevant evidence has been preserved.

\- The root cause has been documented.

\- Recovery has been validated.

\- Outstanding risks and corrective actions are recorded.



\## 11. Lessons Learned



Review opportunities to improve:



\- Multi-factor authentication.

\- Conditional access policies.

\- Privileged access management.

\- Password security.

\- Account monitoring.

\- Authentication alerting.

\- User security awareness.

