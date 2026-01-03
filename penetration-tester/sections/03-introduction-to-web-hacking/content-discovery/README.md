# Content Discovery

Content discovery is the process of **identifying hidden or unlinked resources** within a web application.

These resources may not be visible through normal navigation but can significantly expand the attack surface.

---

## What Is Content Discovery?

Content discovery focuses on finding:
- Hidden directories and endpoints
- Unlinked pages or APIs
- Backup or legacy files
- Administrative or debug functionality

Many vulnerabilities exist in areas developers did not intend to expose publicly.

---

## Why Content Discovery Matters

Applications often contain:
- Features under development
- Deprecated functionality
- Misconfigured access controls
- Forgotten files or endpoints

Attackers frequently discover vulnerabilities simply by **accessing functionality others overlooked**.

---

## Types of Content Discovery

### Manual Discovery
- Observing links and application behavior
- Reviewing JavaScript files
- Modifying URLs and parameters logically

### Automated Discovery
- Using tools to enumerate directories or endpoints
- Identifying common file and folder patterns

Automation supports discovery, but **manual validation is required**.

---

## Attacker Perspective

From an attacker’s mindset:
- “What exists that isn’t linked?”
- “Is this endpoint protected?”
- “Was this intended to be public?”

Hidden functionality often has weaker security controls.

---

## Defensive Perspective

From a defender’s viewpoint:
- Unused content should be removed
- Sensitive endpoints must be protected
- Access controls must be enforced server-side
- Security through obscurity is insufficient

---

## Common Mistakes

- Assuming hidden content is inaccessible
- Relying only on client-side restrictions
- Failing to review legacy resources
- Not validating discovered endpoints

---

## Key Takeaways

- Hidden content increases attack surface
- Discovery often reveals high-impact issues
- Manual analysis complements automation
- Proper access control is essential
