---
title: "Etherfuse can unblock Assetto's stalled launch from stacked ecosystem grants instead of waiting on its capital raise"
type: synthesis
source: synthesis
source_date: 2026-07-19
source_trust: reported
confidence: medium
neighborhood: "assetto-precept-labs"
---

# Etherfuse can unblock Assetto's stalled launch from stacked ecosystem grants instead of waiting on its capital raise

> Assetto's Won deal is frozen on 'Waiting on Customer' pending Assetto's own capital raise, but its Solana/Stellar/Movement architecture touches all three ecosystems where Etherfuse already controls grant and liquidity pools — so Etherfuse can fund the launch liquidity itself rather than wait.

Assetto's onboarding (ONB-67) is stuck in 'Waiting on Customer' because next steps are 'contingent on Assetto completing a capital raise and hiring engineers and marketing staff before integrating Etherfuse Stablebond vaults and launching' [wiki/entities/companies/assetto-precept-labs.md]. But the wiki frames this as an Assetto problem to solve, missing that Assetto's own bridging architecture — **LayerZero OFT across Solana, Stellar, and Movement, with Stellar as the cheapest backend** [wiki/entities/companies/assetto-precept-labs.md] — maps onto three grant/liquidity pipelines Etherfuse already controls:

- **Solana:** Etherfuse is a grant *facilitator* placing $50K–$120K grants, and already offered Assetto a Solana omnibus grant ($50–100K) to seed its liquidity pools, which Abtin expressed interest in [wiki/entities/companies/Solana.md] [wiki/entities/companies/assetto-precept-labs.md].
- **Stellar:** Etherfuse has been allocated ~$1M from Stellar to distribute as grants of $50K–$120K each, with Stellar's grant form provided directly by Etherfuse [wiki/entities/companies/Stellar.md]. Stellar is Assetto's *cheapest* deployment leg.
- **Movement:** Movement offered a MOVE-token grant ($20–100K) *plus* ~$100K liquidity pre-funding [wiki/entities/companies/Movement.md] — and Assetto is a Movement-native team.

**Non-obvious implication:** The three grants Assetto qualifies for (~$150K–$300K combined) exceed the 7% over-collateralization buffer (~$100–150K for CETES) Assetto needs to seed closed-hours liquidity [wiki/entities/companies/assetto-precept-labs.md]. Etherfuse doesn't have to wait on Assetto's raise — it can stack ecosystem grants across the exact chains Assetto bridges to fund the launch liquidity directly, converting a 92%-weighted Onboarding stall into a live TVL channel before the July 9 circle-back.
