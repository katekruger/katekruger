## Kate Kruger

B2B revenue operator turned GTM engineer. I build the tooling that revenue teams keep rebuilding badly.

Every project here shares one idea: **a GTM system should refuse to act on data it cannot verify.** Most of them cannot, which is why pipeline reports do not reconcile, why sending reputation collapses without warning, and why nobody notices until a board meeting.

### What I have shipped

| Project | What it does | Status |
|---|---|---|
| [pipeline-waterfall](https://github.com/katekruger/pipeline-waterfall) | dbt package for the bookings and pipeline waterfall. Fails the build rather than reporting a bridge that does not tie out. | `0.1.0` |
| [segment-mcp](https://github.com/katekruger/segment-mcp) | Read-first MCP server for Segment: which destinations get which events, which sources are dead, which are governed by nothing. Deletion is not exposed. | PyPI `0.1.1` |
| [deliverability-guard](https://github.com/katekruger/deliverability-guard) | Sending circuit breaker for outbound email. Throttles or pauses before a domain burns, and refuses to trip on one bad day at n=1. | PyPI `0.1.0` |
| [n8n-operator](https://github.com/katekruger/n8n-operator) | Governed MCP control plane for operating approved n8n workflows from Claude, OpenAI and Codex. Every run passes a human gate. | `v1.0.0-rc3` |
| [instantly-mcp](https://github.com/katekruger/instantly-mcp) | MCP server for the Instantly v2 API. Every write is gated behind an explicit confirm, with code-enforced autonomy tiers and volume caps. | live |
| [campaign-preflight](https://github.com/katekruger/campaign-preflight) | Read-only preflight for outbound campaigns: contacts, personalization, suppressions, schedules, sender readiness. CLI and MCP. | live |
| [agent-audit](https://github.com/katekruger/agent-audit) | A portable record binding what an agent proposed, what a human decided, what executed, and what it cost. An OpenTelemetry semantic convention plus a thin emitter. | in build |
| [awesome-gtm-engineering](https://github.com/katekruger/awesome-gtm-engineering) | Curated list of GTM engineering tools, with a written curation policy and a deterministic build. | live |

### How I build

- Architecture decisions are written down before the code, as ADRs in `docs/decisions/`
- `AGENTS.md` is the source of truth in every repo; `CLAUDE.md` is a one-line include
- Packages publish through PyPI Trusted Publishing with build attestations
- Tests assert the refusal, not just the happy path

### Elsewhere

[paigeconsultancy.com](https://paigeconsultancy.com) · [LinkedIn](https://www.linkedin.com/in/kathleenstumph)
