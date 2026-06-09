---
title: "Shinhan × Etherfuse — RWA Collaboration Model"
type: partner-doc
partner: Shinhan
date: 2026-06-08
classification: confidential
source: "3._Shinhan_Etherfuse_RWA_Collaboration_Model_20260608.pdf"
---

# Shinhan × Etherfuse — RWA Collaboration Model

> End-to-end tokenization of a SOL ETF via the Etherfuse model. Confidential — Shinhan × Etherfuse | June 2026.

## Deal Structure

| Role | Entity |
|------|--------|
| **Issuer** (regulated) | Etherfuse |
| **Custodian** (Real Asset) | Shinhan Partners (Bank, etc.) |
| **Target Asset** | SOL ETF (Shinhan Asset Management) |

## Architecture Overview

### Off-Chain Layer
- **Shinhan Asset Management** — Fund Manager / ETF Issuer. Manages SOL ETF exposure & distribution.
- **Shinhan Securities × Custody Partners** — Offshore Distributor and Domestic Custodian. Safekeeping under Etherfuse entity. Provides Risk Segregation & Bankruptcy Remoteness.

### Bridge Layer (Etherfuse)
- Buys & holds the Fund via the custodian
- Mints Stablebond tokens against reserves
- **Oracle / Price Attestation** — on-chain oracle or off-chain attestation via API

### On-Chain Layer
- **Vault** — Mint/Subscribe & Redeem/Withdraw. Accepts USDT/USDC
- **Global Investors (LP/Investor)** — Deposit stablecoins → Receive Stablebond token
- **Yield** — NAV Accrual (Total return)
- **AML Compliance** — TRM Labs on every vault interaction (mint/subscribe & redeem/withdraw). Flagged transactions blocked.
- **Multichain (Omni) Liquidity** — Etherfuse-native

### On/Off Ramp
- **Broker (e.g., Exchange)** — USD ↔ Stablecoin conversion

## Token Flow

```
Global Investor → deposits stablecoins → Vault
Vault → forwards USD → Shinhan Securities
Shinhan → subscribes Fund → Fund Shares acquired into custody
Custodian → NAV data → Etherfuse oracle → on-chain token price
Vault → mints Stablebond token → Investor wallet
```

## Key Differentiators

1. **Zero smart contract risk** — tokens exchanged for Fund shares, assets in regulated custody
2. **Omni-chain** (ETH/SOL/etc) · NAV-accrual yield · Proof-of-Reserves + audited custody
3. **Risk Segregation** between Real-World Assets and Digital Assets

## Regulatory Pathway

- **Pre-tapping → pre-approval → formal process**
- Sandbox readiness via law firm engagement
