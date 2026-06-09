---
title: "Shinhan × Etherfuse — K-BUIDL Regulatory Requirements Report V7"
type: partner-doc
partner: Shinhan
date: 2026-06-08
classification: confidential
source: "1._Shinhan_Etherfuse_Regulatory_Requirement_Report_V7.docx"
version: 7
---

# Shinhan × Etherfuse RWA Tokenization Project — Regulatory Requirements

> Classification: Confidential / Internal Partner Use Only  
> Date: June 2026  
> **Drafting Note (provisional):** Token issuance mechanisms, stablecoin conversion, FX processing, and vendor arrangements are tentative drafts for discussion only. All terms subject to Etherfuse review and final confirmation. Specific vendor names are illustrative pending final determination.

## 1. Purpose & Structure

**Primary purpose:** First domestic case of an offshore "permission is not required" K-BUIDL MMF tokenization. Technical specification for issuing, on Solana, a tokenized representation of a Shinhan Asset Management money market fund.

**Model:** Mirrors BlackRock's BUIDL framework. Maps Korean regulatory data requirements onto on-chain architecture. Commercial/GTM matters are out of scope.

### Underlying Asset
**SOL Short-Term Bond (Tentative) ETF** — KRX-listed, actively managed ETF by Shinhan Asset Management.
- Classified as a **security-type (bond) ETF** — not a traditional MMF; not subject to tight WAM limits or 30% liquidity floor
- Benchmark: **KAP MTM MMF Index** (weighted average maturity <120 days)
- Invests primarily in high-quality bonds (**AA- or above**) and commercial papers (**A2- or above**) with remaining maturity ≤6 months
- **Liquidity:** Market sale = T+2 settlement. Institutional investor direct redemption via designated participants (APs) = T+1.

### Acquisition
Offshore vehicle (foreign investor) acquires fund as underlying RWA, subscribing in USD through **Shinhan Securities (Seoul branch)** as onshore distributor.

### Tokenization
1:1 token minted offshore on **Solana** via the Etherfuse model.

### Applicable Authorities
- **Bank of Korea + Ministry of Economy and Finance** — foreign-exchange reporting
- **Financial Services Commission + Financial Supervisory Service** — securities regulation + foreign-investor identification
- **Korea FIU (KoFIU)** — anti-money laundering

Reporting filed on Etherfuse's behalf by its standing proxy/custodian and Shinhan Securities. Etherfuse does not file directly.

---

## 2. Entity Mapping (BlackRock BUIDL ↔ Shinhan × Etherfuse)

Mirrors the BUIDL reference model role-for-role across off-chain and bridge layers. On-chain layer is Etherfuse's vault.

**Key divergence from BUIDL:** Etherfuse is the token issuer minting against custodied reserves — it does **not** act as a transfer agent maintaining an investor cap table.

---

## 3. Architecture & Roles

No PII or proprietary data on the public ledger. No transfer agent, no permission-required KYC register. Investor compliance via AML/sanctions screening at each vault interaction.

### Layer 1: Off-Chain (Real-World Asset & Custody)
| Entity | Role |
|--------|------|
| **Shinhan Asset Management** | Fund Manager. Manages ETF, retains fiduciary duty. Digital layer does not affect fund management (segregated). |
| **Shinhan Securities (Seoul)** | Onshore Distributor / Broker-Dealer. Offshore vehicle opens USD account and subscribes to fund through this channel. |
| **Shinhan Partners** | Domestic Custodian and Fund Administrator. Holds fund shares in legal custody. Calculates and publishes NAV daily (EOD). |

### Layer 2: Bridge (Tokenization & NAV Linkage)
| Entity | Role |
|--------|------|
| **Etherfuse** | Token Issuer. Acquires and holds fund via custodian. Issues Stablebond tokens 1:1 against custodied reserves. **Not a transfer agent** — no investor cap table. |
| **NAV Oracle / Attestation** | NAV from custodian/admin → Etherfuse → pushed on-chain. Token price accrues proportional to NAV. |
| **Stablecoin ↔ USD Bridge** | Qualified custodian (Anchorage / Coinbase Prime). Converts stablecoins→USD on subscription; USD→stablecoins on redemption. |

