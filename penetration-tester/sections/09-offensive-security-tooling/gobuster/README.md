# Gobuster

Gobuster is a tool used for **content and resource discovery** during authorized penetration tests.

It helps testers identify **hidden or unlinked resources** by systematically requesting potential paths or names.

---

## What Is Gobuster?

Gobuster is designed to:
- Enumerate directories and files
- Discover hidden endpoints
- Identify virtual hosts or DNS entries
- Support attack surface mapping

It automates discovery but does not determine exploitability.

---

## Why Content Discovery Matters

Hidden resources may include:
- Administrative interfaces
- Legacy or deprecated functionality
- Backup files or test endpoints
- Poorly protected APIs

Discovering these resources expands understanding of the application’s attack surface.

---

## Responsible Use of Enumeration

Enumeration tools must be used:
- Within defined scope
- With controlled request rates
- Without causing denial-of-service conditions
- With awareness of detection and logging

Uncontrolled enumeration creates risk and noise.

---

## Attacker Perspective

From an attacker’s mindset:
- “What exists that is not linked?”
- “Are these resources protected?”
- “Do hidden endpoints behave differently?”

Attackers rely heavily on discovery to find weak points.

---

## Defensive Perspective

From a defensive standpoint:
- Hidden content should not be relied on for security
- Unused resources should be removed
- Access controls must be enforced server-side
- Enumeration activity should be monitored

Reducing exposed content limits attacker options.

---

## Common Mistakes

- Assuming unlinked content is inaccessible
- Running enumeration without rate control
- Ignoring scope restrictions
- Treating discovery as exploitation

---

## Key Takeaways

- Gobuster supports attack surface discovery
- Enumeration reveals hidden exposure
- Responsible usage is essential
- Discovery precedes validation
