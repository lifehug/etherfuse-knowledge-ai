---
title: "The LayerZero/Oracle Security Writeup Andy Owes Avalanche Is the Same Document Four Other Institutional Deals Need"
type: synthesis
source: synthesis
source_date: 2026-07-24
source_trust: reported
confidence: high
neighborhood: "avalabs"
---

# The LayerZero/Oracle Security Writeup Andy Owes Avalanche Is the Same Document Four Other Institutional Deals Need

> The 'LayerZero security writeup (DVN config, oracle setup — Redstone + Pyth + Highland Security ISO)' that Andy has owed Avalanche since May 2026 does not exist as a reusable asset anywhere in Etherfuse's documentation, despite cross-chain infrastructure security being a question every institutional counterparty asks — making this single unwritten document a shared blocker across the Avalanche, Freedom Bank, NIC NBK, MoneyGram, and IBT pipelines.

## The Specific Deliverable

The May 5, 2026 Avalanche call produced an explicit action item: 'Andy to send LayerZero/oracle writeup' covering DVN configuration, oracle setup (Redstone + Pyth), and Highland Security ISO certification [wiki/entities/companies/avalabs.md]. As of the June 5 status update, the ball is with Avalanche but this writeup is listed as an outstanding key action item [wiki/entities/companies/avalabs.md].

## Where the Same Question Appears Across the Pipeline

| Deal | Stage | What They Asked For | Source |
|------|-------|---------------------|--------|
| **Avalanche Foundation** | Negotiation ($3M LOI) | LayerZero DVN config, oracle setup, Highland ISO — explicitly requested | [wiki/entities/companies/avalabs.md] |
| **Freedom Bank** | In Progress (5M users) | 'deck + documentation (regulatory summaries, API specs, IPS integration, custody options)' | [shared/meetings/2026-05-21-freedom-bank-followup.md] |
| **NIC NBK** | Active engagement | Counterparty risk research — questioned single-counterparty model vs multi-bank | [shared/meetings/2026-05-26-nic-nbk.md] |
| **MoneyGram** | NDA stage → DD next | NDA executing, Slack channel spinning up, DD will follow | [shared/meetings/2026-05-13-moneygram-kian-schreiber.md] |
| **IBT (Tajikistan)** | Proposal | Concept brief sent; custody and infrastructure DD will follow | [shared/partners/2026-05-30-etherfuse-ibt-concept-brief.md] |

## What Exists Today vs. What's Missing

Etherfuse has strong documentation on **legal** security (bankruptcy remoteness guide covering Mexican asset separation + Swiss DLT registration [shared/bd/bankruptcy-remoteness-communication-guide.md]) and **audit** security (OtterSec smart contract audit, Highland Security pen tests, Stellar bridge audit [shared/master-knowledge-base.md]). The institutional platform overview markets multi-chain distribution as a key differentiator [shared/institutional-platform-overview.md].

What does **not** exist as a reusable document:

- How LayerZero's DVN (Decentralized Verifier Network) is configured for Stablebond cross-chain transfers
- Which oracle providers (Redstone, Pyth) feed which price data, with what redundancy and staleness guarantees
- Highland Security's ISO certification scope as applied to cross-chain infrastructure
- The cross-chain supply tracking and reconciliation mechanism that prevents double-minting across Solana, Stellar, and EVM chains

These are precisely the questions institutional counterparties ask when they see 'available on 5+ blockchains' in the pitch deck.

## Impact of Creating This Once

A single reusable 'Cross-Chain Infrastructure Security' document, covering the LayerZero/oracle/Highland scope Avalanche requested, would:

1. Unblock the Avalanche IC pitch — this is an explicitly owed deliverable [wiki/entities/companies/avalabs.md]
2. Satisfy a chunk of Freedom Bank's documentation request before their July–August evaluation window [shared/partners/2026-05-21-freedom-bank-aidos-zhumagulov.md]
3. Feed into NIC NBK's counterparty risk research request [shared/meetings/2026-05-26-nic-nbk.md]
4. Pre-load MoneyGram's upcoming DD process [shared/meetings/2026-05-13-moneygram-kian-schreiber.md]
5. Become a permanent section in the institutional platform overview, which currently has a gap between 'multi-chain by default' and 'security & compliance summary' [shared/institutional-platform-overview.md]

This is a documentation task, not an engineering task. The infrastructure already works. The writeup just hasn't been formalized.
