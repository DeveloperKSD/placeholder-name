# Security Policy

## Reporting a Vulnerability

Please do not publicly disclose security vulnerabilities before they have been investigated.

Report vulnerabilities through the repository's private security reporting mechanism where available.

---

# Source Code Privacy

CodeSentinel is designed as a local-first application.

The project aims to process source code locally whenever possible.

Users should verify their configured AI provider before enabling any cloud-based model.

---

# AI-Generated Changes

AI-generated code should be reviewed by the user before being applied.

CodeSentinel should not silently modify source code.

---

# Secrets

Never commit:

- API keys
- Passwords
- Tokens
- Private keys
- `.env` files
- Credentials

Use environment variables or secure local configuration.

---

# Dependency Security

Dependencies should be kept reasonably up to date.

Security vulnerabilities in dependencies should be investigated and patched promptly.
