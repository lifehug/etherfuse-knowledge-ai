---
title: "AAA CGS Is the Missing Credit Anchor for the Stablebond Index"
type: synthesis
source: synthesis
source_date: 2026-07-22
source_trust: reported
confidence: medium
neighborhood: "australian-office-of-financial-management"
---

# AAA CGS Is the Missing Credit Anchor for the Stablebond Index

> NIC NBK asked for an on-chain Stablebond index yielding ~6% blended, and multiple existing findings discuss the wrapper vehicle (3iQ, AIX ETN, AIFC SPC) — but none address composition, and a standalone AAA-rated AUD Stablebond is the single product that makes the index viable for institutional mandates with minimum credit quality thresholds.

## The Index Request

NIC NBK explicitly asked about on-chain index funds during Dave's Kazakhstan pitch: 'Dave suggested an index of Etherfuse stable bonds = ~6% blended yield, diversified across strong and emerging market currencies' [shared/meetings/2026-05-26-nic-nbk.md]. NIC also raised counterparty-concentration risk as their main objection to the single-custodian model.

## The Composition Gap

Existing analysis covers how to package the index (3iQ fund wrapper, AIX ETN, AIFC SPC tax optimization) but not **what goes into it**. The current live product credit profile is:

| Product | Rating | Yield |
|---------|--------|-------|
| CETES (MXN) | Baa2/BBB | ~5.58% |
| TESOURO (BRL) | Ba1/BB | ~13.14% |
| GILTS (GBP) | Aa3/AA | ~3.43% |
| EUROB (EUR) | Aaa to Baa3 (basket) | ~1.53% |
| USTRY (USD) | Aaa/Aa+ | ~3.21% |
| KTB (KRW) | AA | ~2.25% |

[shared/master-knowledge-base.md] [shared/bond-roadmap.md]

Institutional mandates (pension funds, sovereign wealth, insurance) typically require a minimum average credit quality (often A or above) for fixed-income allocations. A blended index heavily weighted to Mexico (BBB) and Brazil (BB) to hit 6% yield will breach those thresholds.

## Why Australia Specifically

Australian CGS carry **unanimous AAA/Aaa/AAA** from all three agencies — S&P, Moody's, and Fitch [wiki/markets/australia.md] [shared/research/raw/2026-07-03-market-research-australia-websearch.md]. This makes it the only planned **standalone** AAA product (EUROB is a multi-country basket; USTRY recently lost its Aaa from one agency). At a 4%+ AUD yield (RBA cash rate was 4.35% as of the research date [wiki/markets/australia.md]), CGS contributes both quality AND meaningful yield.

An index with 15-20% Australian CGS weight would:
- Raise the blended credit quality above the institutional A-threshold
- Add geographic diversification (APAC, developed market) that answers NIC's concentration objection
- Maintain a ~5-6% blended yield target

## Implication

The Q3 2026 CGS launch isn't just another country on the roadmap — it's the credit quality input that determines whether the institutional index product NIC requested is marketable to regulated buyers. Prioritize accordingly.
