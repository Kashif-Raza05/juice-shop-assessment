# Web Application Security Assessment: OWASP Juice Shop

A penetration-test-style assessment of OWASP Juice Shop, a deliberately vulnerable web application, with findings, evidence, and fixes a developer could apply.

> Testing was done only on a local copy of Juice Shop running on my own machine. Do not run these techniques against systems you do not own or have written permission to test.

## Scope
- **Target:** OWASP Juice Shop `[version]` running locally at `http://localhost:3000`
- **Type:** Black-box web application test
- **Dates:** [from] to [to]
- **Tester:** Kashif Raza

## Tools used
- Docker (to run Juice Shop)
- Burp Suite Community Edition [and any others you actually used]
- Browser developer tools

## Setup
```bash
docker run -p 3000:3000 bkimminich/juice-shop
```

## Summary of findings

| # | Vulnerability | OWASP Top 10 category | Severity |
|---|---|---|---|
| 1 | [SQL injection on login] | A03: Injection | [High] |
| 2 | [Reflected/DOM XSS in search] | A03: Injection | [Medium] |
| 3 | [Broken access control, e.g., viewing another user's basket] | A01: Broken Access Control | [High] |
| 4 | [Your finding] | [ ] | [ ] |
| 5 | [Your finding] | [ ] | [ ] |

## Detailed findings

### Finding 1: [SQL Injection on Login]
- **Severity:** [High] and why: [short reasoning]
- **Location:** [URL / endpoint / parameter]
- **Steps to reproduce:**
  1. [Step]
  2. [Step]
  3. [Step]
- **Evidence:**

  ![Finding 1](screenshots/finding1.png)
- **Impact:** [What an attacker could do]
- **Recommended fix:** [e.g., use parameterized queries, validate input, return generic error messages]
- **Example of safer code:**

```javascript
// [short before/after snippet written by you]
```

### Finding 2: [Title]
[Copy the same structure as above]

### Finding 3: [Title]
[Copy the same structure as above]

## Overall recommendations
- [e.g., adopt secure coding practices and input validation across the app]
- [e.g., enforce access control checks on the server side]
- [e.g., add security testing to the development pipeline]

## What I learned
- [Honest points: how injection works, how Burp intercepts requests, thinking like both an attacker and a developer]

## References
- OWASP Top 10: https://owasp.org/www-project-top-ten/
- OWASP Juice Shop: https://owasp.org/www-project-juice-shop/

## Author
Kashif Raza | [LinkedIn link] | [email]
