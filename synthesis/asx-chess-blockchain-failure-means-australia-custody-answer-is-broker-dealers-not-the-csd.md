---
title: "ASX's $250M CHESS blockchain failure means the Australia custody answer is broker-dealers, not the CSD"
type: synthesis
source: synthesis
source_date: 2026-07-22
source_trust: reported
confidence: medium
neighborhood: "australian-securities-and-investments-commission"
---

# ASX's $250M CHESS blockchain failure means the Australia custody answer is broker-dealers, not the CSD

> ASX wrote off A$250M on its blockchain-based CHESS replacement, which eliminates the CSD as either a competitor or a custody partner for tokenized CGS — and confirms that Etherfuse should replicate its secondary-market broker-dealer model (BBVA/Actinver in Mexico, Shinhan in Korea) with an Australian broker-dealer to fill the open custody gap.

The Australia market page notes that 'ASX wrote off A$250 million on a blockchain-based CHESS replacement project in 2022, signaling caution around DLT-based settlement infrastructure at the CSD level' and explicitly flags that 'No custody partner has been identified for Australia' [wiki/markets/Australia.md].

This is a structurally important signal, not just a data point. In every other Etherfuse market, the custody partner is a local broker-dealer or bank — not the CSD:
- Mexico: BBVA, Actinver, Kuspit (all broker-dealers) [shared/master-knowledge-base.md]
- Korea: Shinhan Securities [shared/master-knowledge-base.md]
- UK: Archax [shared/master-knowledge-base.md]
- Brazil: B3 (exchange, not CSD function) [shared/master-knowledge-base.md]

The regulatory framework confirms the model: 'Underlying bonds are purchased in secondary markets through locally licensed brokers... secondary market purchases are not new securities offerings' [wiki/concepts/regulatory.md]. The bankruptcy remoteness guide explains why this works legally: 'Assets are held at Category I regulated financial institutions... without solvency problems and not subject to special regulatory measures' [shared/bd/bankruptcy-remoteness-communication-guide.md].

With ASX having publicly abandoned its own blockchain settlement project, no CSD-led tokenization competitor will emerge in Australia for years. This removes one potential threat but also removes the most obvious custody pathway. The solution is clear from the pattern: find a large Australian broker-dealer or bank with primary-dealer status for CGS (similar to how Shinhan is a Korean securities firm and BBVA is a Mexican bank). Australia's primary dealer equivalent is the 'market maker panel' designated by the AOFM for CGS auctions.

The collateral playbook [shared/bd/collateral-playbook-ktb-krwq.md] and the Visa card model [shared/bd/visa-local-issuer-card-collateral.md] both show that the custody partner selection cascades into messaging ('the asset's credibility replaces the need for custodian credibility') and distribution. Choosing the right Australian broker-dealer now unblocks the Q3 CGS launch.

**Action:** Identify AOFM market maker panel members (Australia's primary dealer equivalent) as CGS custody partner candidates. Prioritize those with existing digital asset or fintech initiatives. Standard Chartered, already in discussions for APAC expansion [shared/master-knowledge-base.md], may cover Australia from its Singapore/HK hub.
