---
title: "EUROB-Only Pitches Leave 6x Partner Revenue on the Table"
type: synthesis
source: synthesis
source_date: 2026-07-23
source_trust: reported
confidence: medium
neighborhood: "av-eu"
---

# EUROB-Only Pitches Leave 6x Partner Revenue on the Table

> The yield-tiered partner revenue model creates a 6x commission differential between EUROB (10 bps at ~1.64% yield) and TESOURO (60 bps at ~13% yield), meaning every EUR-denominated prospect pitched only EUROB — like AV.eu — is being shown the lowest-earning product when the 'Why Stablebonds' tax-efficiency framework already justifies multi-product float-parking at higher tiers.

## The Math

Etherfuse's partner revenue tiers pay basis points of AUM scaled to the underlying bond yield [shared/bd/partner-revenue-tiers.md]:

| Product | Yield | Partner Share | Revenue on $10M AUM |
|---------|-------|---------------|---------------------|
| EUROB | ~1.54% | 10 bps | $10,000/yr |
| USTRY | ~3.21% | 10 bps | $10,000/yr |
| CETES | ~5.58% | 20 bps | $20,000/yr |
| TESOURO | ~13.14% | 60 bps | $60,000/yr |

A distribution partner earns 6x more commission on the same AUM in TESOURO vs. EUROB. Etherfuse's own management fee also scales with yield (0.25% at low yield to 1.5% at high yield) [shared/bd/partner-revenue-tiers.md], creating the same 6x multiplier on Etherfuse's side.

## The Current Pitch Leaves Money on the Table

AV.eu was pitched EUROB exclusively — '~1.64% yield on idle EUR balances' [wiki/entities/companies/av-eu.md]. The AV.eu page itself notes: 'Lower yield on EUROB (~1.64%) compared to LATAM products — value prop is more about settlement efficiency than yield' [wiki/entities/companies/av-eu.md]. This is correct for the settlement layer, but EU grant organizations hold idle EUR for weeks or months between receipt and disbursement. That float period is a yield opportunity.

## The Multi-Product Pitch

The 'Why Stablebonds vs Direct Bonds' objection handler already provides the justification: 'Holding them outside of Mexico gives you an instant 36% tax rate that you save. If you onboard your offshore structure, you don't have to pay that' [shared/bd/why-stablebonds-vs-direct-bonds.md]. An EU-funded organization using an offshore structure could park idle EUR in TESOURO (~13%) during the float window and convert back to EUROB for disbursement — earning ~11% more yield while the partner earns 6x more commission.

The recommended pitch structure for any EUR-denominated prospect: **EUROB for settlement and disbursement** (the efficiency argument: 2-5% fee savings vs. banking rails) **+ TESOURO or CETES for idle-balance float parking** (the yield argument: 6-13% vs. 1.64%). This doubles Etherfuse's revenue on the same prospect by capturing both ramp fees on the EUROB settlement leg [shared/bd/partner-revenue-tiers.md] and management fees on the higher-yield float leg.

## Caveat

Float-parking in non-EUR products introduces FX risk and operational complexity. The 'Why Stablebonds' doc warns not to make specific tax promises — 'say there are meaningful tax efficiencies depending on structure and let them explore with their tax advisors' [shared/bd/why-stablebonds-vs-direct-bonds.md]. But for organizations with predictable multi-week float windows, the yield differential is large enough to absorb modest FX drag.
