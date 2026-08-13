# 🚨 Incident Timeline

## 📌 Incident

**Incident Type:** Suspicious Authentication Activity

**Affected Account:** `employee01`

**Initial Severity:** Medium–High

**Environment:** Fictional corporate environment

---

## 🕐 Timeline of Events

| Time  | Event                     | Analyst Observation                                         |
| ----- | ------------------------- | ----------------------------------------------------------- |
| 08:15 | Failed login              | First failed authentication attempt                         |
| 08:16 | Failed login              | Second failed attempt from the same IP                      |
| 08:17 | Failed login              | Third consecutive failed attempt                            |
| 08:19 | Successful login          | Successful authentication follows repeated failures         |
| 08:23 | File access               | Account accesses corporate files                            |
| 08:30 | Security alert reviewed   | Analyst begins investigation                                |
| 08:35 | Account activity reviewed | Analyst checks authentication and file-access logs          |
| 08:45 | Account contained         | Account temporarily disabled pending investigation          |
| 09:00 | Credentials reset         | User credentials are reset according to security procedures |
| 09:15 | Access reviewed           | Active sessions and permissions are reviewed                |
| 09:30 | Monitoring increased      | Additional monitoring is applied to the account             |
| 10:00 | Recovery begins           | Normal access is restored after security checks             |
| 10:30 | Incident documented       | Findings and recommendations are recorded                   |

---

## 🔎 Key Observations

### 08:15–08:17 — Failed Authentication

Three consecutive failed login attempts were recorded against `employee01`.

The attempts originated from:

`203.0.113.25`

This activity was considered potentially suspicious because several authentication failures occurred within a short period.

### 08:19 — Successful Authentication

A successful login occurred shortly after the failed attempts.

This increased the need for investigation because an attacker could potentially use password-guessing techniques to obtain valid credentials.

However, the event alone does not confirm that the account was compromised.

### 08:23 — File Access

The account accessed corporate files shortly after the successful login.

The analyst reviewed the activity to determine whether the access was authorized.

---

## 🛡️ Containment

At 08:45, the account was temporarily contained while the investigation continued.

Actions included:

* Temporarily disabling the account
* Reviewing active sessions
* Resetting credentials
* Reviewing account permissions
* Increasing monitoring

---

## 🔄 Recovery

After the account and related activity were reviewed, recovery procedures were initiated.

The account was restored after security checks were completed.

Additional monitoring was maintained to identify any further suspicious activity.

---

## 📚 Lessons Learned

The incident demonstrates the importance of:

* Monitoring authentication events
* Investigating repeated failed logins
* Reviewing successful authentication after failed attempts
* Maintaining detailed security logs
* Using appropriate access controls
* Having documented incident response procedures

---

## ⚠️ Disclaimer

This timeline is based on a fictional cybersecurity scenario created for educational purposes.

No real users, accounts, systems, or organizations were investigated.

**Author:** Mthokozisi Khulu
