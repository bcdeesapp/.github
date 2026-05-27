# Security Policy

## Reporting a Vulnerability

**Please do not open a public GitHub issue for security vulnerabilities.**

BCDees handles real financial transactions and user identity data. We take security seriously and ask that you give us the opportunity to address issues responsibly before any public disclosure.

### How to Report

Email **security@bcdees.com** with:

1. A clear description of the vulnerability
2. Steps to reproduce or a proof-of-concept
3. The potential impact (what an attacker could achieve)
4. Your contact details for follow-up

We will acknowledge your report within **48 hours** and aim to provide a resolution timeline within **5 business days**.

### Scope

Areas of particular sensitivity in our platform:

- Escrow logic and fund release conditions
- Wallet balances and ledger integrity
- KYC / identity data exposure
- Authentication and session management
- Admin role escalation or bypass
- P2P trade flow manipulation

### Our Commitment

- We will not take legal action against good-faith security researchers.
- We will keep you informed of remediation progress.
- We will credit researchers who wish to be acknowledged (upon request).

## Supported Versions

| Version | Supported |
|---|---|
| Production (latest) | ✅ |
| Staging | ✅ (for testing only) |
| Older releases | ❌ |
