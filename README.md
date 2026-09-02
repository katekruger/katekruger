## Kate Kruger

B2B revenue operator & builder on the side. I've worked alongside highly technical teams, and automate my job with shippable software to keep up.  
Every project here shares one idea: **a GTM system should refuse to act on data it cannot verify.** Most of them cannot, which is why pipeline reports do not reconcile, why sending reputation collapses without warning, and why nobody notices until the CRM & data collapses pre board meeting.

### What I have shipped

| Project | What it does | Status |
|---|---|---|
| [segment-mcp](https://github.com/katekruger/segment-mcp) | Read-only MCP server for Segment. Which destinations get which events, which sources are dead. It cannot delete anything. | PyPI `0.1.3` |
| [deliverability-guard](https://github.com/katekruger/deliverability-guard) | Circuit breaker for outbound email. Pauses sending before a domain burns, and will not panic over one bad day. | PyPI `0.1.0` |
| [instantly-mcp](https://github.com/katekruger/instantly-mcp) | MCP server for the Instantly v2 API. Nothing sends without an explicit confirm. | PyPI `0.1.0` |
| [pipeline-waterfall](https://github.com/katekruger/pipeline-waterfall) | dbt package for the bookings and pipeline waterfall. Fails the build instead of shipping a bridge that does not tie out. | `0.1.0` |
| [n8n-operator](https://github.com/katekruger/n8n-operator) | Run approved n8n workflows from Claude, OpenAI or Codex. Every run passes a human gate. | `v1.0.0-rc3` |
| [campaign-preflight](https://github.com/katekruger/campaign-preflight) | Checks an outbound campaign before it sends: suppressions, merge fields, schedules, sender health. It cannot launch anything. | 76 checks, unreleased |
| [agent-audit](https://github.com/katekruger/agent-audit) | A record of what an agent proposed, what a human decided, and what actually ran. OpenTelemetry convention plus a small emitter. | in build |
| [awesome-gtm-engineering](https://github.com/katekruger/awesome-gtm-engineering) | A list of GTM engineering tools, with a curation policy and a build that checks the links. | live |

### How I build

- Architecture decisions are written down before the code, as ADRs in `docs/decisions/`
- `AGENTS.md` is the source of truth in every repo; `CLAUDE.md` is a one-line include
- Packages publish through PyPI Trusted Publishing with build attestations
- Tests assert the refusal, not just the happy path

### Elsewhere

[paigeconsultancy.com](https://paigeconsultancy.com) · [LinkedIn](https://www.linkedin.com/in/kathleenstumph)
