\# Phishing Incident Response Procedure



\## 1. Purpose



This procedure establishes the steps required to identify, investigate, contain and resolve phishing incidents.



Phishing is a social engineering attack in which an attacker attempts to deceive individuals into revealing sensitive information, downloading malicious files or performing unauthorised actions.



\## 2. Initial Identification



Potential phishing indicators include:



\- Suspicious sender addresses or domains.

\- Unexpected attachments or links.

\- Requests for passwords or confidential information.

\- Urgent payment or account verification requests.

\- Unexpected MFA approval requests.

\- Impersonation of colleagues, suppliers or recognised organisations.

\- Suspicious email headers or authentication failures.



\## 3. Initial Assessment



The analyst must establish:



1\. Who received the message?

2\. When was it received?

3\. Was the email opened?

4\. Was a link clicked?

5\. Was an attachment downloaded or executed?

6\. Were credentials entered?

7\. Was an MFA request approved?

8\. Did other employees receive the same message?



The incident must be classified using the severity assessment procedure.



\## 4. Investigation



\### Email Analysis



Inspect the following:



\- Sender address.

\- Reply-to address.

\- Subject line.

\- Email headers.

\- SPF authentication result.

\- DKIM authentication result.

\- DMARC authentication result.

\- Embedded URLs.

\- Attachment names and file hashes.



\### URL Analysis



Examine suspicious URLs using approved security analysis tools.



Do not open suspicious links directly on a normal workstation.



Record the URL, domain, redirect behaviour and any available threat intelligence findings.



\### Attachment Analysis



Record:



\- Filename.

\- File extension.

\- File size.

\- SHA-256 hash.

\- Antivirus or endpoint detection results.



Do not execute suspicious attachments during investigation.



\## 5. Containment



If the email is confirmed malicious:



1\. Notify the incident lead.

2\. Identify all affected recipients.

3\. Request that the authorised email administrator quarantines or removes malicious messages.

4\. Block confirmed malicious domains, URLs and sender addresses where appropriate.

5\. Warn affected employees through a trusted communication channel.

6\. If credentials were disclosed, initiate the compromised-account response procedure.

7\. If malware was executed, initiate the malware response procedure.



\## 6. Evidence Preservation



Preserve:



\- Original email.

\- Full email headers.

\- Sender and recipient information.

\- Suspicious URLs.

\- Attachment files and SHA-256 hashes where appropriate.

\- Email gateway logs.

\- Relevant authentication logs.

\- User interaction timeline.



Assign evidence reference numbers and document who collected each item.



\## 7. Recovery



1\. Confirm malicious emails have been contained.

2\. Secure affected accounts.

3\. Revoke compromised sessions where applicable.

4\. Investigate potentially affected endpoints.

5\. Verify that no further suspicious activity is occurring.

6\. Monitor affected users and systems.



\## 8. Escalation Criteria



Escalate immediately when:



\- Credentials have been disclosed.

\- An MFA request has been approved unexpectedly.

\- A malicious attachment has been executed.

\- Multiple employees have interacted with the email.

\- Financial information or payments may have been compromised.

\- Sensitive or personal data may have been accessed.



\## 9. Incident Closure



Before closure, confirm:



\- The phishing message has been contained.

\- Affected users have been identified.

\- Compromised accounts have been secured.

\- Relevant evidence has been preserved.

\- The incident timeline has been completed.

\- Outstanding risks have been documented.

\- Corrective actions have been assigned.



\## 10. Lessons Learned



Review how the phishing email bypassed existing controls and identify opportunities to improve:



\- Email filtering.

\- Multi-factor authentication.

\- Security awareness training.

\- Domain protection.

\- User reporting procedures.

\- Endpoint security controls.

