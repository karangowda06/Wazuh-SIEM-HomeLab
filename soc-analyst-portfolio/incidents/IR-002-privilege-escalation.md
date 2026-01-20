Incident ID: IR-002
Type: Privilege Escalation  
Severity: Critical  
MITRE ATT&CK: T1068  

Summary
Suspicious privilege escalation activity was detected on a Linux host involving
the use of elevated privileges by a non-administrative user.

Evidence
- Log Source: /var/log/auth.log
- Detection Rule ID: 100020
- User Account: testuser
- Command Executed: sudo su

Analysis
The user account attempted to obtain root-level access without a documented
business requirement. This behavior is consistent with post-compromise activity
following initial access.

Response Actions
- User account temporarily disabled
- Host reviewed for persistence mechanisms
- Privileged access logs audited

Outcome
No additional malicious activity detected. Privilege escalation attempt contained.
