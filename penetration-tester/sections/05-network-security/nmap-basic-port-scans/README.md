# Nmap Basic Port Scans

Basic port scanning is the process of **identifying open ports on a target system** to understand which services may be accessible.

Open ports represent **potential entry points** into a system or network.

---

## What Is Port Scanning?

Port scanning involves:
- Sending probes to specific ports on a host
- Observing responses to determine port state
- Identifying which ports are open, closed, or filtered

It answers the question: **“What services can I reach?”**

---

## Why Open Ports Matter

Each open port typically corresponds to:
- A running service or application
- A protocol accepting connections
- A potential attack surface

Unnecessary or misconfigured services increase risk.

---

## Basic Port Scan Concepts

Basic port scans focus on:
- Common service ports
- Network-level responses
- Initial visibility into exposed services

They provide a starting point before deeper service analysis.

---

## Attacker Perspective

From an attacker’s mindset:
- “Which ports are open?”
- “What services might be running here?”
- “Are these ports expected or unusual?”

Attackers prioritize systems with exposed and poorly protected services.

---

## Defensive Perspective

From a defensive standpoint:
- Only required ports should be open
- Services should be hardened and monitored
- Firewall rules should restrict unnecessary exposure
- Unexpected open ports indicate misconfiguration

Port visibility informs network hardening.

---

## Common Mistakes

- Assuming open ports are harmless
- Exposing services unnecessarily
- Failing to document intended service exposure
- Ignoring filtered or inconsistent responses

---

## Key Takeaways

- Port scanning reveals exposed services
- Open ports expand attack surface
- Minimal exposure reduces risk
- Visibility supports effective defense
