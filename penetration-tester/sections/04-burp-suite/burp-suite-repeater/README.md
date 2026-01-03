# Burp Suite: Repeater

Burp Suite Repeater is a tool for **manually replaying and modifying HTTP/S requests** in a controlled and repeatable way.

It allows penetration testers to test application behavior **precisely and deliberately**, without automation noise.

---

## What Is Repeater?

Repeater allows a tester to:
- Send the same request multiple times
- Modify parameters, headers, or body content
- Observe how small changes affect responses
- Validate logic and access control decisions

It is designed for **manual testing and confirmation**.

---

## Why Repeater Is Important

Many vulnerabilities:
- Require exact request crafting
- Depend on specific sequences or values
- Are hidden behind normal UI behavior

Repeater enables testers to:
- Remove randomness
- Test assumptions systematically
- Confirm whether behavior is exploitable

Repeatability is critical for reliable findings.

---

## Common Use Cases

Repeater is commonly used to:
- Validate authentication and authorization checks
- Test IDOR and access control behavior
- Modify hidden or client-controlled parameters
- Replay requests after changing user context

It supports careful reasoning over brute force.

---

## Attacker Perspective

From an attacker’s mindset:
- “What happens if I repeat this request?”
- “Does changing this value affect access?”
- “Is the server validating each request?”

Attackers rely on repeatability to confirm flaws.

---

## Defensive Perspective

From a defensive standpoint:
- Repeater shows how attackers test logic
- Inconsistent enforcement becomes visible
- Missing server-side checks are exposed

Defenders can use this insight to harden controls and logging.

---

## Common Mistakes

- Treating Repeater as an automation tool
- Ignoring response differences
- Testing without understanding context
- Failing to document tested variations

Repeater is about **precision, not speed**.

---

## Key Takeaways

- Repeater enables controlled request replay
- Precision testing reveals logic flaws
- Repeatability strengthens findings
- Manual validation improves credibility
