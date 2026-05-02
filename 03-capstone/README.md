# Phase 3 — Capstone

**Week 8 · ~10 hours**

## Goal
Polish both artifacts to portfolio quality. By end of week, your `api-study-vault` repo should be pinned on your GitHub profile and ready to show anyone — recruiter, peer, or future-you.

## Artifact 1 — Portfolio API (~4 hrs)

Polish the API you built in Phase 1, now with the security knowledge from Phase 2.

- [ ] README explains design choices, threat model, and what you'd do differently
- [ ] OpenAPI spec linked from README
- [ ] Postman collection committed to the repo
- [ ] **Security section** in README listing OWASP API Top 10 controls implemented:
  - Rate limiting
  - JWT validation (algorithm pinning, expiry, issuer/audience)
  - RBAC / authorization checks on every endpoint
  - Input validation
  - Proper error messages (no stack traces in prod)
  - HTTPS-only

## Artifact 2 — crAPI Pentest Report (~6 hrs)

A markdown report at `crapi-pentest-report.md` written like a deliverable to a real client.

Required sections:

1. **Executive Summary** (3-5 sentences) — what was tested, what was found, severity at-a-glance
2. **Methodology** — tools used: Burp Community, Postman, custom Node/Python scripts
3. **Findings** — one section per OWASP API Top 10 category found, each with:
   - Endpoint(s) affected
   - PoC request/response (sanitize sensitive values)
   - Severity rating with reasoning (CVSS-style if you want)
   - Remediation recommendation
4. **Appendix** — screenshots, HAR exports, full request/response logs

Tone: professional. Imagine handing this to a paying client.

## Final verification

- [ ] Both artifacts visible in `api-study-vault` GitHub repo
- [ ] Repo README links to: freeCodeCamp cert, deployed API URL, pentest report
- [ ] Repo pinned on your GitHub profile
- [ ] You can describe both artifacts in a 60-second elevator pitch

## What "done" looks like

A future hiring manager scans your GitHub. They see one pinned repo. They open the README. They see a deployed API they can hit, an OpenAPI spec they can read, a freeCodeCamp cert they can verify, and a pentest report that reads like a real consulting deliverable.

Most candidates have one of those. You'll have all four. That's the asymmetry this curriculum buys you.