### Layer 3: On-Chain (Solana, omni-chain optional)
| Component | Description |
|-----------|-------------|
| **Vault** | Stablecoin deposit mints Stablebond tokens. Redemption burns them. |
| **Global Investors** | Subscribe/redeem by depositing stablecoins (USDT/USDC). Interact only with the vault. |
| **Yield** | NAV accrual (total return). Token price appreciates with NAV. No distributions; gains realized upon redemption. |
| **AML Compliance** | Continuous TRM Labs screening at each vault interaction. Flagged transactions blocked. No investor-level KYC whitelist at token layer. |

---

## 4. NAV, Currency & FX

### NAV Mechanism
Data flow: **Custodian/Admin** (NAV calculation) → **Etherfuse** (oracle push) → **On-chain token price**
- Calculated once daily at EOD in USD
- Transmitted by API or daily file, reusing fund's standard publishing process
- Intraday NAV is optional

### Currency Chain
```
Stablecoin (USDT/USDC) ↔ USD (qualified custodian or Shinhan Securities KR account) ↔ KRW (fund's underlying assets)
```

### FX Risk (To Be Determined by Mutual Agreement)
Fund holds KRW-denominated assets; investors subscribe/redeem in USD or stablecoins → **KRW/USD exposure** (unlike BUIDL which is USD→USD).

Open items for mutual agreement:
- Hedge or not (and cost/bearing party)
- FX reporting flow
- Whether FX transaction metadata is anchored on Solana (scope + privacy handling)

---

## 5. Risk Segregation & Bankruptcy Remoteness

| Insolvency Scenario | Protection |
|--------------------|------------|
| **Shinhan Asset Management** | Fund assets remain segregated in custody. Management may transfer to another asset manager. |
| **Custodian** | Fund shares held in name of offshore vehicle. May transfer to another custodian. |
| **Etherfuse** | Issuing vehicle is bankruptcy-remote SPE. Fund shares distributed to token holders. |
| **Third-party verification** | Proof of Reserves reconciles custodied fund shares vs. circulating token supply + audited custody. No smart-contract credit risk on backing. |

---

## 6. Korean Regulatory Reporting & On-Chain Mapping

Applicable statutes:
- **Foreign Exchange Transactions Act**
- **Financial Investment Services and Capital Markets Act (FSCMA)**
- **Act on Reporting and Use of Certain Financial Transaction Information (Specified Financial Information Act)** — AML

**Key principle:** Statutory reporting fulfilled off-chain through established regulatory channels. On-chain data records do not automatically replace legal filing procedures. Technical anchoring of metadata on Solana for transaction reconciliation may be performed subject to mutual agreement.

---

## 7. End-to-End Flow

### Subscription
1. Global investor deposits USDT/USDC into Etherfuse vault (on-chain)
2. TRM Labs screens wallet address; clear → proceed (compliance)
3. Vault forwards stablecoins to qualified custodian — Anchorage / Coinbase Prime (bridge)
4. Custodian converts stablecoins to USD, typically within 24 hours (bridge)
5. Shinhan Securities (KR) processes fund subscription with USD (off-chain)
6. Fund shares acquired into custody; Etherfuse reserves increase (off-chain / bridge)
7. Vault mints Stablebond tokens to investor's wallet (on-chain)

### Redemption
1. Investor submits redemption request for Stablebond tokens at vault (on-chain)
2. TRM Labs screens wallet, including post-deposit bad-actor check (compliance)
3. Vault burns tokens and relays redemption request to Etherfuse (on-chain / bridge)
4. Redemption order relayed to Shinhan Securities (KR) (bridge)
5. Custodian and admin sell fund assets T+1 in KRW or per institutional channels (off-chain)
6. Custodian converts USD to stablecoins (bridge)
7. Vault sends stablecoins to investor's wallet (on-chain)

> **Liquidity note:** Redemption is governed by fund's operational cycle plus FX conversion — not instantaneous. Large-scale redemption liquidity managed at fund level under Korean market rules.

---

## 8. Next Action Items

1. **Technical mapping synchronization** — Etherfuse engineering reviews data fields and establishes schema within Solana metadata structure
2. **Institutional PoC kickoff** — pilot testing to demonstrate 1:1 mint-and-redeem lifecycle with custody partners
3. **Legal & PR alignment** — prepare joint press release on regulatory-sandbox readiness through engaged counsel, synchronized with formal compliance approvals
4. **Distribution & FX scoping** — confirm per-jurisdiction investor eligibility for token distribution and FX approach (hedged or unhedged) and bearing party
