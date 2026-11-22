# Open Agentic Web implementation and entrant review plan

Prepared November 22, 2026, with AI assistance. This is a design aid, not a conforming network or a completed submission.

## Specification baseline

Working reference: MVP Profile 0.3 (18 November 2026), pinned document revision:
https://github.com/cognizant-ai-labs/agentic-web/blob/a0ceda34e4f2e653223e13e63282abc9b60eaf7c/docs/worldwide_agentic_web_mvp_spec.md

Recheck the current contest specification before implementation and submission. Official rules: https://cognizant-agenticweb.devpost.com/rules

## Candidate flow for entrant to refine

A fictional visitor chooses a synthetic community resource need and controls which fields can be shared. Three proposed responsibilities: a front-facing coordinator, a consent-policy checker, and a resource finder. The coordinator requests a permitted category, the checker returns allowed fields, and the finder chooses among synthetic resources only. No real referral, sensitive information, external action or credential collection.

The entrant should choose the target audience, define the synthetic categories, design the consent transition table, implement a substantive piece of the solution, test it, and document their contribution. Suggestions from this planning document are not a record of work done by the entrant.

## Acceptance matrix

| Requirement | Planned artifact | Evidence required |
|---|---|---|
| Discoverable site | agent-manifest.json | Public GET, valid network reference, configured router metadata and peer policy |
| Declarative multi-agent network | Resolved Neuro SAN network JSON | Schema validation and browser runtime loading the network from its manifest |
| Named peer bindings | links.json | Public GET; peer reference resolution where applicable |
| Browser runtime | Accessible site with actual runtime integration | Demonstrate a permitted synthetic request end to end; no invented inference or hardcoded pretend agent response |
| Consent | Scoped field authorization and revocation | User-visible consent before sharing; unknown scope denied; revocation blocks later forwarding |
| Interoperability | Public HTTPS and CORS | Test manifest and network retrieval from a separate permitted origin |
| Privacy | Synthetic records only | No credentials embedded in client code; no real personal data |
| Submission | Public site, description, recorded demo | Entrant's actual project ownership and contribution; working demo under two minutes |

## Entrant design worksheet

Complete these choices before claiming the idea or implementation ready:
1. Which fictional community resource categories will you include, and why?
2. Which fields are necessary for routing, and which must never leave the originating site?
3. What should happen if consent is revoked midway through a workflow?
4. Which component will you personally implement and test?
5. What new capability does the agent network provide over a normal search form?

Do not put real personal details or API keys in the answers. Record design decisions and commits honestly; preserve third-party notices and disclose AI assistance.

## Current boundary

Only architecture and acceptance planning exist. Runtime, manifest, JSON network, public hosting, CORS, real inference, conformance and submission remain unverified. The contest requires original entrant work and ownership. Assistance does not substitute for that contribution.
