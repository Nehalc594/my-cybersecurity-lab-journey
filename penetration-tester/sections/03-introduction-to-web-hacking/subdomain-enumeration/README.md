# Subdomain Enumeration

Subdomain enumeration is the process of **identifying additional domains and services** associated with a target organization.

These subdomains often host separate applications, environments, or services that may not receive the same security attention as the primary site.

---

## What Is Subdomain Enumeration?

Subdomain enumeration focuses on discovering:
- Development and staging environments
- Legacy or deprecated applications
- API endpoints and microservices
- Administrative portals
- Third-party integrations

Each subdomain represents a **potential expansion of the attack surface**.

---

## Why Subdomains Matter

Organizations frequently:
- Deploy multiple environments under different subdomains
- Expose internal tools unintentionally
- Apply inconsistent security controls across environments

Attackers often target **non-production subdomains** due to weaker monitoring and configuration.

---

## Common Sources of Subdomains

Subdomains may be discovered through:
- DNS records
- SSL/TLS certificate transparency logs
- Public documentation or source code references
- Search engine indexing

Discovery often reveals assets the organization is unaware of.

---

## Attacker Perspective

From an attacker’s viewpoint:
- “Is this subdomain less protected?”
- “Does it expose different functionality?”
- “Is authentication enforced consistently?”

Lower-visibility assets are frequent entry points.

---

## Defensive Perspective

From a defensive standpoint:
- Asset inventories must be accurate and up to date
- All environments require baseline security controls
- Non-production systems should not expose sensitive data
- Monitoring should cover all public-facing assets

---

## Common Mistakes

- Assuming subdomains are secure by default
- Forgetting to decommission unused environments
- Applying weaker controls to staging or development
- Failing to monitor subdomain traffic

---

## Key Takeaways

- Subdomains significantly expand attack surface
- Non-production systems are high-risk targets
- Enumeration improves asset visibility
- Consistent security controls are essential
