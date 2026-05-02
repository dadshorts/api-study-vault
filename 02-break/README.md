# Phase 2 — Break

**Weeks 5-7 · ~36 hours · 45% of total curriculum**

## Goal
Develop offensive API thinking. Attack OWASP crAPI under structured guidance, then turn the same tools on your own portfolio API and find real vulnerabilities.

## Weekly breakdown

### Week 5 — Theory + First Attacks (~12 hrs)
- 2 hrs: Read [OWASP API Security Top 10 (2023)](https://owasp.org/API-Security/) cover to cover
- 2 hrs: Deploy [OWASP crAPI](https://github.com/OWASP/crAPI) locally via Docker Compose. Verify all services up.
- 8 hrs: [APISec University — API Penetration Testing (Corey Ball)](https://www.apisecuniversity.com/) — modules 1-4, labs against crAPI

### Week 6 — Hands-On Exploitation (~12 hrs)
- 6 hrs: APISec University — finish remaining modules (BOLA/BFLA, mass assignment, SSRF, JWT)
- 6 hrs: [PortSwigger Web Security Academy](https://portswigger.net/web-security) — **API testing learning path** (Apprentice + Practitioner labs)

### Week 7 — Specialty Attacks + Self-Assessment (~12 hrs)
- 4 hrs: PortSwigger labs — **JWT attacks**
- 4 hrs: PortSwigger labs — **GraphQL API vulnerabilities**
- 4 hrs: **Turn your tools on your own portfolio API.** Find at least 3 real vulnerabilities and patch them.

## Deliverables (commit to this folder)

- [ ] `owasp-top10-notes.md` — all 10 categories defined in your own words with example endpoints
- [ ] `crapi-poCs/` — screenshots/HAR files showing crAPI exploited end-to-end
- [ ] `portswigger-progress.png` — dashboard screenshot showing solved labs
- [ ] `self-pentest.md` — vulnerabilities you found in your **own** portfolio API, with finds + fixes

## Verification

- [ ] All 10 OWASP API Top 10 categories defined in your own words
- [ ] crAPI exploited end-to-end with PoCs saved
- [ ] PortSwigger API testing path showing solved labs
- [ ] At least 3 vulns found and patched in your own portfolio API

## Why this phase is the differentiator

Almost everyone in your peer group can build a CRUD API by the end of Phase 1. Almost no one can attack one. This phase is the one that compounds — every API you ever build later will be more secure because you spent 36 hours thinking like an attacker.

The week 7 self-pentest is the moment of truth. Finding real bugs in your own code (and patching them) is where you stop being a builder who knows about security and become a builder who *practices* security.
