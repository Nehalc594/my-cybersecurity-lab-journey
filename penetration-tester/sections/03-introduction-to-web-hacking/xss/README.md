# Cross-Site Scripting (XSS)

Cross-Site Scripting (XSS) vulnerabilities occur when an application **includes untrusted input in its output** without proper validation or encoding.

This allows attackers to **execute malicious scripts in a victim’s browser**.

---

## What Is XSS?

XSS happens when:
- User-controlled input is reflected or stored
- The application fails to safely encode output
- The browser interprets the input as executable script

XSS targets **users**, not the server directly.

---

## Why XSS Is Dangerous

XSS vulnerabilities can lead to:
- Session hijacking
- Account takeover
- Data theft
- Phishing and social engineering attacks
- Defacement or malicious redirection

Impact depends on application context and user privileges.

---

## Common Types of XSS

- **Reflected XSS**: Input is immediately reflected in the response
- **Stored XSS**: Malicious input is saved and later served to users
- **DOM-based XSS**: Client-side JavaScript processes untrusted input

All forms result from **unsafe handling of user input**.

---

## Attacker Perspective

From an attacker’s mindset:
- “Where is user input rendered?”
- “Is output encoded based on context?”
- “Can I influence JavaScript execution?”

Attackers look for trust boundaries between input and output.

---

## Defensive Perspective

From a defensive standpoint:
- Validate input and encode output properly
- Apply context-aware encoding (HTML, JS, URL)
- Use security headers where appropriate
- Avoid dangerous client-side patterns

Defense requires both server-side and client-side controls.

---

## Common Mistakes

- Relying solely on input filtering
- Using incorrect encoding for context
- Trusting client-side validation
- Underestimating impact on privileged users

---

## Key Takeaways

- XSS targets users through their browsers
- Unsafe output handling is the root cause
- Proper encoding is essential
- Context awareness determines security
