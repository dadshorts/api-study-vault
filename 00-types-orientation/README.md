# Phase 0 — Types Orientation

**Week 1 · ~8 hours · 10% of total curriculum**

## Goal
Build a mental map of the API landscape before specializing in REST. By end of week you should be able to explain — in your own metaphors — what REST, GraphQL, gRPC, WebSocket, SOAP, and webhooks each are, and when you'd reach for which.

## Sources

| Time | Source | Format |
|---|---|---|
| 1 hr | [Roadmap.sh — API Design](https://roadmap.sh/api-design) | Visual roadmap |
| 3 hrs | [fCC YouTube — APIs for Beginners (Craig Dennis)](https://www.youtube.com/watch?v=WXsD0ZgxjRw) | 3-hour video, ELI5 metaphor-driven |
| 4 hrs | [Postman Learning Center — Galaxy: API Fundamentals + APIs 101](https://learning.postman.com/) | Hands-on in Postman client |

## Deliverables (commit to this folder)

- [ ] `apis-101.md` — your notes from Craig Dennis video. Use your own metaphors. ELI5-first.
- [ ] `roadmap-screenshot.png` — annotated screenshot of the Roadmap.sh API Design map; mark what you already know vs. need to learn
- [ ] `postman/` — exported Postman collections from the Galaxy course
- [ ] `api-types-glossary.md` — your one-page README explaining all 6 API types in your own words. **This is the milestone.**

## Why this phase exists

Most courses jump straight to "build a REST API" and never explain why REST won, what GraphQL solves that REST doesn't, when gRPC is appropriate, etc. Skipping types orientation means you'll build REST without knowing what REST *is* in contrast to its alternatives. That's how you become a developer who only knows one tool.

## Done when

You can answer this question without looking anything up: "I have a mobile app that needs to receive real-time stock price updates from a server, then occasionally call admin functions on a third-party SOAP service. What API technologies would you use for each leg, and why?"

If you can answer that confidently, you've internalized this phase.
