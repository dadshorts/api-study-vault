# Problems I Could Automate With APIs
Date: 2026-05-02 (during Phase 0 video — fCC APIs for Beginners)

Captured during the "I'm a few APIs away from solving real problems" moment.
Raw, unfiltered. Will triage later.

---

## 1. HOA treasurer job — QuickBooks reconciliation and management
*API angle: QuickBooks has a real public REST API (Intuit Developer Platform). Reconciliation is the classic "match transactions across two systems" automation — pull from bank, pull from QB, diff, flag mismatches. Solid Phase 1 target. Teaches auth (OAuth 2), pagination, idempotency.*

## 2. PNC banking — automated reporting and transactions
*API angle: Personal banking is harder — most US banks don't expose retail APIs directly. The bridge most fintech uses is **Plaid** (and a few alternatives: MX, Yodlee, Teller). You'd integrate Plaid's API, which gives you read access to PNC. Read-only is approachable; transactions are gated. Teaches: third-party API integration, bank-grade auth.*

## 3. TripAdvisor — find users who rate my favorite places the same way, then search their other favorites
*API angle: This is a **recommendation system via collaborative filtering** — "people who liked X also liked Y." TripAdvisor's public API doesn't expose user social graphs (data access is the limit, not your skill). Real path is either their Content API (B2B partnership) or alternatives like Yelp Fusion / Google Places. The pattern itself is gold — same algorithm Spotify, Netflix, Amazon use.*

## 4. Foodies for foodies
*API angle: This is the bigger product idea behind #3 — a social/recommendation app for food lovers. Start small: build a clone of #3's pattern using Yelp Fusion or Google Places API (both have generous free tiers and expose what you need). If it works for one user (you), you have an MVP. From there: add other users, then it's a real product.*

---

## Notes for Phase 1 portfolio API decision

- **#1 is the strongest first target** — real API, real problem, lots to learn, narrow scope.
- **#2 builds on #1** — once you've done bank-side reconciliation in QB, layering Plaid is a natural extension.
- **#3 + #4 are the "if I keep going" projects** — Phase 2/3 territory, or post-curriculum.

## What to learn that unlocks each

- All four require: REST fundamentals, auth (API keys → OAuth 2), JSON parsing, error handling.
- #1 specifically requires: webhook receivers (so QB notifies you of changes).
- #2 specifically requires: working with a third-party SDK (Plaid client library).
- #3/#4 require: at minimum, a database to store cached user data + a frontend (eventually).

Phase 1 of the curriculum gets you 80% of #1. Phase 2 lets you secure it. Phase 3 ships it.
