---
title: "The KYB/compliance stack is a product line, not onboarding overhead"
type: synthesis
source: synthesis
source_date: 2026-07-09
source_trust: reported
confidence: medium
neighborhood: "alula-finance"
---

# The KYB/compliance stack is a product line, not onboarding overhead

> Etherfuse's proprietary KYB/KYC/AML platform and its free KYB API are a monetizable product and a customer-acquisition wedge in their own right — validated by the Shinhan deck explicitly repositioning Etherfuse as a 'total compliance platform' and by BMONI/BeKey already reskinning the API into their own flows.

Alula Finance is a dead 0%-KYB lead [wiki/entities/companies/alula-finance.md], but the concept page behind it reveals a much bigger asset hiding under 'compliance': Etherfuse has built a full institutional KYB platform — entity-tree builder, jurisdiction-aware questionnaires, automated risk scoring, compliance dashboard, PDF generation — plus a partner-facing KYB API that shipped ~end of April 2026, initially free [wiki/concepts/KYB.md].

Three sources show this is already being consumed as a standalone product, independent of Stablebond usage:
- The Shinhan compliance deck opens by reframing the entire company: 'Etherfuse is a total compliance and infrastructural platform, not just a Stablebond issuer,' with KYB/KYC, wallets, FX, payment rails, reporting and AML screening as the sellable layers, and a proprietary weighted KYB risk-scoring model (client 40% / geography 20% / product 20% / channel 20%) [shared/partners/2026-06-05-shinhan-compliance-presentation.md].
- BMONI committed to route all business onboarding through Etherfuse's KYB + RAMP widget the moment it shipped, and Etherfuse agreed to price it 'free at launch... then the cheapest option in market' [shared/meetings/2026-04-15-bmoni-etherfuse-kyb-business-onboarding.md].
- In the BeKey/bmoni call, the partner's own product philosophy — 'free for the business because they almost certainly guarantee volume... then you take pennies off the dollar' — is exactly the KYB-as-loss-leader-to-lock-in-volume playbook, and BeKey plans to embed Etherfuse's KYB APIs directly into its interface [shared/partners/bekey.md].

The strategic read: KYB is not a cost center gating deals, it's a distribution product. Give it away free to businesses (Mexico PLD fully implemented, NatTech reporting to INH at a fraction of Encode's ~$10k/month) [wiki/concepts/KYB.md], capture the transaction/yield/FX volume those businesses then run through Etherfuse rails, and upsell institutions like Shinhan on the compliance stack as the reason to standardize on Etherfuse. The same architecture is designed to extend to Kazakhstan and Brazil [wiki/concepts/KYB.md], meaning every new-market entry inherits a ready compliance product.
