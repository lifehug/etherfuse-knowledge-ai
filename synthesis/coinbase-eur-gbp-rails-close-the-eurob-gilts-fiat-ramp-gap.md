---
title: "Coinbase EUR/GBP rails close the missing fiat ramp for EUROB and GILTS"
type: synthesis
source: synthesis
source_date: 2026-06-12
source_trust: reported
confidence: medium
neighborhood: "aaro-capital"
---

# Coinbase EUR/GBP rails close the missing fiat ramp for EUROB and GILTS

> Etherfuse ships live EUROB and GILTS Stablebonds but has no native EUR or GBP fiat on/off-ramp — only MXN SPEI and BRL PIX — and Coinbase Institutional just turned on EUR and GBP payment rails for Etherfuse as an existing client, which is the cheapest, fastest way to make its European products actually usable for European treasury and allocator demand.

**The gap no single page names.** Etherfuse's own institutional platform overview lists exactly two native fiat rails — Mexican SPEI (MXN) and Brazilian PIX (BRL) — plus CCTP for USDC; everything else routes through stablecoins [shared/institutional-platform-overview.md]. The partner pricing sheet confirms this: ramp pricing covers only USDC↔MXN, with EUR/GBP nowhere [shared/bd/partner-revenue-tiers.md]. Yet EUROB (EUR) and GILTS (GBP) are *live* products with custodians (Spiko, Archax) and real demand [shared/master-knowledge-base.md]. The result: European clients can hold these tokens but can't get in/out in their home currency without an external rail.

**The case studies already expose the workaround.** The Rotterdam freight operator converges everything to USDC and then 'converts to EUR at institutional FX rates and wires to Netherlands HQ' — an off-platform EUR leg Etherfuse doesn't own [shared/bd/case-study-freight-eu-egypt-mena.md]. Singapore and Hong Kong clients similarly redeem to USD via Circle rather than into their native EUR/GBP positions [shared/bd/case-study-tech-singapore.md][shared/bd/case-study-psp-hongkong.md]. Every one of these flows leaks the final fiat hop to a third party.

**The unlock just arrived.** Coinbase Institutional notified Etherfuse on 2026-06-10 that 'EUR and GBP Payment Rails Now Live' [shared/partners/coinbase.md]. Etherfuse is already a Coinbase institutional counterparty (it received the notice), so this is a near-zero-setup capability, not a new partnership. Wiring Coinbase EUR/GBP rails to EUROB and GILTS internalizes the missing leg and turns two otherwise rail-less products into complete buy-and-redeem-in-local-currency offerings.

**Why it matters now.** This is the same operational-rail bottleneck the 1Money/US-ACH finding solves for the dollar — but for the euro and sterling, and with rails that are already switched on rather than bartered for. It also directly serves the focal neighborhood: a UK institutional allocator like Aaro Capital was pitched GILTS as 'foundational yield' [wiki/entities/companies/aaro-capital.md], but a UK buyer needs a GBP in/out path, not a USDC detour. Pairing GILTS with Coinbase GBP rails (and Archax, the GILTS custodian, already expanding across regulated venues [shared/ecosystems/capital-markets.md]) converts the European-product pitch from theoretical to transactable.

**Action:** scope a Coinbase EUR/GBP ramp integration as the fiat layer for EUROB and GILTS, then re-pitch UK/EU institutional prospects (starting with the live Aaro thread) with a complete local-currency on/off-ramp rather than a stablecoin round-trip.
