# Passive Reconnaissance

Passive reconnaissance is the process of **gathering information about a target without directly interacting with its systems**.

It is typically the **first phase of network penetration testing** because it minimizes risk and avoids detection.

---

## What Is Passive Reconnaissance?

Passive reconnaissance focuses on collecting information from:
- Publicly available sources
- Third-party services
- Documentation and metadata
- Previously exposed data

No packets are sent directly to the target’s infrastructure.

---

## Why Passive Reconnaissance Matters

Passive reconnaissance helps testers:
- Build an initial understanding of the environment
- Identify potential targets and technologies
- Reduce unnecessary active scanning
- Avoid alerting defensive monitoring systems

Much can be learned **before touching the network**.

---

## Common Passive Reconnaissance Sources

Information is often gathered from:
- DNS records and public registries
- Certificate transparency logs
- Search engines and cached content
- Public code repositories
- Documentation and job postings

These sources frequently reveal architecture details unintentionally.

---

## Attacker Perspective

From an attacker’s mindset:
- “What is already exposed publicly?”
- “Which technologies are in use?”
- “Are there patterns across environments?”

Attackers often rely heavily on passive recon to plan next steps.

---

## Defensive Perspective

From a defensive standpoint:
- Public exposure should be minimized
- Sensitive information should not be leaked
- Asset inventories must include public-facing data
- Monitoring should include OSINT awareness

Reducing passive information leakage limits attacker advantage.

---

## Common Mistakes

- Ignoring publicly available information
- Assuming exposure is harmless
- Failing to review external data regularly
- Overlooking third-party disclosures

---

## Key Takeaways

- Passive reconnaissance is low-risk and valuable
- Public data can reveal sensitive insights
- Preparation improves active testing quality
- Reducing exposure improves security posture
