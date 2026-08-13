# 🚨 Incident Response Playbook

## 📌 Purpose

This playbook provides a structured response process for suspicious authentication activity.

It is designed for a fictional corporate environment and demonstrates the basic incident response workflow used by security teams.

---

## 🎯 Trigger

This playbook should be considered when security monitoring identifies:

- Multiple failed login attempts
- Successful login after repeated failures
- Login from an unusual location or IP address
- Suspicious account activity
- Unusual file or system access

---

# 1. Detection

### Objective

Identify and confirm that a potentially suspicious event has occurred.

### Actions

- Review the security alert.
- Identify the affected username.
- Record timestamps.
- Identify the source IP address.
- Review authentication logs.
- Determine whether the activity is unusual.

### Evidence to Collect

- Authentication logs
- SIEM alerts
- Source IP addresses
- User account information
- File-access logs
- Relevant system events

---

# 2. Analysis

### Objective

Determine whether the activity may represent a security incident.

### Actions

- Count failed login attempts.
- Check whether a successful login occurred.
- Review the timing of authentication events.
- Determine whether the source IP is known.
- Review activity after successful authentication.
- Compare activity with normal user behavior.

### Important Consideration

Repeated failed logins do not automatically confirm an attack.

The analyst should collect sufficient evidence before making a final determination.

---

# 3. Containment

### Objective

Limit potential damage while the investigation continues.

### Possible Actions

- Temporarily disable the affected account.
- Reset the user's password.
- Revoke active sessions.
- Block suspicious access where authorized.
- Increase monitoring.
- Protect potentially affected systems.

### Important

Containment actions should follow organizational procedures and require appropriate authorization.

---

# 4. Eradication

### Objective

Remove the underlying cause of the security incident.

### Actions

- Remove unauthorized access.
- Reset compromised credentials.
- Remove malicious software if discovered.
- Correct security weaknesses.
- Review account permissions.
- Apply required security updates.

---

# 5. Recovery

### Objective

Safely restore normal operations.

### Actions

- Restore the affected account when appropriate.
- Confirm that security controls are functioning.
- Verify that unauthorized access has been removed.
- Monitor the account closely.
- Review systems for additional suspicious activity.

---

# 6. Post-Incident Review

### Objective

Learn from the incident and reduce the chance of recurrence.

### Questions

- How was the incident detected?
- What caused the suspicious activity?
- Were the logs sufficient?
- Did security alerts work correctly?
- Were access controls effective?
- Was MFA available?
- Could the incident have been detected earlier?
- What security improvements are required?

---

# 📊 Incident Documentation Checklist

The analyst should document:

- [ ] Incident date and time
- [ ] Affected account
- [ ] Source IP address
- [ ] Authentication events
- [ ] Evidence collected
- [ ] Initial severity
- [ ] Containment actions
- [ ] Eradication actions
- [ ] Recovery actions
- [ ] Final findings
- [ ] Lessons learned
- [ ] Recommended improvements

---

# 🛡️ Security Principles

This playbook demonstrates:

- Incident response
- Security monitoring
- Authentication analysis
- Least privilege
- Access control
- Defense in depth
- Evidence collection
- Risk assessment

---

# 📚 Reference Framework

The response process is broadly aligned with the incident response lifecycle concepts taught in cybersecurity training and the NIST Cybersecurity Framework.

---

## ⚠️ Disclaimer

This playbook is an educational portfolio project based on a fictional security incident.

No real systems, users, accounts, or organizations were investigated.

**Author:** Mthokozisi Khulu
