<div align="center">

# 🔐 Security Policy

**Multilingual AI Receptionist** handles real customer data, business operations, and communication workflows.
Security is not an afterthought — it is a core responsibility.

[![Security](https://img.shields.io/badge/Security-Responsible%20Disclosure-red?style=for-the-badge&logo=shield&logoColor=white)](https://github.com/nikhil-ai-insights/multilingual-ai-receptionist/security)
[![HTTPS](https://img.shields.io/badge/Communication-HTTPS%20Enforced-green?style=for-the-badge&logo=letsencrypt&logoColor=white)](https://github.com/nikhil-ai-insights)
[![Secrets](https://img.shields.io/badge/Secrets-Env%20Variables%20Only-blue?style=for-the-badge&logo=dotenv&logoColor=white)](https://github.com/nikhil-ai-insights)

</div>

---

## 🎯 Scope of This Policy

This project processes and stores sensitive data across multiple systems. The following areas are considered in-scope for security review:

| Area | Sensitive Assets |
|---|---|
| 👤 **Customer Data** | Contact info, appointment records, preferences |
| 📅 **Calendar Systems** | Business schedules, Google/Outlook integrations |
| 📞 **Voice Workflows** | Call transcripts, voice data, AI interactions |
| 🔑 **Authentication** | Login systems, session tokens, admin access |
| 📬 **Notifications** | SMS, Email, WhatsApp delivery pipelines |
| 🔗 **API Integrations** | Third-party credentials, OAuth tokens, webhooks |
| 🖥️ **Admin Dashboard** | Business data, analytics, user management |

---

## 🚨 Reporting a Vulnerability

> **Do not open a public GitHub Issue for security vulnerabilities.**
> Public disclosure before a fix is available puts real users and businesses at risk.

### How to Report

Contact the project maintainer **privately** through GitHub:

**👤 Maintainer:** [Nikhil AI Insights](https://github.com/nikhil-ai-insights)

### What to Include in Your Report

```
1. Clear description of the vulnerability
2. Affected component or module
3. Steps to reproduce the issue
4. Potential impact and severity assessment
5. Screenshots or logs (if relevant)
6. Suggested fix (optional but appreciated)
```

> 🔒 **Privacy note:** Use test data or masked examples only. Never include real customer information in your report.

---

## ⚡ Response Process

Once a valid report is received, we follow this process:

```
┌──────────────────────────────────────────────────────────────────┐
│                                                                  │
│  📨 STEP 1 — ACKNOWLEDGEMENT                                     │
│  Confirm receipt of the report                                   │
│                                                                  │
│  🔍 STEP 2 — INVESTIGATION                                       │
│  Reproduce, assess severity, and evaluate risk scope             │
│                                                                  │
│  🛠  STEP 3 — REMEDIATION                                        │
│  Develop patch, update dependencies, or redesign affected area   │
│                                                                  │
│  🚀 STEP 4 — RELEASE FIX                                        │
│  Security update published with release notes                    │
│                                                                  │
│  🏅 STEP 5 — CREDIT (Optional)                                   │
│  Responsible reporters acknowledged if they wish                 │
│                                                                  │
└──────────────────────────────────────────────────────────────────┘
```

---

## 🔐 Security Practices in This Project

### 🔑 Authentication & Access
- Secure login with session protection
- Token-based authentication
- Role-based admin access control
- Two-factor authentication recommended for admin accounts
- Session timeout enforcement

### 🛡️ Data Protection
- Encrypted storage for sensitive fields
- HTTPS enforced across all communication
- Minimal data exposure by design
- Controlled access permissions per role

### 🔒 Secrets Management
- All API keys and credentials stored in environment variables
- **Zero hardcoded secrets in source code**
- Separate credentials per environment (dev / staging / production)

### ✅ Input Validation
- User input validated on all endpoints
- Malformed requests rejected before processing
- Data sanitized before database writes

### 📦 Dependency Security
- Third-party libraries kept up to date
- Vulnerable packages audited and removed
- Regular dependency reviews

### 📊 Logging & Monitoring
- Error monitoring in production
- Admin activity logs
- Abuse detection systems

---

## 🧠 AI & Voice Security

This platform uses AI and voice systems that require additional safeguards:

| Control | Description |
|---|---|
| 🔐 Secure API usage | All AI API calls made over encrypted channels |
| 🧱 Prompt protection | Minimal prompt exposure to end users |
| 🎙️ Voice data | Not stored beyond session unless explicitly required |
| 🔗 Integrations | Permission-based, least-privilege access only |
| 📝 Transcripts | Controlled access, not publicly exposed |

---

## 📅 Calendar & Integration Security

Third-party integrations (Google Calendar, Outlook, SMS, Email) follow secure standards:

- ✅ OAuth 2.0 for calendar authorization
- ✅ Least-privilege permission scopes
- ✅ Regular token rotation
- ✅ Revoke unused or stale integrations
- ✅ Audit connected services periodically

---

## 🌍 Infrastructure Security

| Control | Standard |
|---|---|
| 🔒 HTTPS | Enforced on all endpoints |
| 🧱 Firewall | Configured to restrict unnecessary access |
| ⚙️ Rate Limiting | Applied to prevent abuse & brute force |
| 🛡️ DDoS Protection | Applied at infrastructure level |
| 💾 Backups | Regular automated database backups |
| 🔄 Patches | Server and OS updates applied regularly |

---

## 🐛 What to Report

**In-scope vulnerabilities include:**

- Authentication bypass or broken access control
- Privilege escalation
- SQL injection
- Cross-Site Scripting (XSS)
- Sensitive data leaks or exposed API keys
- Server-Side Request Forgery (SSRF)
- Remote Code Execution (RCE)
- Booking manipulation or account takeover
- Insecure direct object references

**Out of scope (unless they create demonstrated risk):**

- UI typos or cosmetic issues
- Rate limit observations without a working exploit path
- Theoretical issues with no realistic impact
- Spam reports unrelated to code security
- Bugs in old, unused third-party packages

---

## 🔄 Staying Up to Date

Security patches are released as needed and may include:

- Dependency upgrades
- Infrastructure hardening
- Authentication improvements
- Access control fixes
- Data handling updates

> **Always run the latest stable version** to ensure you have the most recent security fixes.

---

## 🤝 Responsible Disclosure Promise

We deeply respect ethical security researchers and contributors who help make this project safer. All good-faith reports are taken seriously, handled with care, and acknowledged appropriately.

Together, we protect the businesses and customers who rely on this platform.

---

<div align="center">

### 👨‍💻 Maintained by [Nikhil AI Insights](https://github.com/nikhil-ai-insights)

*Security is an ongoing process — not a one-time feature.*
*Thank you for helping us build something trustworthy.* 🔐🚀

</div>
