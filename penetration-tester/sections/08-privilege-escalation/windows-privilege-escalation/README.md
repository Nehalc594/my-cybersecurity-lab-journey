# Windows Privilege Escalation

Windows privilege escalation involves **gaining higher-level permissions** on a Windows system after initial access is obtained.

In enterprise environments, escalation often occurs due to **misconfigurations, weak access controls, or excessive privileges**, rather than zero-day exploits.

---

## Why Windows Privilege Escalation Occurs

Common causes include:
- Services running with excessive privileges
- Weak user rights assignments
- Misconfigured scheduled tasks
- Insecure registry permissions
- Poor separation between users and administrators

These issues are frequently present in real-world environments.

---

## Windows Privilege Escalation Themes

Typical escalation paths involve:
- Abusing service configurations
- Leveraging inherited permissions
- Exploiting trust relationships between components
- Accessing sensitive credentials or tokens

Understanding Windows internals is essential for accurate assessment.

---

## Importance of Enumeration

Effective escalation depends on:
- Identifying current user privileges and group memberships
- Discovering services and processes running with higher rights
- Reviewing registry and file permissions
- Understanding domain or local context

Enumeration drives escalation strategy.

---

## Attacker Perspective

From an attacker’s mindset:
- “What privileges do I already have?”
- “Which services or processes run as SYSTEM or Administrator?”
- “Can I influence higher-privileged execution?”

Attackers look for **paths of least resistance**.

---

## Defensive Perspective

From a defensive standpoint:
- Least privilege must be enforced consistently
- Services should run with minimal rights
- User rights assignments should be reviewed regularly
- Privileged activity should be logged and monitored

Strong configuration management reduces escalation risk.

---

## Common Mistakes

- Granting excessive privileges to users
- Running services as SYSTEM unnecessarily
- Ignoring inherited permissions
- Failing to audit privilege boundaries

---

## Key Takeaways

- Windows escalation often relies on misconfiguration
- Enumeration is critical to success
- Context determines viable escalation paths
- Defensive hardening prevents most issues
