# API Infrastructure Lesson Plan — 8 Weeks, JS-First, Build→Break

## Context

Jon is moving into infrastructure with **APIs as the entry vector**, building on his existing JS/Python/JSON learning track. The goal is end-to-end fluency: understand the protocol landscape, build a real API in JavaScript, then attack it like a security engineer would.

This plan is calibrated to:
- **80 hours over 8 weeks** (~10 hrs/week)
- **JavaScript / Node + Express** as the build language
- **10/45/45 weighting** — light orientation, deep build, deep break
- **Two deliverable artifacts**: a deployed portfolio API + a pentest report on OWASP crAPI mapped to the API Security Top 10

The plan uses **only convergent sources** — resources that two or more of the research agents independently surfaced — so every hour spent is on a vetted on-ramp.

---

## Prerequisites & Setup (Week 0 — half a day)

Install before Week 1:
- Node.js LTS + npm
- Postman desktop app (free tier)
- Git + a GitHub account
- Docker Desktop for Windows (needed for crAPI in Phase 2)
- VS Code with REST Client extension
- Burp Suite Community Edition (free; needed for Phase 2)

Create a single GitHub repo: `api-study-vault`. Every project, exercise, and writeup goes here. Treat it as your portfolio from day one.

---

## Phase 0 — Types Orientation (Week 1, ~8 hrs, 10%)

**Goal:** Build a mental map of the API landscape before specializing in REST.

