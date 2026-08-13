# 🚨 Incident Response Investigation

## 📌 Overview

This project documents a fictional cybersecurity incident involving suspicious authentication activity on a company account.

The purpose of this project is to demonstrate my understanding of **incident detection, investigation, containment, eradication, recovery, and lessons learned**.

The scenario is based on concepts covered during my cybersecurity learning, including security monitoring, authentication logs, incident response, SIEM, and the NIST Cybersecurity Framework.

## 🎯 Incident Scenario

A security analyst receives an alert indicating that an employee account has experienced multiple failed login attempts followed by a successful login from an unfamiliar IP address.

The analyst must investigate the activity and determine whether further action is required.

### Initial Alert

The security monitoring system reports:

* Multiple failed authentication attempts
* A successful login following the failed attempts
* An unfamiliar source IP address
* Activity occurring outside the user's normal working pattern

The activity is treated as **potentially suspicious** and requires investigation.

---

## 🔎 Initial Investigation

The analyst reviews available authentication logs and security alerts.

The investigation focuses on:

* Username
* Source IP address
* Login timestamps
* Number of failed attempts
* Successful authentication
* Other activity associated with the account

### Example Activity

| Time  | Event            | User       | Source IP    |
| ----- | ---------------- | ---------- | ------------ |
| 08:15 | Failed Login     | employee01 | 203.0.113.25 |
| 08:16 | Failed Login     | employee01 | 203.0.113.25 |
| 08:17 | Failed Login     | employee01 | 203.0.113.25 |
| 08:19 | Successful Login | employee01 | 203.0.113.25 |
| 08:23 | File Access      | employee01 | 203.0.113.25 |

The repeated failed authentication attempts followed by a successful login require further investigation.

---

## 🚩 Indicators of Suspicious Activity

The following indicators were identified:

### 1. Multiple Failed Logins

Several authentication attempts failed within a short period.

This could indicate:

* Incorrect credentials
* Password guessing
* Automated authentication attempts
* Account compromise attempts

### 2. Successful Login After Failed Attempts

A successful authentication occurred shortly after several failed attempts.

This increases the importance of investigating the account activity.

### 3. Unfamiliar Source IP

The login originated from an IP address that is not recognized as part of the user's normal activity.

The IP address used in this fictional scenario is:

`203.0.113.25`

### 4. Unusual File Activity

The account accessed files shortly after authentication.

The analyst should determine whether the activity was authorized.

---

# 🛡️ Incident Response Process

## 1. Preparation

Before an incident occurs, organizations should establish:

* Incident response procedures
* Security monitoring
* Logging
* Access controls
* Backup procedures
* Incident response roles
* Communication procedures

---

## 2. Detection and Analysis

The suspicious authentication activity is detected through security monitoring.

The analyst reviews:

* Authentication logs
* SIEM alerts
* Source IP addresses
* User activity
* Timestamps
* File-access events

The analyst determines that the activity requires further investigation.

---

## 3. Containment

If the investigation indicates that the account may be compromised, containment actions could include:

* Temporarily disabling the affected account
* Resetting the user's password
* Revoking active sessions
* Blocking suspicious network access where appropriate
* Increasing monitoring of related activity

Containment should be performed according to organizational procedures and authorization.

---

## 4. Eradication

After containment, the security team investigates and removes the underlying cause.

Possible actions include:

* Removing unauthorized access
* Resetting compromised credentials
* Removing malicious software if discovered
* Correcting security weaknesses
* Reviewing account permissions

---

## 5. Recovery

Recovery actions may include:

* Restoring normal account access
* Confirming that systems are secure
* Monitoring the account for additional suspicious activity
* Confirming that security controls are functioning
* Documenting the incident

Systems should be monitored closely after recovery.

---

## 6. Lessons Learned

After the incident, the organization should conduct a review.

Questions should include:

* How was the incident detected?
* What allowed the suspicious activity to occur?
* Were logs sufficient?
* Did the security alerts work correctly?
* Were access controls effective?
* Could MFA have reduced the risk?
* What improvements should be implemented?

---

# 📊 Incident Severity

### Initial Severity

**Medium to High**

The incident requires investigation because successful authentication occurred after multiple failed attempts.

The final severity would depend on additional evidence, such as:

* Whether the account was actually compromised
* Whether sensitive data was accessed
* Whether unauthorized changes occurred
* Whether other systems were affected

---

# 🧰 Security Tools and Concepts

This investigation demonstrates understanding of:

* SIEM
* Authentication logs
* Security monitoring
* Incident response
* Access control
* Network information
* User activity analysis
* NIST Cybersecurity Framework
* Principle of least privilege

---

# 📚 What I Learned

This project helped me understand that incident response is a structured process rather than simply reacting to an alert.

A security analyst must:

1. Detect suspicious activity.
2. Collect and review evidence.
3. Determine the potential impact.
4. Contain the incident.
5. Remove the underlying cause.
6. Recover affected systems.
7. Document lessons learned.

The project also reinforced the importance of accurate logs and effective security monitoring.

---

# 🚀 Future Improvements

I plan to expand this project by adding:

* A fictional SIEM alert
* Additional authentication logs
* An incident timeline
* An incident response playbook
* MITRE ATT&CK technique mapping
* Indicators of compromise
* A final incident report

---

## ⚠️ Disclaimer

This is a fictional cybersecurity incident created for educational and portfolio purposes.

No real users, accounts, IP addresses, systems, or organizations were investigated.

The IP address `203.0.113.25` is used as fictional documentation data.

---

**Author:** Mthokozisi Khulu
**GitHub:** [@mthokozisi90](https://github.com/mthokozisi90)

⭐ Part of my ongoing journey into IT Support and Cybersecurity.

