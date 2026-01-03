# Active Reconnaissance

Active reconnaissance involves **direct interaction with target systems** to gather information about hosts, services, and network behavior.

Unlike passive reconnaissance, active techniques generate traffic that may be **logged or detected**.

---

## What Is Active Reconnaissance?

Active reconnaissance focuses on:
- Identifying live hosts
- Discovering open ports
- Detecting exposed services
- Understanding network response behavior

These techniques provide **accurate, real-time visibility** into the environment.

---

## Why Active Reconnaissance Matters

Active reconnaissance allows testers to:
- Confirm which systems are reachable
- Identify actual attack surface
- Validate assumptions from passive recon
- Discover misconfigurations and weak services

It bridges the gap between theory and reality.

---

## Risk and Detection Considerations

Because active recon:
- Sends packets to target systems
- May trigger alerts or logs
- Can affect system performance if misused

It must always be:
- Authorized
- Scoped
- Performed carefully and deliberately

Uncontrolled scanning can cause operational issues.

---

## Attacker Perspective

From an attacker’s mindset:
- “Which hosts respond?”
- “What services are exposed?”
- “Are there signs of monitoring or filtering?”

Attackers adjust tactics based on observed responses.

---

## Defensive Perspective

From a defensive standpoint:
- Active recon often appears as scanning activity
- IDS/IPS and firewalls may detect probes
- Logs can reveal attacker intent and patterns

Monitoring active reconnaissance improves early detection.

---

## Common Mistakes

- Scanning without authorization
- Running aggressive scans too early
- Ignoring scope and exclusions
- Misinterpreting filtered or blocked responses

---

## Key Takeaways

- Active reconnaissance provides real-world visibility
- Direct interaction increases detection risk
- Controlled scanning is essential
- Authorization and scope are mandatory