| Time | Source | Deliverable |
|---|---|---|
| 1 hr | [Roadmap.sh — API Design](https://roadmap.sh/api-design) | Screenshot the roadmap, mark what you already know |
| 3 hrs | [fCC — APIs for Beginners (Craig Dennis)](https://www.youtube.com/watch?v=WXsD0ZgxjRw) | Notes file `phase-0/apis-101.md` with your own metaphors |
| 4 hrs | [Postman Learning Center — Galaxy: API Fundamentals + APIs 101](https://learning.postman.com/) | Earn at least one Postman badge; export collections to `phase-0/postman/` |

**Milestone:** Write a one-page README in your repo explaining REST, GraphQL, gRPC, WebSocket, SOAP, and webhooks in *your own words* — using metaphors. If you can teach it, you understand it.

---

## Phase 1 — Build (Weeks 2-4, ~36 hrs, 45%)

**Goal:** Ship a deployed Express REST API with auth, persistence, and an OpenAPI spec.

### Week 2 — Foundations (~12 hrs)
- [microsoft/Web-Dev-For-Beginners](https://github.com/microsoft/Web-Dev-For-Beginners) — Node/Express lessons (~6 hrs)
- [MDN — Express/Node Server-Side Tutorial](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs) — read through "Routes and controllers" (~6 hrs)

### Week 3 — freeCodeCamp Back-End Cert: Projects 1-3 (~12 hrs)
[freeCodeCamp — Back-End Development and APIs Certification](https://www.freecodecamp.org/learn/back-end-development-and-apis/)
- Timestamp Microservice
- Header Parser Microservice
- URL Shortener Microservice

### Week 4 — freeCodeCamp Cert: Projects 4-5 + Portfolio API (~12 hrs)
- Exercise Tracker
- File Metadata Microservice
- **Earn the freeCodeCamp Back-End certificate**
- Start your **portfolio API**: a "BookShelf" or similar CRUD service with users, JWT auth, and Postgres or MongoDB. Commit it to your repo.

**Phase 1 verification:**
- [ ] freeCodeCamp Back-End cert URL pasted into your repo README
- [ ] Portfolio API deployed (Render, Railway, or Fly.io free tier)
- [ ] OpenAPI 3 spec at `/openapi.json`
- [ ] `npm test` passes with at least 5 integration tests
- [ ] Self-graded against [shieldfy/API-Security-Checklist](https://github.com/shieldfy/API-Security-Checklist) — record score in `phase-1/security-self-grade.md`

---

## Phase 2 — Break (Weeks 5-7, ~36 hrs, 45%)

**Goal:** Develop offensive API thinking. Attack OWASP crAPI under structured guidance, then test your own portfolio API.

### Week 5 — Theory + First Attacks (~12 hrs)
- 2 hrs: Read [OWASP API Security Top 10 (2023)](https://owasp.org/API-Security/) cover to cover. Take notes on each category.
- 2 hrs: Deploy [OWASP crAPI](https://github.com/OWASP/crAPI) locally via Docker Compose. Verify all services up.
- 8 hrs: [APISec University — API Penetration Testing (Corey Ball)](https://www.apisecuniversity.com/) — modules 1-4, labs against crAPI

### Week 6 — Hands-On Exploitation (~12 hrs)
- 6 hrs: APISec University — finish remaining modules (BOLA/BFLA, mass assignment, SSRF, JWT)
- 6 hrs: [PortSwigger Web Security Academy](https://portswigger.net/web-security) — **API testing learning path** (Apprentice + Practitioner labs)

### Week 7 — Specialty Attacks + Self-Assessment (~12 hrs)
- 4 hrs: PortSwigger labs — JWT attacks
- 4 hrs: PortSwigger labs — GraphQL API vulnerabilities
- 4 hrs: **Turn your tools on your own portfolio API.** Find at least three real vulnerabilities and patch them. Document each find/fix in `phase-2/self-pentest.md`.

**Phase 2 verification:**
- [ ] Notes file with all 10 OWASP API Top 10 categories defined in your own words
- [ ] crAPI exploited end-to-end with PoCs saved as screenshots/HAR files
- [ ] PortSwigger API testing path showing "Solved" labs (screenshot the dashboard)
- [ ] At least 3 vulnerabilities found and patched in your own portfolio API

---

## Phase 3 — Capstone (Week 8, ~10 hrs)

**Goal:** Polish both artifacts to portfolio quality.

### Artifact 1: Portfolio API (~4 hrs)
- README explaining design choices, threat model, and what you'd do differently
- OpenAPI spec linked in README
- Postman collection committed to repo
- "Security" section in README listing the OWASP API Top 10 controls you implemented (rate limiting, JWT validation, RBAC, input validation, etc.)

### Artifact 2: crAPI Pentest Report (~6 hrs)
A markdown report at `phase-3/crapi-pentest-report.md` containing:
- Executive summary (3-5 sentences)
- Methodology (tools used: Burp Community, Postman, custom scripts)
- One section per OWASP API Top 10 category found, each with:
  - Endpoint(s) affected
  - PoC request/response (sanitized)
  - Severity rating with reasoning
  - Remediation recommendation
- Appendix: screenshots
- Tone: professional, as if delivered to a real client

**Final verification:**
- [ ] Both artifacts visible in `api-study-vault` GitHub repo
- [ ] Repo README links to: freeCodeCamp cert, deployed API URL, pentest report PDF
- [ ] Repo pinned on your GitHub profile

---

## Source Index (only what's used)

### Types
- [Roadmap.sh API Design](https://roadmap.sh/api-design)
- [fCC YouTube — APIs for Beginners (Craig Dennis)](https://www.youtube.com/watch?v=WXsD0ZgxjRw)
- [Postman Learning Center](https://learning.postman.com/)

### Build
- [microsoft/Web-Dev-For-Beginners](https://github.com/microsoft/Web-Dev-For-Beginners)
- [MDN Express/Node Server-Side](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs)
- [freeCodeCamp Back-End & APIs Cert](https://www.freecodecamp.org/learn/back-end-development-and-apis/)
- [shieldfy/API-Security-Checklist](https://github.com/shieldfy/API-Security-Checklist)

### Break
- [OWASP API Security Top 10 (2023)](https://owasp.org/API-Security/)
- [OWASP crAPI](https://github.com/OWASP/crAPI)
- [APISec University](https://www.apisecuniversity.com/)
- [PortSwigger Web Security Academy](https://portswigger.net/web-security)

### Optional supplements (skip unless ahead of schedule)
- [InsiderPhD YouTube](https://www.youtube.com/@InsiderPhD) — bug bounty thinking
- [HackerOne Hacktivity](https://hackerone.com/hacktivity) — real exploit writeups
- [erev0s/VAmPI](https://github.com/erev0s/VAmPI) — gentler alternative to crAPI if Docker is painful

---

## How to recover if a week slips

- **Falling behind in Phase 1?** Drop fCC projects 4-5; the cert is a bonus, not a requirement. Keep the portfolio API.
- **Falling behind in Phase 2?** Drop PortSwigger GraphQL labs. APISec U + crAPI is the irreducible core.
- **Falling behind in Phase 3?** Ship the pentest report at minimum. The portfolio API is already deployed; polish can come later.

The two artifacts are the load-bearing deliverables. Everything else is scaffolding.
