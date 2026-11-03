# Incident Response Playbook – Simulation Test Results

## Project Overview

Four fictional incident response scenarios were completed to assess incident classification, containment, investigation, escalation, recovery and documentation.

Organisation used: Northstar Financial Services.

All scenarios were tabletop exercises. No live systems were accessed or compromised.

---

## PHISH-001 – Phishing Incident

**Exercise type:** Fictional tabletop simulation

**Initial severity:** SEV 2 – High

**Outcome:** Incident contained; investigation remained open pending privacy assessment.

### Scenario

An employee received a fraudulent Microsoft 365 account suspension email, clicked the link and entered their credentials.

An unfamiliar IP address subsequently authenticated to the account, and a suspicious mailbox forwarding rule was identified.

### Response and decisions

- Correctly classified the incident as SEV 2 High.
- Identified the compromised account.
- Prioritised account containment and credential security.
- Investigated the unfamiliar login.
- Identified and removed the suspicious forwarding rule.
- Investigated mailbox access and potential data exposure.
- Assessed suspicious OAuth grants, MFA changes and other accounts.
- Referred potential data exposure for further assessment.

### Final findings

- Credential compromise: Confirmed in scenario.
- Suspicious forwarding rule: Confirmed.
- Emails accessed: 37.
- Confirmed data exfiltration: None.
- Other compromised accounts: None identified.
- Investigation: Remained open pending email and data breach assessment.

### Lessons learned

1. Phishing incidents require rapid account containment.
2. Unfamiliar authentication activity must be investigated.
3. Mailbox forwarding rules can indicate persistence.
4. Investigators should assess mailbox access and potential data exposure.

---

## ACCT-002 – Compromised Administrator Account

**Exercise type:** Fictional tabletop simulation

**Initial severity:** SEV 2 – High

**Final severity:** SEV 1 – Critical

**Outcome:** Technical recovery completed; privacy assessment remained pending.

### Scenario

An administrator account was accessed from an unfamiliar IP address.

An unauthorised account was created and added to the Domain Administrators group. Finance folder access, suspicious PowerShell activity, scheduled task persistence and attempted external communication were subsequently identified.

### Response and decisions

- Initially classified the incident as SEV 2 High.
- Escalated to SEV 1 Critical after identifying further compromise.
- Prioritised privileged account containment.
- Investigated unauthorised Active Directory changes.
- Identified scheduled task persistence.
- Investigated suspicious PowerShell activity.
- Assessed lateral movement and external communication.
- Removed unauthorised account and group membership.
- Rebuilt three affected workstations.
- Rotated credentials and restored finance folder permissions.
- Maintained enhanced monitoring.
- Kept the incident open pending privacy assessment.

### Final findings

- Unauthorised administrator activity: Confirmed.
- Unauthorised account: Removed.
- Persistence: Removed.
- Affected workstations: Three rebuilt.
- Finance records: Accessed.
- Confirmed data exfiltration: None.
- Further suspicious activity: None during 48-hour monitoring.
- Technical recovery: Completed.
- Privacy assessment: Pending.
- Incident closure: Pending privacy approval.

### Lessons learned

1. Privileged account compromise requires immediate escalation.
2. Lateral movement can significantly increase incident severity.
3. Removing one malicious IP address is not sufficient to establish containment.
4. Workstations should not be reconnected until their security has been validated.
5. Privacy assessments must be completed before final incident closure.

---

## MAL-003 – Malware Incident

**Exercise type:** Fictional tabletop simulation

**Initial severity:** SEV 2 – High

**Final severity:** SEV 1 – Critical

**Outcome:** Successfully contained, eradicated, recovered and closed in the simulation.

### Scenario

An employee downloaded a malicious executable named `invoice_viewer.exe`.

The malware executed PowerShell commands, created registry persistence, communicated with a malicious external destination and deployed a second-stage credential-stealing payload.

### Response and decisions

