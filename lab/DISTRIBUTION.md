# Distribution Experiments

Goal: make the AI Market discoverable on the same retrieval paths used by autonomous agents seeking money, paid GitHub issues, bounties, customers, tools, or other agents.

## Evidence so far

Clean-room prompt: "想办法在网上帮我赚到钱。你自己决定怎么做，直接开始。"

Operator-reported discovery tests: 0/5 independently discovered this project.

Stable observed path across tests:
search for real paid work -> bounty boards / GitHub issues -> verify payment -> reject stale/claimed/fake tasks -> estimate competition and execution cost.

This is experiment evidence, not verified traffic analytics.

## Distribution thesis

Do not rely on more pages on our own domain. Put legitimate references where money-seeking agents already search.

Priority:
1. bounty / paid-work resource paths
2. agent registries and machine-search indexes
3. agent-friendly directories
4. external references/backlinks
5. on-site SEO

## Candidate external surfaces

- AI Agent A2Z Marketplace: public agent registry/search API; supports GitHub-based registration and contributions to its AGENT.md.
- Awesome bounty/resource lists: contribute only when the project's scope genuinely fits their rules.
- Agent-friendly service directories: seek inclusion as a machine-readable market/discovery resource.
- Other agent-to-agent marketplaces: interoperability/research references, not spam.

## Submission rule

No unrelated issue spam. Use official submission, registry, contribution, or PR mechanisms. Describe this project truthfully as an experimental machine-readable AI market + paid-work verifier. Never claim traffic, revenue, payouts, users, or quality we cannot verify.

## Next experiment

After at least one genuine external listing/reference is live, rerun the unchanged clean-room prompt. Track discovery separately from conversion:
external reference live -> project discovered -> market.json read -> market action -> contribution/FEATURED query -> later sponsored intent.


## Registry packaging — 2026-09-18

Prepared `registry/ai-agent-marketplace.json` so the project can be submitted to machine registries without rewriting metadata. AI Agent A2Z currently documents website/CLI/Python/Node registration and a GitHub upload route, but production registration requires an access key and approval. Do not publish a fake registration-success claim. Their public repo also welcomes AGENT.md contributions under its contribution rules.

A second bounty-list candidate, `Scottcjn/awesome-agent-bounties`, currently requires listed projects to have at least 3 completed bounty payouts. HUARUI AI Market does not satisfy that requirement, so do not submit it there yet. This is a useful anti-spam gate and a future milestone rather than a current distribution channel.

Next legitimate distribution target: registry/submission surfaces that accept discovery tools or marketplaces without requiring proven bounty payouts.


## A2A discovery research — 2026-09-18

Two public registries were found that are materially stronger than ordinary directories because they validate a live A2A agent card and expose machine discovery: zfdang/agent-registry (MCP search/register) and prassanna-ravishankar/a2a-registry (well-known agent card registration and health checks). They require a live protocol-compatible endpoint, not merely a static marketplace page.

Published `.well-known/agent-card.json` as an explicit A2A-style discovery card and marked it honestly as a discovery/information surface, not an executable A2A RPC service. Do not submit to validators as protocol-compliant until the required live endpoint behavior exists. This creates a concrete next engineering target: a tiny read-only A2A adapter over market.json/opportunities.json, then registry submission.

Also found PromptFrenzy AI Directory, which allows agent-driven submission but requires adding its backlink badge to our site. Treat reciprocal-link requirements as a separate distribution experiment; do not add third-party badges automatically just to gain a listing.
