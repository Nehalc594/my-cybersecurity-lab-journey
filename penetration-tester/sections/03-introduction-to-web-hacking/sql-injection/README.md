# SQL Injection

SQL Injection (SQLi) vulnerabilities occur when an application **constructs database queries using untrusted input** without proper handling.

These flaws allow attackers to **manipulate database queries** and access or modify data beyond intended limits.

---

## What Is SQL Injection?

SQL injection happens when:
- User input is embedded directly into SQL queries
- Input is not properly parameterized or validated
- The database interprets the input as part of the query logic

This vulnerability targets the **data layer** of an application.

---

## Why SQL Injection Is High Impact

Successful SQL injection can lead to:
- Unauthorized data disclosure
- Modification or deletion of records
- Authentication bypass
- Complete database compromise

Because databases often store sensitive information, impact is frequently severe.

---

## Common Causes of SQL Injection

Typical root causes include:
- Dynamic query construction with user input
- Lack of parameterized queries
- Improper input validation
- Legacy code and insecure database access patterns

SQL injection is preventable with secure development practices.

---

## Attacker Perspective

From an attacker’s mindset:
- “Is my input affecting the query structure?”
- “Are errors revealing database behavior?”
- “Is input safely parameterized?”

Attackers test how input interacts with backend queries.

---

## Defensive Perspective

From a defensive standpoint:
- Use parameterized queries or prepared statements
- Apply least privilege to database accounts
- Validate input based on expected format
- Monitor database activity for anomalies

Defense must be implemented at both the application and database layers.

---

## Common Mistakes

- Relying on input filtering alone
- Concatenating user input into queries
- Over-privileged database users
- Ignoring legacy code paths

---

## Key Takeaways

- SQL injection targets application databases
- Unsafe query construction is the root cause
- Parameterization is the primary defense
- Secure design prevents entire classes of attacks
