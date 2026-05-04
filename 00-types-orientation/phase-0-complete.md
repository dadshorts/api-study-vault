# Phase 0 — Complete ✅

Date: 2026-05-02
Total session time: ~6 hrs across two consecutive evenings

## What I learned

### HTTP foundation
- API = a conversation between client and server
- 5 HTTP methods: GET (read), POST (create), PUT (replace all), PATCH (replace parts), DELETE
- Status code mnemonic: 2 = good, 4 = my fault, 5 = their fault
- Path parameters, query parameters, headers, body — all "parameters" in different slots

### 6 API types — in my own metaphors
- **REST** — text messages, get the whole menu sent back
- **GraphQL** — text message asking for specific pieces (specialty pizzas for vegetarians)
- **gRPC** — binary code, computer-to-computer, lightning fast
- **WebSocket** — phone call, server can push unprompted (online video games)
- **SOAP** — old, structured, legacy enterprise (run)
- **Webhooks** — the nightwatchman who calls *you* when something happens (vs polling = calling every 5m)

### The 4 pillars realization
APIs aren't a technique — they're leverage. Every product I'll ever build uses:
1. **Data sources** (APIs)
2. **Logic layer** (Claude as coding partner)
3. **Storage** (GitHub, databases, cloud)
4. **Surfaces** (UI for humans, MCP for agents)

### Postman crash course — 5 chunks
1. **5 surfaces** — Method+URL, Params, Headers, Body, Response
2. **Collections** — folders for related requests ("my preciousess")
3. **Variables & environments** — placeholders for values that change ("the rules of reality" for dev/staging/prod)
4. **Auth (4 flavors)** — API Key, Bearer Token, Basic Auth, OAuth 2 — all built via the Authorization tab
5. **Tests & scripts** — JS that runs after the response, can save data to environment for the next request (the chained-request pattern, foundation for SSO/auth-token flows)

### SSO clicked
Single Sign-On = log in once, every app in the same ecosystem trusts the token. Stark identity server → Jarvis + September Foundation all accept the same auth.

## Setup completed (Week 0)
- ✅ All 9 dev tools installed (Node 22, npm, Git, VS Code, gh CLI, Postman, Burp Community, REST Client, Docker 29.4.1)
- ✅ PowerShell 5.1 → 7.6.1
- ✅ 4 accounts created (freeCodeCamp, Postman, APISec U, PortSwigger)
- ✅ GitHub repo `dadshorts/api-study-vault` live
- ✅ All 3 sanity checks passed

## Real-world projects to build (captured during the video)
1. HOA treasurer / QuickBooks reconciliation — Phase 1 portfolio target
2. PNC banking automation via Plaid
3. TripAdvisor / "foodies for foodies" — collaborative filtering
4. Plus whatever else comes up

## Lessons learned the hard way
- **PowerShell 5.1 doesn't support `&&`** — use PowerShell 7 (already upgraded)
- **The right altitude for `baseUrl`** is just the origin — don't bake paths into it
- **Stale Postman lockfiles** can hang the app silently — kill processes + delete `settings.json.lock` + `.STALE`
- **"Lint yourself before send"** — before any non-GET request, check method, URL (hover variables), environment dropdown, body. Tonight saved a 404; in production saves you from `DELETE /users/`.

## Phase 0 milestone — DONE
- `api-types-glossary.md` ✅
- `roadmap-survey.md` ✅
- `problems-i-could-automate.md` ✅
- `phase-0-complete.md` ✅ (this file)

## Next session — Phase 1 Week 2 starts here
- microsoft/Web-Dev-For-Beginners — Node/Express lessons
- MDN Express tutorial
- First real `npm init`, first Express server, first route handler I wrote myself

The crash course tonight was the bridge from "I'm reading about APIs" to "I'm using a tool that works with APIs." Phase 1 is the bridge from "I'm using a tool" to "I built the tool."
