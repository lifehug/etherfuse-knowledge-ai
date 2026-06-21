---
title: "P0 is the single integration that captures the untouched Drift/Jupiter/Kamino collateral wishlist"
type: synthesis
source: synthesis
source_date: 2026-06-21
source_trust: reported
confidence: medium
neighborhood: "0xyz"
---

# P0 is the single integration that captures the untouched Drift/Jupiter/Kamino collateral wishlist

> Drift sits at 'Wishlist / no outreach initiated,' but P0 (0.xyz) is a cross-venue portfolio-margin layer that consolidates collateral across Drift, Jupiter, and Kamino — so listing all six Stablebonds as collateral on P0 makes them borrowable on Drift without ever running separate Drift BD.

**The wasted parallel effort.** Drift is logged as a standalone prospect (LEA-140) whose entire deal status is 'Wishlist… No outreach initiated… Identify BD contacts at Drift and propose Stablebond collateral integration' [wiki/entities/companies/Drift.md]. It's framed as a one-by-one venue chase: 'Drift's large user base would provide significant distribution for Stablebonds within the Solana ecosystem' [wiki/entities/companies/Drift.md].

**Why P0 already contains it.** P0 (0.xyz) is explicitly described as a protocol where 'users consolidate positions across venues (Jupiter, Drift, Kamino, etc.) into one unified collateral portfolio and borrow against it cross-venue,' and the active discovery deal is 'listing all 6 Stablebonds (CETES, TESOURO, KTB, GILTS, EUROB, USTRY) as yield-bearing collateral, looping strategies via P0's borrow rails' [wiki/entities/companies/0xyz.md]. P0 is a P0-priority deal already in KYB with Etherfuse compliance, assigned to Maria Esther [wiki/entities/companies/0xyz.md]. Drift is at zero engagement.

**The synthesis no page states.** Because P0's whole product is cross-venue collateral aggregation including Drift, a single Stablebond-as-collateral listing on P0 routes Stablebond collateral into Drift (and Jupiter and Kamino) borrow markets automatically — the exact 'use yield-bearing collateral while trading perpetuals' use case the Drift page wants [wiki/entities/companies/Drift.md], delivered without identifying Drift BD contacts, negotiating a Drift listing, or doing a second KYB. The DeFi case study confirms this is the intended pattern: Stablebonds posted as collateral let traders 'earn sovereign yield while posted' across lending/perp venues [shared/bd/generic-case-studies.md].

**Decision.** Treat Drift, Jupiter, and Kamino not as three separate wishlist deals but as downstream venues that the in-flight P0 integration covers in one shot. Prioritize closing P0's KYB and resolving the closed-hours oracle gap (already in flight via the backend liquidity stablecoin), and the three largest Solana DeFi venues come with it — impact × ease that the current one-venue-at-a-time framing misses. The only residual reason to pursue Drift directly is native Stablebond *trading pairs* (vs. collateral) [wiki/entities/companies/Drift.md], which P0 does not provide.
