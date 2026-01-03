# Linux Privilege Escalation

Linux privilege escalation involves **gaining higher permissions on a Linux system** after initial access has been obtained.

In many cases, escalation is possible due to **misconfiguration rather than software exploits**.

---

## Why Linux Privilege Escalation Occurs

Common causes include:
- Incorrect file or directory permissions
- Insecure service configurations
- Weak credential handling
- Poor separation of privileges
- Unsafe environment variables

These issues are often preventable with proper system hardening.

---

## Common Linux Privilege Escalation Themes

Linux escalation typically focuses on:
- Files or processes running with elevated privileges
- Misconfigured scheduled tasks or services
- Trust relationships between users and processes
- Improper access to sensitive system files

Understanding the system context is essential.

---

## Enumeration Is Critical

Effective escalation depends on:
- Identifying current user privileges
- Discovering what the user can execute
- Understanding file ownership and permissions
- Mapping running processes and services

Enumeration informs decision-making.

---

## Attacker Perspective

From an attacker’s mindset:
- “What can I access or modify?”
- “What runs as a higher-privileged user?”
- “Can I influence privileged behavior?”

Attackers look for trust violations and shortcuts.

---

## Defensive Perspective

From a defensive standpoint:
- Least privilege should be enforced
- Services should not run with excessive rights
- File permissions should be restrictive
- Monitoring should detect privilege abuse

Strong configuration management reduces risk.

---

## Common Mistakes

- Overlooking simple permission issues
- Running services as root unnecessarily
- Ignoring environment variable security
- Failing to audit privilege boundaries

---

## Key Takeaways

- Linux escalation often relies on misconfigurations
- Enumeration drives successful escalation
- Context matters more than exploits
- Proper hardening prevents most issues
