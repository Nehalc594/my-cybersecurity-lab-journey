# File Inclusion

File inclusion vulnerabilities occur when an application **loads files based on user-controlled input** without proper validation.

These issues can allow attackers to **read sensitive files**, execute unintended code, or manipulate application behavior.

---

## What Is File Inclusion?

File inclusion happens when:
- An application dynamically includes files
- User input influences which file is loaded
- Validation or restriction is insufficient

File inclusion issues are commonly categorized as:
- Local File Inclusion (LFI)
- Remote File Inclusion (RFI)

---

## Why File Inclusion Is Dangerous

Successful file inclusion can lead to:
- Disclosure of sensitive configuration files
- Exposure of credentials or secrets
- Application logic manipulation
- In some cases, code execution

Impact depends on application design and server configuration.

---

## Common Causes of File Inclusion

Typical root causes include:
- Trusting user input for file paths
- Insufficient input validation
- Insecure file handling logic
- Overly permissive server configurations

These vulnerabilities often appear in templating or content-loading features.

---

## Attacker Perspective

From an attacker’s viewpoint:
- “Can I control which file is loaded?”
- “Are path traversal protections enforced?”
- “Can I access files outside the intended directory?”

Attackers test how file paths are processed.

---

## Defensive Perspective

From a defensive standpoint:
- Avoid dynamic file inclusion where possible
- Use allowlists for permitted files
- Normalize and validate file paths
- Restrict file system permissions

Defense-in-depth reduces the impact of file inclusion flaws.

---

## Common Mistakes

- Relying on blacklists for path filtering
- Assuming client-side controls are sufficient
- Exposing internal file structures
- Failing to limit file system access

---

## Key Takeaways

- File inclusion stems from unsafe file handling
- User input must never directly control file paths
- Validation and access controls are essential
- Design choices strongly influence risk
