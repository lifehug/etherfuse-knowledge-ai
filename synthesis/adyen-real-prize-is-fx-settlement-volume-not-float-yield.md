---
title: "Adyen's real prize is FX-settlement volume, not float yield"
type: synthesis
source: synthesis
source_date: 2026-06-30
source_trust: reported
confidence: medium
neighborhood: "adyen"
---

# Adyen's real prize is FX-settlement volume, not float yield

> At Adyen's enterprise transaction volumes, becoming its MXN/LatAm settlement layer at the 5bps FX tier is a far larger and faster revenue lever than the 'settlement float optimization' the wiki pitches.

The Adyen wiki page frames the entire opportunity as "multi-market settlement float optimization via Stablebonds (CETES, potentially others)" and books it as a yield play [wiki/entities/companies/adyen.md]. That undersells where the money actually is. Adyen is described as enterprise payment infrastructure "processing significant transaction volumes for major brands" across Mexico, Argentina, the US and many other markets [wiki/entities/companies/adyen.md] — and Etherfuse's revenue on that flow scales with **FX/settlement volume**, not with idle-float yield share.

The Case Study 3 remittance playbook shows the mechanism: replace the USD→correspondent-bank→MXN chain with USDC→MXNe/CETES settlement, cutting FX spread from 100–300+ bps to **5–20 bps**, settling same-day, while the in-transit float earns ~7% [shared/bd/generic-case-studies.md]. Etherfuse's published CETES FX pricing reaches the floor of **5 bps at $100M+ monthly volume** [shared/partners/anchorage-one-pager.md], and the Visa card-collateral doc confirms the same 5–20 bps tiering on local-fiat settlement off-rail [shared/bd/visa-local-issuer-card-collateral.md]. An enterprise acquirer the size of Adyen clears that $100M/month threshold many times over, which means the FX-settlement revenue line dwarfs anything float yield contributes — and it is collected on *every* MX/LatAm payout, not just the slice of balance left idle.

The reframe matters for how to open the deal. Of Adyen's three named markets, only Mexico has a live, high-value local Stablebond (CETES); Argentina has no product yet (see the Argentina roadmap gap) and USTRY's ~3% yield is a weak hook. So the correct day-one pitch is not "earn yield on your float" but **"be the cheapest, instant MXN settlement rail for your Mexican merchant payouts via MXNe/CETES"** — with float yield and the option to pass sovereign yield through to merchants as differentiators on top [shared/bd/generic-case-studies.md]. Given the page sits at Wishlist with "identify contacts" as the only next step [wiki/entities/companies/adyen.md], the immediate action is to find a contact and lead with the FX-corridor economics, which convert faster and bigger than the yield framing currently on file.
