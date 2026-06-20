---
title: "0.xyz is P0 — the stalled, grant-funded 6-asset collateral deal"
type: synthesis
source: synthesis
source_date: 2026-06-20
source_trust: reported
confidence: high
neighborhood: "0-xyz"
---

# 0.xyz is P0 — the stalled, grant-funded 6-asset collateral deal

> The 0.xyz wiki page treats the P0-priority partner as an unknown 'Waiting on Customer' blocker, but SALES-380 in the same neighborhood reveals it is P0, a Solana portfolio-margin protocol that already agreed to list all six Stablebonds as collateral — and its only real blocker is the closed-hours price-gap problem Etherfuse's in-flight backend liquidity stablecoin is built to solve.

## The identity gap

The focal entity page says outright that '[f]urther details about 0.xyz's business operations, products, or market focus are not yet available on record' and lists six Open Questions including 'What is the nature of 0.xyz's business and why is it classified P0 priority?' [wiki/entities/companies/0-xyz.md]. Every one of those questions is already answered by a Won sales record in the same neighborhood: **0.xyz is P0, a DeFi-native portfolio margin protocol on Solana** run by Jeremie De Pins De Caucalieres (jere@0.xyz), where users consolidate positions across Jupiter, Drift, Kamino into one cross-venue collateral portfolio [teams/sales/2026-03-26-0xyz-p0.md]. The compliance and integration tracks (Maria Esther / AJ Taylor, both opened 2026-04-21) are the downstream of a deal Andres Salcedo already closed [teams/cfo/compliance/2026-04-21-0xyz-kyb-p0.md, teams/cto/2026-04-21-onb66-0xyz-integration.md].

## What was actually agreed

The deal is not a vague 'integration.' P0 agreed to **list all six Stablebonds (CETES, TESOURO, KTB, GILTS, EUROB, USTRY) as yield-bearing collateral**, enable looping strategies on its borrow rails, and add an MXN on/off-ramp at 20bps for payment use cases — a single partner driving usage across the entire live asset roster plus the FX rail [teams/sales/2026-03-26-0xyz-p0.md]. Jeremie also flagged Swiss franc interest for future tokens, matching Etherfuse's Switzerland/DLT registration track [wiki/entities/companies/Etherfuse.md].

## The blocker is a problem we are already solving

The 'Waiting on Customer' status hides a specific, technical objection: Jeremie's 'main concern' is that **market-close price gaps on sovereign bonds could trigger bad debt or unwanted liquidations on leveraged positions**, plus oracle pricing (Pyth/Switchboard) for RWA-backed assets [teams/sales/2026-03-26-0xyz-p0.md]. That is precisely the closed-hours liquidity gap the existing 'backend liquidity stablecoin' work is designed to close, and the over-collateralization buffer (7%, ~100–150K for CETES) plus DeFi pools already quoted to comparable lending/margin prospects like Assetto and Rheo [teams/ceo/docs/inbox/linear/2026-04-16-sales-332-assetto-precept-labs.md, teams/cfo/2026-04-21-rheo-partnership-structure.md]. The unblock is a product conversation Etherfuse can already have — not a customer-side dependency.

## The free money sitting on the table

SALES-380 also records that the **Solana Foundation is offering up to $70K to fund the Etherfuse payments integration**, with the action item 'Andy to connect Jeremie with Antonio (Solana Foundation)' [teams/sales/2026-03-26-0xyz-p0.md]. This is the same omnibus-grant mechanism Etherfuse routinely runs (e.g. the $50–120K Stellar/Solana/Monad grants offered to SBC/Stablecoin.xyz) [teams/sales/2026-04-19-sbc-stablecoinxyz.md]. A Won, P0 deal is stalled on a customer-side technical worry while $70K of integration funding goes unclaimed.

## Action

Re-engage Jeremie directly (no Etherfuse contact is even listed on the wiki page) on two concrete items: (1) walk him through the over-collateralization + backend-liquidity answer to the closed-hours price-gap concern, and (2) make the Antonio/Solana Foundation intro to bank the $70K. Both are near-zero-cost and convert a six-asset, FX-rail usage driver that the entity page currently can't even describe.
