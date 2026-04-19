# Security Policy

## Supported Versions

This is a single-file static study app with no backend, no user accounts, and no server-side components. All data is stored locally in your browser's `localStorage`.

| Component | Status |
|-----------|--------|
| `AWS_SCS-C03_Study_Guide.html` | ✅ Actively maintained |

## Scope

Because this app runs entirely in the browser with no external API calls and no user data leaving the device, the attack surface is limited to:

- **Client-side JavaScript** — logic bugs, XSS via DOM manipulation
- **localStorage** — data stored in the browser (progress, scores, flashcard ratings)
- **Supply chain** — no external dependencies are loaded at runtime; the file is fully self-contained

Out of scope: server infrastructure, CI/CD pipelines, third-party services (there are none).

## Reporting a Vulnerability

If you find a security issue — XSS, unintended data exposure, or anything that could affect a user who opens this file — please report it responsibly before disclosing publicly.

**Report via GitHub:** Open a [GitHub Security Advisory](../../security/advisories/new) on this repository (private by default — only you and the maintainer can see it until disclosed).

Include:
- A description of the vulnerability and potential impact
- Steps to reproduce
- The browser and OS you tested on
- Any suggested fix, if you have one

I'll respond within **5 business days** and aim to push a fix within **14 days** for any confirmed issue.

## What We Ask

- Give reasonable time to fix before public disclosure
- Don't access or modify other users' data (there are no other users — it's a local app)
- Don't use findings to disrupt availability

Thank you for helping keep this project secure.
