# AWS Security Specialty (SCS-C03) Interactive Study Guide

A fully interactive, self-contained study app built for the **AWS Certified Security – Specialty (SCS-C03)** exam. No frameworks, no dependencies, no internet required — just one HTML file that runs on any device.

Built as part of my journey toward AWS Security certification while developing hands-on knowledge of cloud security architecture, IAM, threat detection, and data protection.

---

## Live Demo

**[▶ Open the live app →](https://brandobank.github.io/aws-security-study-guide/)**

*(GitHub Pages — loads directly in your browser, no download needed)*


Download [`AWS_SCS-C03_Study_Guide.html`](./AWS_SCS-C03_Study_Guide.html), open it in any browser, and it works — fully offline.

---

## Features

### Study Tools
- **Full Exam Guide** — All 6 SCS-C03 domains with collapsible sections, searchable content, tables, and callouts
- **Flashcards** — Spaced repetition system (Again / Hard / Good / Easy rating), filterable by domain, progress tracked in localStorage
- **8-Week Progress Tracker** — Daily study checklist with completion percentage and streak tracking
- **Exam Timer** — 170-minute countdown (real exam duration) with warning states and a practice score log
- **Cheat Sheet** — Quick-reference card for the most-tested services and distinctions

### Study Games
| Game | Description |
|------|-------------|
| ⚡ Security Blitz | Fast-paced multiple choice — 3 lives, streak multiplier, speed bonus points |
| ⚖️ Policy Judge | Read an IAM scenario, rule ALLOW or DENY — trains policy evaluation instinct |
| 🔰 Service Showdown | "Which AWS service handles X?" — the most common exam question type |
| 🌌 Jedi Force Trial | 25 Star Wars-lore security questions + Force Power hint system (eliminates 2 wrong answers) |

### Exam Coverage
All 6 SCS-C03 domains covered with weighted focus matching the real exam:

| Domain | Weight |
|--------|--------|
| Identity & Access Management | 20% |
| Infrastructure Security | 18% |
| Data Protection | 18% |
| Detection | 16% |
| Security Foundations & Governance | 14% |
| Incident Response | 14% |

---

## Technical Implementation

Built entirely in **vanilla HTML/CSS/JavaScript** — no build tools, no npm, no dependencies.

- **Canvas API** — Animated starfield background (280 twinkling stars, requestAnimationFrame loop)
- **CSS 3D transforms** — Flashcard flip animation with `transform-style: preserve-3d`
- **localStorage** — Persists all progress, flashcard ratings, hi-scores, and score history across sessions
- **CSS custom properties** — Full theme system (Space dark mode / Tatooine light mode) via a single class toggle
- **Spaced repetition logic** — Cards rated Again/Hard are requeued; Easy cards are deprioritized
- **Game engine** — Shared engine handles 4 distinct game modes with per-mode question banks, scoring, and hi-score tracking

---

## AWS Security Concepts Covered

A sample of what's inside:

- IAM policy evaluation logic (explicit deny, permission boundaries, SCPs, ABAC)
- VPC security (security groups, NACLs, Gateway vs Interface endpoints, Network Firewall)
- KMS key management (CMKs, data key caching, S3 Bucket Keys, `kms:ViaService`)
- GuardDuty → EventBridge → Lambda automated remediation patterns
- CloudTrail configuration (multi-region, log file validation, Insights, Lake)
- Incident response (EC2 isolation, EBS forensic snapshots, IAM session revocation)
- AWS Organizations + Control Tower (SCPs, preventive vs detective guardrails)
- Secrets Manager rotation, Macie data discovery, WAF rule groups, Shield Advanced

---

## About This Project

This started as a personal study tool and grew into a full ADHD-friendly interactive textbook. The goal was to make AWS security concepts actually stick — through active recall, gamification, and spaced repetition — rather than passive reading.

I'm currently pursuing the AWS Security Specialty certification as part of building a career in cloud security and cybersecurity. This repo is part of my portfolio demonstrating both security domain knowledge and practical development skills.

---

## What's Next

- [ ] SAA-C03 (Solutions Architect Associate) version
- [ ] Additional practice question banks
- [ ] GitHub Pages deployment for browser access without downloading

---

## License

MIT — fork it, study with it, build on it.
