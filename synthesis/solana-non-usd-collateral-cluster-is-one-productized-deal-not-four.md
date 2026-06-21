---
title: "The Solana non-USD DeFi collateral cluster is one product Etherfuse keeps re-negotiating from scratch"
type: synthesis
source: synthesis
source_date: 2026-06-21
source_trust: reported
confidence: high
neighborhood: "0xyz-p0"
---

# The Solana non-USD DeFi collateral cluster is one product Etherfuse keeps re-negotiating from scratch

> At least four Solana protocols — P0, Assetto, Rheo, and Hibachi — are independently asking for the identical thing (Stablebonds as yield-bearing DeFi collateral/listing), two of them quoting the exact same 25bps→1.5% fee schedule and the same closed-hours over-collateralization buffer, yet each is being hand-negotiated as a bespoke deal rather than served by one packaged product and one grant-seeded liquidity pool.

Four separate Solana-native DeFi venues in this neighborhood want the same integration:

- **P0 (0.xyz)** — portfolio-margin protocol, wants all six Stablebonds listed as collateral and is expanding to EM/forex collateral [teams/sales/2026-03-26-0xyz-p0.md].
- **Assetto (Precept Labs)** — non-USD stablecoin liquidity hub on Solana, already marked **Won**, with a fee schedule of **25bps/yr if bond yield <4.5%, up to 1.5%/yr if yield >10%**, and a **7% closed-hours over-collateralization buffer (~100–150K for CETES)** [teams/sales/2026-04-16-assetto-precept-labs.md].
- **Rheo** — fixed-rate lending protocol, using Stablebonds as looping collateral, quoting the **identical** fee tier: **25 bps below 4.5%, graduating to 1.5% above 10%** [teams/cfo/2026-04-21-rheo-partnership-structure.md].
- **Hibachi.xyz** — on-chain exchange that flagged CETES as a listing/liquidity addition at CDMX Stablecoin Week, June 2026 [teams/ceo/docs/inbox/linear/2026-06-18-sales-512-hibachi-xyz.md].

The repeated 25bps→1.5% fee schedule across Assetto and Rheo, and the repeated closed-hours-buffer requirement across Assetto and P0 (whose only blocker is exactly the closed-hours oracle price-gap problem), show Etherfuse has **already converged on a standard Stablebond-as-DeFi-collateral product** — it just hasn't named or packaged it. The decision-useful move: ship one fee sheet + the in-flight backend liquidity stablecoin (the structural fix for the buffer problem) + one foundation-grant-seeded liquidity pool that serves all four at once, rather than re-deriving terms and re-seeding liquidity deal by deal. The same Solana Foundation grant rails already cited for P0 ($70K) and Assetto ($50–100K omnibus) make a single shared seeding effort near-zero marginal cost [teams/sales/2026-03-26-0xyz-p0.md, teams/sales/2026-04-16-assetto-precept-labs.md].
