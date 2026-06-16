---
title: "Shared Kappa Markets MM is the zero-onboarding unlock for EURAU↔Stablebond FX pools"
type: synthesis
source: synthesis
source_date: 2026-06-16
source_trust: reported
confidence: high
neighborhood: "all-unity"
---

# Shared Kappa Markets MM is the zero-onboarding unlock for EURAU↔Stablebond FX pools

> All Unity and Etherfuse already use the same market maker (Kappa Markets), so the on-chain EUR↔Stablebond FX marketplace Manuel explicitly asked for can be stood up with no new liquidity-provider onboarding — the fastest path to a live cross-currency FX product anchored on EURAU.

All Unity's market maker is **Kappa Markets — the same MM Etherfuse uses for its Mexican assets** [wiki/entities/companies/all-unity.md]. On the January discovery call, Manuel Becker flagged interest in "FX pools: EURAU-Stablebonds for on-chain FX market" [wiki/entities/companies/all-unity.md]. These two facts together are a concrete operational shortcut that no page connects: because both sides already clear liquidity through Kappa, an EURAU↔CETES / EURAU↔GILTS / EURAU↔EUROB pool can be quoted by an MM that is already integrated with both issuers, against Etherfuse's documented market-making target spread of 5–10 bps (max 25 bps) [wiki/markets/mexico-cetes.md → shared/products/market-making.md].

This turns a 'Discovery / awaiting regulatory alignment' relationship into a near-term shippable product that doesn't depend on All Unity's BaFin MXN approval (~3 months per currency) [wiki/entities/companies/all-unity.md]. EURAU becomes the EUR leg of an FX marketplace spanning the entire Stablebond roster — the same marketplace logic separately identified for AUSD as the USD leg, but here with the MM coordination already in place rather than to be built.

**Action:** ask Kappa to seed an EURAU/EUROB and EURAU/CETES pool as a pilot; this is the lowest-friction deliverable in the All Unity relationship and de-risks the larger MXN-stablecoin discussion by proving the rails first.
