---
title: "Aplazo's 'critical' Etherfuse-vs-Bando contradiction is already resolved — it reverts to Etherfuse"
type: synthesis
source: synthesis
source_date: 2026-07-14
source_trust: reported
confidence: high
neighborhood: "aplazo"
---

# Aplazo's 'critical' Etherfuse-vs-Bando contradiction is already resolved — it reverts to Etherfuse

> The Aplazo page flags the Etherfuse/Bando lead-ownership conflict as 'critical, needs immediate clarification,' but Bando's own handoff scope rules already answer it: Aplazo requires wallet embedding and stablecoin issuance, both explicitly excluded from Bando's treasury-hold-only resale scope.

The Aplazo wiki treats the lead-ownership conflict as an unresolved blocker — two sources disagree on whether Etherfuse retained the deal or handed it to Bando, and the page lists 'Is Etherfuse or Bando the actual lead?' as a **Critical** open question needing 'immediate clarification' [wiki/entities/companies/aplazo.md].

That question is already answered by the Bando handoff document's own rubric. Per the April 2026 reseller handoff, Bando's scope is strictly limited to treasury-hold (direct CETES buyer + thin Stablebonds UI); any prospect 'requiring API integration, wallet embedding, card issuance, or stablecoin issuance support' reverts to Etherfuse [wiki/entities/companies/Bando.md].

Aplazo's documented interest is precisely the excluded set: it is evaluating [[Privy]] embedded wallets for its merchant/consumer UX, wants stablecoin-powered checkout, and is exploring digital wallets across its 9,000+ merchant base [wiki/entities/companies/aplazo.md]. Those are wallet-embedding and stablecoin-issuance workstreams — categorically outside Bando's treasury-hold mandate.

**Decision:** Etherfuse retains Aplazo directly. This is not a judgment call requiring a BD escalation; it falls out of the handoff rules Etherfuse itself wrote. Resolving this unblocks a high-priority deal (BNPL float + checkout across 9,000 merchants, ~$100M revenue platform) that has been drifting in a Discovery/Proposal limbo since April largely because of the ownership ambiguity [wiki/entities/companies/aplazo.md].

**Watch-out:** Aplazo is also exposed to the IFL onboarding-friction problem that stalled Bando's other referred leads (MACA, Solutrust, etc.) [wiki/entities/companies/Bando.md]; the in-flight DocuSign migration should be sequenced ahead of Aplazo's onboarding to avoid the same drop-off.
