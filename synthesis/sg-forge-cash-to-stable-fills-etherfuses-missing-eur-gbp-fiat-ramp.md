---
title: "SG Forge's Cash-to-Stable ramp fills Etherfuse's missing EUR/GBP fiat rail"
type: synthesis
source: synthesis
source_date: 2026-07-03
source_trust: reported
confidence: medium
neighborhood: "aha-company"
---

# SG Forge's Cash-to-Stable ramp fills Etherfuse's missing EUR/GBP fiat rail

> Etherfuse ships EUROB (EUR) and GILTS (GBP) as live products but has fiat on/off-ramps only in MXN and BRL — and SG Forge's 'Cash to Stable' product, launching on Etherfuse's own Stellar deployment, is exactly the EUR/GBP ramp needed to make those European Stablebonds operationally complete.

Etherfuse has EUROB (EUR sovereign debt) and GILTS (UK Gilts) live as products [shared/overview.md, shared/master-knowledge-base.md], but its native fiat rails are limited to **Mexican SPEI (MXN) and Brazilian PIX (BRL)** — the institutional platform overview lists no EUR (SEPA) or GBP (Faster Payments) on-ramp [shared/institutional-platform-overview.md]. That means Etherfuse's European products can be bought with stablecoins but not directly funded from EUR/GBP bank accounts, a gap for exactly the European institutional users EUROB/GILTS target.

In the April 2026 AHA meeting, Enzo flagged that SG Forge is building a **'Cash to Stable' product (already live on Ethereum + Solana, launching on Stellar soon)** and discussed integrating it as a **EUR/GBP fiat ramp into Etherfuse assets** [wiki/entities/companies/aha-company.md]. This is the same structural completion the 1Money finding identified for US ACH rails — a partner supplying the fiat leg Etherfuse doesn't operate itself — but for Europe, and it lands on Stellar, the chain Etherfuse already ships on and where AHA is SDF's integration partner [wiki/entities/companies/aha-company.md, shared/overview.md]. Integration friction is therefore low.

Decision-useful implication: the SG Forge thread should be scoped as **two linked products, not one** — (1) EUROB-backing for SG Forge's own euro stablecoin, and (2) SG Forge Cash-to-Stable as Etherfuse's EUR/GBP on-ramp — and both are prerequisites to seriously distributing EUROB/GILTS into European institutional users, which the current 'Nurture / intro pending' status leaves dormant [wiki/entities/companies/aha-company.md].
