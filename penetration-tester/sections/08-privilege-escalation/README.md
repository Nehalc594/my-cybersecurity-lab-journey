# Privilege Escalation

Privilege escalation is the process of **gaining higher levels of access** than initially granted after compromising a system.

In real-world attacks, initial access is often limited.  
Privilege escalation is what turns **access into control**.

---

## What Is Privilege Escalation?

Privilege escalation occurs when an attacker:
- Gains additional permissions
- Moves from a low-privileged user to a higher-privileged one
- Accesses restricted resources or system-level control

It is a critical phase in post-exploitation.

---

## Why Privilege Escalation Matters

Most compromises start with:
- Limited user access
- Restricted application context
- Non-administrative privileges

Without privilege escalation:
- Impact is limited
- Persistence is harder
- Lateral movement is restricted

Privilege escalation unlocks the full risk.

---

## Common Privilege Escalation Paths

Privilege escalation typically involves:
- Misconfigured permissions
- Insecure services or processes
- Weak credential handling
- Trust relationships between components
- Kernel or system-level weaknesses

The root cause is often **misconfiguration**, not exploits.

---

## Linux vs Windows Privilege Escalation

While the goal is the same, approaches differ:

- **Linux** focuses on file permissions, services, environment variables, and configuration
- **Windows** focuses on user rights, services, registry settings, and domain context

Understanding the operating system is essential.

---

## Attacker Perspective

From an attacker’s mindset:
- “What permissions do I have?”
- “What runs with higher privileges?”
- “Can I influence privileged processes?”

Attackers look for **trust violations**.

---

## Defensive Perspective

From a defensive standpoint:
- Least privilege should be enforced
- Services should run with minimal rights
- Misconfigurations should be eliminated
- Privilege use should be logged and monitored

Privilege escalation failures often indicate **system hygiene issues**.

---

## Key Takeaways

- Initial access is rarely enough
- Privilege escalation defines real impact
- Misconfigurations are common root causes
- Defense depends on least privilege and monitoring
