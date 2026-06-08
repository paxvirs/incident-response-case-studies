# Case Study 002: Phishing Email Investigation

## Executive Summary

On 2026-06-09, a user reported receiving a suspicious email claiming that their Microsoft 365 account would be suspended unless immediate action was taken. The message contained a hyperlink directing the recipient to a credential submission page.

An investigation was initiated to determine the legitimacy of the email, assess potential risk, identify indicators of compromise, and recommend appropriate response actions.

Analysis determined that the email was a phishing attempt designed to harvest user credentials through social engineering techniques. No evidence indicated that the user interacted with the malicious link or submitted credentials.

---

## Incident Information

### Incident Type

Phishing Attempt

### Severity

High

### Status

Closed

### Detection Method

User Report

### Affected Asset

Corporate Email Account

### Investigation Date

2026-06-09

---

## Initial Alert

A user reported receiving an email that requested immediate account verification and warned that failure to act would result in account suspension.

The email contained urgent language and a hyperlink directing the recipient to an external website.

---

## Email Analysis

### Subject

Urgent: Verify Your Account to Avoid Suspension

### Sender Domain

security-notification-example[.]com

### Link Observed

hxxps://account-verification-example[.]com

### Attachment

None

---

## Indicators of Compromise (IOCs)

* Suspicious sender domain
* Urgent language designed to create panic
* Credential harvesting theme
* External login page
* Domain impersonation attempt

---

## Evidence Collected

### Observed Characteristics

* Email requested immediate action
* Hyperlink directed users to a non-corporate domain
* Sender domain was unrelated to the claimed organization
* Message attempted to create a sense of urgency

### Social Engineering Indicators

* Fear of account suspension
* Pressure to act immediately
* Impersonation of a trusted service provider

---

## MITRE ATT&CK Mapping

### Tactic

Initial Access

### Technique

T1566 - Phishing

### Sub-Technique

T1566.002 - Spearphishing Link

Description:

Adversaries may send emails containing malicious links that direct victims to credential harvesting pages or malicious websites.

---

## Investigation Timeline

### 09:15 UTC

User reported suspicious email.

### 09:20 UTC

Email reviewed by security analyst.

### 09:25 UTC

Sender domain analyzed.

### 09:30 UTC

Embedded hyperlink inspected.

### 09:35 UTC

Indicators consistent with phishing activity identified.

### 09:40 UTC

User activity reviewed.

### 09:45 UTC

No evidence of link interaction or credential submission discovered.

### 09:50 UTC

Incident classified as phishing attempt.

---

## Analysis

The investigation determined that the email was crafted to impersonate a trusted service provider and persuade the recipient to disclose credentials.

The sender domain did not belong to the organization being represented, and the embedded URL directed users to an unrelated external site.

The attack relied on social engineering techniques, including urgency and fear, to influence user behavior.

No indicators suggested successful credential compromise.

---

## Risk Assessment

### Likelihood

High

### Impact

High

### Risk Rating

High

Justification:

Had the user submitted credentials, the attacker could have gained unauthorized access to organizational resources. Although no compromise occurred, the attack presented significant risk.

---

## Detection Opportunities

Security teams can identify similar threats through:

* Email gateway monitoring
* Domain reputation analysis
* User-reported phishing messages
* URL filtering alerts
* Threat intelligence feeds

---

## Containment Actions

* Email quarantined and removed
* Sender domain blocked
* Security team notified
* User advised not to interact with the message

---

## Recommendations

1. Enforce Multi-Factor Authentication (MFA).
2. Conduct regular phishing awareness training.
3. Implement advanced email filtering controls.
4. Verify sender domains before responding to requests.
5. Encourage prompt reporting of suspicious messages.

---

## Analyst Notes

This phishing attempt demonstrates how attackers exploit urgency and trust to obtain credentials.

User awareness played a critical role in preventing compromise. Early reporting enabled rapid investigation and reduced organizational risk.

---

## Lessons Learned

Users remain an essential layer of defense against phishing attacks.

Regular security awareness training and technical email controls significantly improve an organization's ability to detect and prevent credential theft.

---

## Conclusion

The incident was classified as a phishing attempt targeting user credentials.

Investigation confirmed the presence of multiple phishing indicators, including domain impersonation and social engineering tactics. No evidence of credential compromise or user interaction was identified.

The attack was unsuccessful, and recommendations were provided to strengthen future defenses.