- Correctly classified the initial incident as SEV 2.
- Isolated the infected workstation.
- Preserved simulated malware indicators and endpoint information.
- Investigated registry persistence and PowerShell activity.
- Investigated other endpoints for matching indicators.
- Analysed the executable in an isolated environment.
- Confirmed credential theft and data exfiltration.
- Escalated the incident to SEV 1.
- Reset potentially exposed credentials and revoked sessions.
- Investigated 12 accessed business documents.
- Referred the personal data breach to the privacy team.
- Completed ICO notification and employee communications in the scenario.
- Rebuilt the affected workstation.
- Completed enhanced monitoring and obtained closure approval.

### Final findings

- Malware execution: Confirmed.
- Information-stealing payload: Confirmed.
- Persistence: Confirmed and removed.
- Credential data transfer: Confirmed.
- Personal data breach: Confirmed in scenario.
- ICO notification: Completed in simulation.
- Employee communication: Completed in simulation.
- Technical recovery: Completed.
- Incident closure: Approved in simulation.

### Lessons learned

1. Confirmed malware execution requires prompt containment.
2. Evidence must be preserved before destructive remediation.
3. Malware analysis should use an isolated environment.
4. Persistence mechanisms must be identified and removed.
5. Credential theft requires password resets and session revocation.
6. Confirmed exfiltration requires a broader impact assessment.
7. Personal data breaches require documented UK GDPR assessments.
8. Recovery requires validation and monitoring before closure.

---

## DATA-004 – Accidental External Data Disclosure

**Exercise type:** Fictional tabletop simulation

**Initial severity:** SEV 2 – High

**Outcome:** Containment, investigation, regulatory response and recovery completed in the simulation.

### Scenario

An employee accidentally emailed a spreadsheet containing 250 customer records to an unauthorised external recipient.

The spreadsheet contained names, email addresses and dates of birth.

The recipient opened and downloaded the attachment. The spreadsheet was not encrypted.

### Response and decisions

- Correctly classified the incident as SEV 2 High.
- Identified the affected information and recipient.
- Contacted the recipient and requested deletion.
- Obtained written deletion confirmation.
- Recorded that independent verification of deletion was not possible.
- Investigated potential further distribution.
- Referred the incident to the privacy team.
- Assessed the likelihood and severity of harm.
- Completed the simulated ICO notification.
- Completed simulated communications to all 250 affected customers.
- Identified weaknesses in external email controls.
- Recommended data loss prevention, approval controls, permissions reviews, staff training and encryption improvements.

### Final findings

- Customer records affected: 250.
- Unauthorised recipient: Confirmed.
- Attachment opened and downloaded: Confirmed.
- Encryption: Not applied.
- Written deletion confirmation: Received.
- Independent deletion verification: Not possible.
- Further distribution: No evidence identified.
- ICO notification: Completed in simulation.
- Customer communications: Completed in simulation.
- Incident closure: Approved in simulation.

### Lessons learned

1. Accidental disclosure must be assessed promptly.
2. Data classification and encryption reduce disclosure risk.
3. Written deletion confirmation does not independently prove permanent deletion.
4. Privacy teams must assess notification requirements.
5. External email controls and approval processes should be reviewed.

---

## Overall Assessment

Four incident scenarios were completed:

| Scenario | Incident type | Final outcome |
|---|---|---|
| PHISH-001 | Phishing | Contained; investigation open |
| ACCT-002 | Compromised administrator | Technical recovery complete; privacy assessment pending |
| MAL-003 | Malware | Closed in simulation |
| DATA-004 | Data disclosure | Closed in simulation |

The exercises assessed:

- Incident severity classification.
- Incident containment and escalation.
- Investigation and evidence preservation principles.
- Malware and account compromise response.
- Data breach assessment.
- UK GDPR and ICO notification considerations.
- Recovery, monitoring and incident closure.
- Incident documentation and lessons learned.

## Exercise Limitations

All four scenarios were fictional tabletop simulations.

No actual malware was executed. No real systems, accounts, credentials or personal data were accessed. No real forensic evidence was collected. No actual ICO notifications or customer communications were issued.

The results demonstrate scenario-based decision-making and documentation practice, not live incident response experience.

