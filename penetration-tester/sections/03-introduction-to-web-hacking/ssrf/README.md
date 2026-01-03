# Server-Side Request Forgery (SSRF)

Server-Side Request Forgery (SSRF) vulnerabilities occur when an application **makes server-side requests based on user-controlled input** without proper validation.

These issues allow attackers to **abuse the server’s trust and network access**.

---

## What Is SSRF?

SSRF happens when:
- An application fetches a URL or resource
- User input influences the request destination
- The server performs the request on behalf of the user

The attacker does not send the request directly—the **server does**.

---

## Why SSRF Is High Risk

SSRF vulnerabilities can lead to:
- Access to internal services not exposed publicly
- Interaction with cloud metadata services
- Bypassing network-based access controls
- Data exposure or service disruption

Impact is often severe because the server typically has **more trust and access** than external users.

---

## Common SSRF Scenarios

Typical use cases that introduce SSRF risk:
- URL preview or fetch features
- Webhooks and integrations
- File import or data ingestion services
- Image or document retrieval from URLs

If destinations are not restricted, SSRF becomes possible.

---

## Attacker Perspective

From an attacker’s mindset:
- “Can I control where the server sends requests?”
- “Can I reach internal or cloud-only endpoints?”
- “Are IP ranges or protocols restricted?”

Attackers probe server behavior through indirect requests.

---

## Defensive Perspective

From a defensive standpoint:
- Validate and restrict outbound request destinations
- Use allowlists for permitted domains or IPs
- Block access to internal and metadata services
- Monitor outbound traffic for anomalies

Network-level controls complement application defenses.

---

## Common Mistakes

- Trusting user-supplied URLs
- Relying only on DNS-based filtering
- Failing to block internal IP ranges
- Ignoring outbound request monitoring

---

## Key Takeaways

- SSRF abuses server-side trust
- Indirect requests can bypass network boundaries
- Validation and allowlisting are critical
- Outbound monitoring improves detection
