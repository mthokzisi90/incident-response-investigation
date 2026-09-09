# Incident Response Investigation: Suspicious Authentication Activity

## Overview

This is a safe, fictional incident-response lab. It investigates repeated failed login attempts followed by a successful login to the account `employee01`. The repository contains simulated evidence and a small Python script that reproduces the investigation findings.

No systems were accessed, scanned, attacked, or changed. The IP addresses in this project (`203.0.113.25` and `192.0.2.44`) are documentation-only example addresses.

## Scenario

On 8 September 2026, a security alert identified three failed login attempts against `employee01` from `203.0.113.25`. A successful login from the same address followed two minutes later, then the account accessed a corporate file share. The activity is treated as suspicious, but the logs alone do not prove account compromise.

| Field | Details |
| --- | --- |
| Incident type | Suspicious authentication activity |
| Affected account | `employee01` |
| Initial severity | Medium–High |
| Environment | Fictional corporate environment |
| Status | Resolved / monitoring (simulated) |

## Evidence and analysis

The sample event log is stored in `data/security-events.log`. Run the analysis from the repository root:

```bash
python3 src/analyze_events.py
```

The script identifies repeated failures, successful logins, and file-access activity from the same source IP. Its output shows that `203.0.113.25` reached the three-failure alert threshold and later authenticated successfully as `employee01`.

## Incident response lifecycle

| Phase | What was done in this lab |
| --- | --- |
| Detection | Identified repeated failed logins and a successful login from the same IP. |
| Analysis | Reviewed timestamps, account name, source IP, and subsequent file access. |
| Containment | Documented simulated account disablement, session review, and credential reset. |
| Eradication | Documented a review of account permissions and removal of unauthorised access, if found. |
| Recovery | Documented restoration of access after security checks and increased monitoring. |
| Lessons learned | Recommended MFA, alerting, log retention, and review of unusual access. |

## Project structure

```text
incident-response-investigation/
├── data/                         # Safe simulated event evidence
├── evidence/screenshots/          # Screenshots collected while running the lab
├── reports/                       # Final incident report
├── src/                           # Python event analysis
├── incident-response-playbook.md
├── incident-timeline.md
└── README.md
```

## Screenshots to add

After running the lab, add your own screenshots to `evidence/screenshots/`:

1. VS Code showing the project structure.
2. The simulated log file open in VS Code.
3. A terminal showing the Python analysis output.
4. The incident report open in VS Code.

Do not include passwords, API keys, personal email addresses, or private paths in screenshots.

## Skills demonstrated

Python, authentication-log analysis, evidence handling, incident triage, containment planning, access-control review, incident documentation, and NIST incident-response concepts.

## Disclaimer

This is an educational portfolio project based entirely on fictional events and simulated logs. It is not an investigation of a real person, company, account, or system.

**Author:** Mthokozisi Khulu  
**GitHub:** [@mthokzisi90](https://github.com/mthokzisi90)
