---
title: "France OAT is a wrapper Etherfuse can ship without AFT"
type: synthesis
source: synthesis
source_date: 2026-07-02
source_trust: reported
confidence: medium
neighborhood: "agence-france-tresor"
---

# France OAT is a wrapper Etherfuse can ship without AFT

> The AFT page treats Agence France Trésor as a required institutional counterpart, but Etherfuse's proven secondary-market model plus the Spiko custody it already runs for EUROB's French leg mean an OAT product needs no AFT relationship at all — only a French DASP registration.

The focal AFT page frames Agence France Trésor as a "key institutional counterpart for Etherfuse's France market entry" and lists as open questions whether a tokenized OAT "would require AFT's explicit approval or cooperation, or can it operate as a secondary-market wrapper" [wiki/entities/companies/agence-france-tresor.md]. Etherfuse's own operating model across six live markets already answers this decisively: it buys sovereign bonds on the **secondary market** and tokenizes them, never needing the issuing treasury as a party. The Kazakhstan structure is explicitly "secondary market purchases of sovereign bonds ... held in segregated accounts" [wiki/concepts/sovereign-bonds.md], and Andres describes the same live model — a segregated SPV per token opening accounts at regulated custodians, minting/burning against real bonds bought and sold at the custodian [shared/partners/paynexa.md]. Just as CETES was tokenized under CNBV with no issuer-side involvement, no OAT deal requires AFT.

Crucially, France sovereign debt is **already inside a live Etherfuse product**: French T-bills are one of eight eurozone issuers backing the live EUROB Stablebond, custodied by Spiko [wiki/markets/france.md] [shared/bond-roadmap.md]. So the two normally-hard legs of a new-country launch — issuer relationship and custody rails — are effectively pre-solved for a dedicated OAT product: AFT is a non-blocker, and Spiko already handles French paper. What remains is a French AMF DASP registration, which the France page itself flags as the MiCA passport into all 27 EU markets [wiki/markets/france.md]. Reframing France from "AFT-dependent, research-stage market entry" to "reuse Spiko custody + file one DASP registration" collapses the perceived timeline and cost on a €2.4T G7 market that is also the gateway to the entire EU.
