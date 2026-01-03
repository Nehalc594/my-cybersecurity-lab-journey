# Insecure Direct Object References (IDOR)

IDOR vulnerabilities occur when an application **exposes internal object references** (such as IDs) and fails to properly enforce authorization checks.

These issues allow users to **access or modify resources they do not own**.

---

## What Is an IDOR?

An IDOR happens when:
- A user-controlled identifier is used to access an object
- The application does not verify that the user is authorized
- Access decisions are based solely on the provided identifier

This is a form of **broken authorization**, not authentication.

---

## Why IDOR Is High Impact

IDOR vulnerabilities can lead to:
- Unauthorized data exposure
- Modification or deletion of other users’ data
- Account takeover scenarios
- Regulatory and privacy violations

They are common and often easy to exploit once discovered.

---

## Common IDOR Scenarios

Typical examples include:
- Accessing another user’s profile by changing an ID
- Downloading files belonging to other users
- Modifying orders, tickets, or records not owned by the attacker

These issues frequently appear in APIs and modern web applications.

---

## Attacker Perspective

From an attacker’s mindset:
- “What happens if I change this ID?”
- “Does the server verify ownership?”
- “Are access checks consistent across endpoints?”

Attackers test object references systematically.

---

## Defensive Perspective

From a defensive standpoint:
- Authorization must be enforced server-side
- Object ownership must be verified for every request
- Indirect references or access control layers can reduce risk
- Authorization failures should be logged

Strong authorization controls are essential.

---

## Common Mistakes

- Assuming authenticated users are authorized
- Relying on client-side restrictions
- Applying access checks inconsistently
- Failing to test APIs thoroughly

---

## Key Takeaways

- IDOR is a broken authorization issue
- User-controlled IDs require strict validation
- Server-side checks are mandatory
- IDOR flaws often affect APIs and business logic
