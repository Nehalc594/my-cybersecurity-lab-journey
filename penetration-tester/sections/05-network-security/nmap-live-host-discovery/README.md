# Nmap Live Host Discovery

Live host discovery is the process of **identifying which systems on a network are active and reachable**.

Before scanning ports or services, a penetration tester must determine **what hosts actually exist**.

---

## What Is Live Host Discovery?

Live host discovery focuses on:
- Detecting systems that respond to network probes
- Distinguishing live hosts from inactive addresses
- Understanding basic network reachability

It answers the question: **“Which systems are online?”**

---

## Why Host Discovery Matters

Effective host discovery helps testers:
- Reduce unnecessary scanning
- Focus efforts on real targets
- Minimize network noise
- Improve accuracy of later scans

Scanning non-existent hosts wastes time and increases detection risk.

---

## Host Discovery Concepts

Host discovery techniques rely on:
- Network-level responses
- Protocol behavior
- Filtering and firewall rules

Different environments may:
- Block certain probe types
- Restrict responses
- Appear “silent” despite being active

Understanding context is essential.

---

## Attacker Perspective

From an attacker’s mindset:
- “Which hosts respond to probes?”
- “Are responses filtered or blocked?”
- “Does the network behave differently for different probe types?”

Attackers adapt discovery techniques based on responses.

---

## Defensive Perspective

From a defensive standpoint:
- Host discovery often generates detectable traffic
- Firewalls and filtering reduce exposure
- Monitoring discovery patterns enables early detection

Controlling visibility limits attacker awareness.

---

## Common Mistakes

- Assuming all addresses are active
- Treating filtered responses as inactive hosts
- Running discovery without scope awareness
- Ignoring network segmentation

---

## Key Takeaways

- Host discovery identifies real targets
- Accuracy reduces noise and risk
- Network behavior affects results
- Understanding responses improves testing quality
