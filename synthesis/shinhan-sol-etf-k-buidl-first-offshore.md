---
title: "Shinhan × Etherfuse is building the world's first offshore K-BUIDL — and Solana is the rails"
type: synthesis
source: synthesis
source_date: 2026-06-08
source_trust: reported
confidence: high
---

# Shinhan × Etherfuse is building the world's first offshore K-BUIDL — and Solana is the rails

> The Shinhan × Etherfuse collaboration isn't just another RWA tokenization deal. It's the first time Korean government bond / bond ETF exposure has been structured for offshore issuance as a Stablebond — creating a BUIDL-equivalent for the Korean capital market, with zero smart contract risk, bankruptcy-remote custody, and omni-chain liquidity.

## What this is

Shinhan Asset Management manages a SOL Short-Term Bond ETF listed on KRX — a bond-type ETF benchmarked to the KAP MTM MMF Index (WAM <120 days), investing in AA-/A2+ Korean bonds. Not technically an MMF, so it escapes the tight WAM and 30% liquidity floor rules that constrain book-value MMFs. T+1 redemption via designated participants.

Etherfuse is the token issuer. Shinhan Securities is the onshore distributor and custody partner. An offshore vehicle (Etherfuse entity) acquires the fund in USD through Shinhan Securities Seoul, and Etherfuse mints 1:1 Stablebond tokens on Solana against those custodied reserves. Global investors interact only with the vault (USDT/USDC in → Stablebond token out). TRM Labs screens every vault interaction.

**Call it K-BUIDL.** The structure mirrors BlackRock BUIDL role-for-role, with one key difference: Etherfuse is not a transfer agent maintaining an investor cap table — it's the issuer against reserves. No on-chain KYC register; compliance is AML screening at point of interaction.

## Why it matters beyond the deal itself

**1. This is the first KRW bond ETF tokenized offshore.**  
KRW is a legally non-deliverable currency — you cannot hold Korean Won in a bank outside Korea through normal channels (see `synthesis/ktb-only-offshore-krw-instrument.md`). This structure gives global investors exposure to Korean bond yields without a Korean bank account, without NDF derivatives, and without smart-contract counterparty risk.

**2. Shinhan is not just a custodian here — they are a distribution partner.**  
Shinhan Asset Management provides the fund. Shinhan Securities acts as onshore distributor and broker-dealer. Shinhan partners provide domestic custody. The relationship runs three layers deep. This is structurally more locked-in than a standard custody arrangement.

**3. The regulatory moat is real — and growing.**  
This transaction engages Bank of Korea, MoEF, FSC, FSS, and KoFIU. Reporting is filed by Etherfuse's standing proxy and Shinhan Securities. Etherfuse doesn't file directly. The path from "pre-tapping → pre-approval → formal process" is being walked with Korean law firm engagement for sandbox readiness. Few competitors have the relationships or regulatory footprint to replicate this.

**4. KRW/USD FX risk is the open structural question.**  
Unlike BUIDL (USD assets, USD investors), this structure carries KRW/USD exposure. Whether to hedge (and who bears the cost) is explicitly deferred to mutual agreement before implementation. This is a real question — but also a feature for investors who specifically want KRW beta.

**5. Omni-chain from day one.**  
Solana is the primary chain. ETH, SOL, and other chains are supported via Etherfuse-native omni-chain infrastructure. This is not a Solana-only product.

## The operation is already operational (KTB side)

The parallel Stablebond Operation Rules Term Sheet (non-binding, in discussion) establishes that Etherfuse is already submitting weekly Purchase Requests to Shinhan Securities every Wednesday KST. The mechanics are live: USD wire to Shinhan Bank (SWIFT: SHBKKRSE), USD→KRW FX conversion, OTC bond sourcing in KRW 1B lots, ±3 bps Valuation Yield tolerance, T+0–T+1 settlement. Stablebonds are minted ONLY on Executed Amount — no pre-minting.

This is not a concept paper. The operational rails are being built in parallel with regulatory approval.

## Positioning implication

The Shinhan × Etherfuse K-BUIDL story is one of Etherfuse's strongest proof points for the broader market:

- **For Korean institutional investors:** first compliant path to tokenize KRX-listed fund products offshore
- **For global investors:** first and only way to get KRW bond yield exposure on-chain without a Korean entity
- **For regulators:** BUIDL-equivalent structure they already understand, with domestic Korean custody and AML at every touchpoint
- **For Etherfuse's pipeline:** Shinhan is a $300B+ financial group — this is a flagship institutional partnership, not a pilot

## Status (June 2026)

| Item | Status |
|------|--------|
| Deal structure | Agreed in principle |
| Regulatory path | In progress (sandbox via law firm engagement) |
| Underlying asset | SOL Short-Term Bond ETF (KRX-listed, Shinhan AM) |
| KTB purchase operations | Term sheet in discussion, operationally active |
| PoC | Not yet started (item 2 in next actions) |
| FX hedging decision | TBD (mutual agreement required) |
| Press release | Pending regulatory sandbox clearance |

## Source Documents

- `partners/shinhan/2026-06-08-rwa-collaboration-model.md`
- `partners/shinhan/2026-06-08-k-buidl-regulatory-requirements-v7.md`
- `partners/shinhan/2026-06-08-underlying-assets-etf-strategy.md`
- `partners/shinhan/2026-06-08-ktb-stablebond-operation-rules-term-sheet.md`
