# Command Injection

Command injection vulnerabilities occur when an application **executes system commands using untrusted input** without proper validation.

These flaws allow attackers to **influence or execute unintended operating system commands**.

---

## What Is Command Injection?

Command injection happens when:
- An application passes user input to system-level commands
- Input is not properly validated or sanitized
- The operating system interprets the input as part of a command

This vulnerability bridges application logic and the underlying system.

---

## Why Command Injection Is Critical

Successful command injection can lead to:
- Full system compromise
- Unauthorized access to sensitive data
- Lateral movement within environments
- Persistence and further exploitation

Impact is often severe because it affects the host directly.

---

## Common Causes of Command Injection

Typical root causes include:
- Using system calls with user-supplied input
- Improper input sanitization
- Relying on blacklists instead of safe APIs
- Insecure scripting practices

These issues often appear in legacy or poorly designed features.

---

## Attacker Perspective

From an attacker’s mindset:
- “Is user input passed to the OS?”
- “Can I influence command execution?”
- “Are inputs properly escaped or validated?”

Attackers test how input interacts with system calls.

---

## Defensive Perspective

From a defensive standpoint:
- Avoid using system commands where possible
- Use parameterized APIs or safe libraries
- Strictly validate and sanitize input
- Apply least privilege to executing processes

Defense-in-depth limits impact if exploitation occurs.

---

## Common Mistakes

- Trusting user input in command execution
- Using weak input filtering
- Running commands with excessive privileges
- Failing to audit system command usage

---

## Key Takeaways

- Command injection affects the operating system
- Untrusted input must never reach system commands
- Secure APIs reduce risk significantly
- Privilege separation limits damage
