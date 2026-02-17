# Industry Feature Taxonomy — Structural Pattern Extraction

**Scope:** Publicly known product capabilities and industry standards only. No internal architecture, implementation, or proprietary design.

**Format:** 6-level hierarchy — Industry → Domain → Capability Area → Feature Group → Feature → User Value

---

## 1. BigTech Platform

- **Domain:** Ecosystem & Distribution
  - **Capability Area:** Account & Access
    - **Feature Group:** Identity & Sign-in
      - Single sign-on across services | User value: One credential for all ecosystem services.
      - Federated identity linking | User value: Link external accounts without re-verification.
      - Multi-factor authentication options | User value: Stronger account protection with choice of methods.
    - **Feature Group:** Profile & Preferences
      - Unified profile across products | User value: Consistent identity and settings everywhere.
      - Consent and preference center | User value: Control how data and communications are used.
  - **Capability Area:** Distribution & Reach
    - **Feature Group:** In-app discovery
      - Cross-product promotion and recommendations | User value: Discover relevant services inside the ecosystem.
      - App/store placement and visibility | User value: Find and install trusted apps from one place.
  - **Capability Area:** Monetization & Billing
    - **Feature Group:** Billing
      - Unified billing and subscription management | User value: One place to manage all subscriptions and payments.
      - In-app purchase and digital goods | User value: Pay for content and features within the platform.
      - Usage-based billing visibility | User value: See and control spend by product or service.
- **Domain:** Data & Intelligence
  - **Capability Area:** Cross-product signals
    - **Feature Group:** Analytics & insights
      - Aggregated usage and behavior insights | User value: Understand how services are used across the ecosystem.
      - Personalization and recommendations | User value: Experiences tailored to behavior and preferences.
  - **Capability Area:** Trust & Safety
    - **Feature Group:** Safety
      - Content and conduct moderation | User value: Safer environment across products.
      - Fraud and abuse detection | User value: Reduced risk of scams and misuse.

---

## 2. FinTech Super App

- **Domain:** Multi-service aggregation
  - **Capability Area:** Core financial services
    - **Feature Group:** Payments
      - P2P and group transfers | User value: Send and split money quickly with contacts.
      - Bill payment and top-up | User value: Pay utilities and mobile in one app.
      - QR and contactless payment | User value: Pay in-store and online with one tap.
    - **Feature Group:** Accounts & storage
      - E-wallet and balance holding | User value: Keep funds ready for spending or transfers.
      - Linked bank accounts and cards | User value: Move money between bank and app seamlessly.
  - **Capability Area:** Lending & credit
    - **Feature Group:** Credit
      - BNPL and short-term credit | User value: Pay in installments without a card.
      - Credit line and overdraft | User value: Access short-term liquidity when needed.
  - **Capability Area:** Savings & investment
    - **Feature Group:** Savings
      - Savings pockets and goals | User value: Set aside and grow money for goals.
      - Automated round-up and rules | User value: Save without thinking.
    - **Feature Group:** Investment
      - Simple investment products | User value: Invest in funds or assets from the same app.
- **Domain:** Lifestyle & ecosystem
  - **Capability Area:** Non-financial services
    - **Feature Group:** Lifestyle
      - Travel, food, and ride booking | User value: Book and pay for daily services in one app.
      - Rewards and cashback aggregation | User value: Earn and redeem across partners.
    - **Feature Group:** Commerce
      - In-app marketplace and offers | User value: Shop and pay with stored balance or linked methods.

---

## 3. Traditional Banking Core

- **Domain:** Core ledger & accounts
  - **Capability Area:** Account management
    - **Feature Group:** Deposits
      - Current and savings account opening and maintenance | User value: Safe place to hold and manage money.
      - Interest and fee disclosure | User value: Clear view of earnings and charges.
    - **Feature Group:** Statements & history
      - Transaction history and search | User value: Review and search past activity.
      - Statement generation and delivery | User value: Official records for tax and reconciliation.
  - **Capability Area:** Payments execution
    - **Feature Group:** Transfers
      - Domestic wire and ACH-style transfers | User value: Move money to other banks reliably.
      - Standing orders and recurring payments | User value: Automate regular bills and transfers.
    - **Feature Group:** Cards
      - Debit and prepaid card issuance | User value: Spend from balance at POS and online.
      - Card controls and limits | User value: Set spending and geographic limits.
- **Domain:** Lending & credit
  - **Capability Area:** Credit products
    - **Feature Group:** Loans
      - Personal and mortgage loan origination | User value: Borrow for large purchases with clear terms.
      - Loan servicing and amortization | User value: Track repayments and payoff.
  - **Capability Area:** Overdraft
    - **Feature Group:** Overdraft
      - Overdraft facility and fees | User value: Avoid bounced payments when balance is short.
- **Domain:** Compliance & reporting
  - **Capability Area:** Regulatory
    - **Feature Group:** Reporting
      - Regulatory reporting and audit trail | User value: Bank meets legal obligations; customer data handled properly.
      - KYC and account verification | User value: Secure, compliant onboarding.

---

## 4. Centralized Exchange (CEX)

- **Domain:** Trading
  - **Capability Area:** Order execution
    - **Feature Group:** Order types
      - Limit, market, and conditional orders | User value: Execute strategy with chosen price and conditions.
      - Order book and depth visibility | User value: See liquidity and place informed orders.
    - **Feature Group:** Execution
      - Spot and derivatives trading | User value: Trade multiple product types in one venue.
      - Matching engine and fill reports | User value: Fast, transparent execution and confirmations.
  - **Capability Area:** Liquidity & pricing
    - **Feature Group:** Liquidity
      - Maker/taker fees and tiers | User value: Lower cost for providing liquidity or volume.
      - Price alerts and notifications | User value: React to market moves without watching constantly.
- **Domain:** Custody & funding
  - **Capability Area:** Wallets & balances
    - **Feature Group:** Balances
      - Multi-asset wallet and balance view | User value: Hold and view all assets in one place.
      - Deposit and withdrawal to external addresses | User value: Move assets in and out of the exchange.
    - **Feature Group:** Staking & earn
      - Staking and yield products | User value: Earn on idle assets.
- **Domain:** Trust & safety
  - **Capability Area:** Security & compliance
    - **Feature Group:** Security
      - Withdrawal whitelist and 2FA | User value: Reduce risk of unauthorized withdrawals.
      - Cold/hot custody disclosure | User value: Understand how assets are stored.
    - **Feature Group:** Compliance
      - KYC tiers and jurisdiction-based access | User value: Access appropriate products per regulation.

---

## 5. Web3 Wallet

- **Domain:** Key & identity
  - **Capability Area:** Key management
    - **Feature Group:** Key storage
      - Self-custody key generation and backup | User value: Own and recover access without a third party.
      - Multi-device and recovery phrases | User value: Restore wallet if device is lost.
    - **Feature Group:** Signing
      - Transaction and message signing | User value: Approve actions with controlled exposure.
      - Session keys and delegation | User value: Grant limited permissions to dApps.
  - **Capability Area:** Identity
    - **Feature Group:** Identifiers
      - ENS and address naming | User value: Human-readable addresses and identity.
      - Multiple addresses and accounts | User value: Separate use cases or privacy.
- **Domain:** Asset & dApp access
  - **Capability Area:** Assets
    - **Feature Group:** Balance & history
      - Multi-chain balance and token list | User value: See all holdings across chains.
      - Transaction history and explorer links | User value: Verify and trace activity.
    - **Feature Group:** Swaps & bridging
      - In-wallet swap and bridge | User value: Exchange and move assets without leaving wallet.
  - **Capability Area:** dApp interaction
    - **Feature Group:** Connectivity
      - dApp connect and disconnect | User value: Use apps without giving full key access.
      - Network switching | User value: Use the correct chain for each app.
- **Domain:** Security & UX
  - **Capability Area:** Safety
    - **Feature Group:** Safety
      - Phishing and scam warnings | User value: Avoid malicious sites and transactions.
      - Allowlist and spending limits | User value: Constrain what can be signed.

---

## 6. Stablecoin Issuer

- **Domain:** Issuance & redemption
  - **Capability Area:** Minting & burning
    - **Feature Group:** Issuance
      - Fiat-backed mint and burn | User value: Convert fiat to stablecoin and back at par.
      - Redemption window and minimums | User value: Clear process to exit to fiat.
  - **Capability Area:** Reserves
    - **Feature Group:** Transparency
      - Reserve attestation and reporting | User value: Trust that tokens are backed.
      - Reserve composition disclosure | User value: Understand backing assets and risk.
- **Domain:** Distribution & use
  - **Capability Area:** Access
    - **Feature Group:** On/off ramp
      - Direct or partner buy/sell | User value: Obtain or redeem stablecoins easily.
    - **Feature Group:** Integration
      - API and partner distribution | User value: Use stablecoins in third-party apps and flows.
- **Domain:** Compliance
  - **Capability Area:** Controls
    - **Feature Group:** Compliance
      - Sanctions screening and freeze | User value: Regulatory compliance and fraud mitigation.
      - Tiered limits by verification | User value: Higher limits with verified identity.

---

## 7. DEX Aggregator

- **Domain:** Routing & execution
  - **Capability Area:** Liquidity sourcing
    - **Feature Group:** Aggregation
      - Multi-DEX and AMM liquidity scan | User value: Best price across venues.
      - Split orders across venues | User value: Large orders filled with minimal slippage.
    - **Feature Group:** Routing
      - Optimal path and gas estimation | User value: See cost and route before signing.
      - MEV protection and private order flow | User value: Reduce front-running and bad execution.
  - **Capability Area:** UX
    - **Feature Group:** Comparison
      - Price comparison vs single DEX | User value: Confirm better execution.
      - Slippage and deadline controls | User value: Limit execution risk.
- **Domain:** Cross-chain
  - **Capability Area:** Bridging
    - **Feature Group:** Cross-chain swap
      - Cross-chain swap in one flow | User value: Swap across chains without manual bridge steps.
      - Bridge fee and time estimate | User value: Compare cost and delay across options.

---

## 8. AMM / DEX Protocol

- **Domain:** Liquidity & pricing
  - **Capability Area:** Pools
    - **Feature Group:** Pool types
      - Constant-product and variant pools | User value: Predictable pricing and fee structure.
      - Concentrated liquidity and ranges | User value: Capital efficiency and targeted exposure.
    - **Feature Group:** Liquidity provision
      - Add/remove liquidity and position management | User value: Earn fees by providing liquidity.
      - LP token and share representation | User value: Track and redeem pool share.
  - **Capability Area:** Swaps
    - **Feature Group:** Execution
      - Swap execution and slippage tolerance | User value: Trade with defined worst-case price.
      - Fee tiers and pool selection | User value: Choose cost vs liquidity depth.
- **Domain:** Incentives & governance
  - **Capability Area:** Incentives
    - **Feature Group:** Rewards
      - Liquidity incentives and gauges | User value: Extra yield for designated pools.
  - **Capability Area:** Governance
    - **Feature Group:** Protocol parameters
      - Fee and parameter voting | User value: Influence protocol economics and risk.

---

## 9. On/Off Ramp Provider

- **Domain:** Fiat–crypto conversion
  - **Capability Area:** Purchase & sell
    - **Feature Group:** Buy
      - Fiat-to-crypto with card or bank | User value: Enter crypto with familiar payment methods.
      - Supported assets and limits | User value: Know what can be bought and up to how much.
    - **Feature Group:** Sell
      - Crypto-to-fiat withdrawal | User value: Cash out to bank or card.
      - Quote and lock window | User value: Know rate and validity before confirming.
  - **Capability Area:** Delivery
    - **Feature Group:** Delivery
      - Send-to-wallet or custody credit | User value: Receive crypto where you choose.
      - Delivery status and receipt | User value: Confirm completion and keep record.
- **Domain:** Compliance & limits
  - **Capability Area:** Verification
    - **Feature Group:** KYC
      - Identity verification and tiers | User value: Unlock higher limits and compliance.
    - **Feature Group:** Limits
      - Per-transaction and daily limits | User value: Clear expectations and fraud protection.

---

## 10. FX & Cross-Border Remittance

- **Domain:** Conversion & transfer
  - **Capability Area:** FX
    - **Feature Group:** Rates
      - Live and locked FX rates | User value: Send at known exchange rate.
      - Multi-currency balance and hold | User value: Hold and convert when desired.
    - **Feature Group:** Transfer
      - Cross-border send to account or wallet | User value: Pay abroad without traditional wire complexity.
      - Recipient options (bank, mobile money, cash pickup) | User value: Choose how recipient gets funds.
  - **Capability Area:** Transparency
    - **Feature Group:** Cost
      - All-in fee and rate disclosure | User value: No hidden FX or fees.
      - Delivery time estimate | User value: Plan around when money arrives.
- **Domain:** Compliance & operations
  - **Capability Area:** Compliance
    - **Feature Group:** Screening
      - Sanctions and AML screening | User value: Compliant, safe corridors.
    - **Feature Group:** Purpose
      - Purpose of payment and documentation | User value: Meet regulatory requirements for large transfers.

---

## 11. RWA Issuance Platform

- **Domain:** Tokenization & lifecycle
  - **Capability Area:** Issuance
    - **Feature Group:** Asset onboarding
      - Real asset documentation and verification | User value: Trust that tokens represent real assets.
      - Token creation and distribution rules | User value: Clear terms and eligibility.
    - **Feature Group:** Lifecycle
      - Income distribution (coupons, rent) | User value: Receive yield from underlying asset.
      - Redemption and exit mechanism | User value: Exit position according to terms.
  - **Capability Area:** Secondary market
    - **Feature Group:** Trading
      - Secondary market access and liquidity | User value: Buy or sell before maturity if allowed.
      - Valuation and pricing information | User value: Understand fair value.
- **Domain:** Compliance & disclosure
  - **Capability Area:** Investor
    - **Feature Group:** Access
      - Accreditation or eligibility checks | User value: Access only products allowed by regulation.
    - **Feature Group:** Disclosure
      - Offering documents and ongoing reporting | User value: Informed investment and monitoring.

---

## 12. Government Bond Tokenization

- **Domain:** Issuance & primary market
  - **Capability Area:** Bond issuance
    - **Feature Group:** Primary issuance
      - Sovereign bond token issuance | User value: Access government debt in token form.
      - Primary auction or subscription | User value: Participate in new issuance on clear terms.
    - **Feature Group:** Terms
      - Coupon and maturity disclosure | User value: Know payment schedule and tenor.
      - Denomination and minimum size | User value: Know minimum investment and granularity.
  - **Capability Area:** Secondary & settlement
    - **Feature Group:** Trading
      - Secondary market and DvP settlement | User value: Trade and settle safely.
    - **Feature Group:** Custody & registry
      - Legal ownership and registry | User value: Legal claim on the bond and income.
- **Domain:** Compliance
  - **Capability Area:** Regulatory
    - **Feature Group:** Compliance
      - Regulatory alignment with securities law | User value: Legally compliant instrument.
      - Investor eligibility and distribution rules | User value: Only eligible investors can hold.

---

## 13. E-commerce Platform

- **Domain:** Catalog & discovery
  - **Capability Area:** Product
    - **Feature Group:** Catalog
      - Product listing and search | User value: Find products quickly.
      - Categories, filters, and recommendations | User value: Discover and compare options.
    - **Feature Group:** Content
      - Reviews, ratings, and Q&A | User value: Decide with others’ experiences.
  - **Capability Area:** Cart & checkout
    - **Feature Group:** Checkout
      - Cart and multi-step checkout | User value: Review and complete purchase in one flow.
      - Multiple payment methods | User value: Pay with preferred method.
      - Guest and saved checkout | User value: Speed for one-time or returning buyers.
- **Domain:** Fulfillment & after-sale
  - **Capability Area:** Order
    - **Feature Group:** Order management
      - Order tracking and history | User value: Know status and reorder easily.
      - Returns and refund flow | User value: Return and get refund with clear process.
  - **Capability Area:** Seller (marketplace)
    - **Feature Group:** Seller tools
      - Seller onboarding and listing tools | User value: Sell with platform reach and tools.
      - Seller payouts and settlements | User value: Get paid on schedule.

---

## 14. Merchant Payment Processor

- **Domain:** Acceptance
  - **Capability Area:** Payment methods
    - **Feature Group:** Card & alternative
      - Card present and not-present acceptance | User value: Accept cards in-store and online.
      - Alternative and local payment methods | User value: Accept preferred methods by region.
    - **Feature Group:** Experience
      - Hosted checkout and redirect | User value: Compliant, fast checkout without full integration.
      - Tokenization and saved payment methods | User value: Repeat purchases without re-entering card.
  - **Capability Area:** Settlement
    - **Feature Group:** Settlement
      - Settlement schedule and currency | User value: Predictable funding and FX.
      - Split and multi-party settlement | User value: Pay marketplace participants automatically.
- **Domain:** Risk & operations
  - **Capability Area:** Risk
    - **Feature Group:** Fraud
      - Fraud scoring and rules | User value: Fewer chargebacks and losses.
      - 3DS and strong customer authentication | User value: Comply with regulation and reduce liability.
  - **Capability Area:** Operations
    - **Feature Group:** Reporting
      - Dashboard and reconciliation | User value: Reconcile and report on transactions.
      - Dispute and chargeback handling | User value: Respond to disputes with evidence.

---

## 15. AI Agent Infrastructure

- **Domain:** Agent orchestration
  - **Capability Area:** Execution
    - **Feature Group:** Task execution
      - Task decomposition and execution | User value: Complex goals broken down and executed.
      - Tool and API invocation | User value: Agents act on external systems and data.
    - **Feature Group:** State & memory
      - Conversation and session memory | User value: Continuity across turns.
      - Context window and summarization | User value: Long interactions without losing context.
  - **Capability Area:** Safety & control
    - **Feature Group:** Guardrails
      - Output filtering and safety rules | User value: Safe, bounded behavior.
      - Human-in-the-loop and approval | User value: Critical actions require confirmation.
- **Domain:** Observability & lifecycle
  - **Capability Area:** Observability
    - **Feature Group:** Monitoring
      - Trace and latency visibility | User value: Debug and optimize agent flows.
      - Cost and token usage | User value: Control spend per agent or task.
  - **Capability Area:** Lifecycle
    - **Feature Group:** Deployment
      - Versioning and rollout | User value: Deploy and roll back safely.
      - A/B and evaluation | User value: Compare agent versions objectively.

---

## 16. Metaverse Economy Platform

- **Domain:** Virtual world & assets
  - **Capability Area:** World
    - **Feature Group:** Environment
      - Persistent world and instances | User value: Shared, persistent spaces and events.
      - Avatars and identity | User value: Represent self in the world.
    - **Feature Group:** Economy
      - Virtual currency and earn/spend | User value: Earn and spend in-world.
      - Asset ownership and transfer | User value: Own and trade virtual items.
  - **Capability Area:** Commerce
    - **Feature Group:** Marketplace
      - In-world marketplace | User value: Buy and sell assets in one place.
      - Creator monetization and royalties | User value: Creators earn from sales and reuse.
  - **Capability Area:** Interop
    - **Feature Group:** Portability
      - Cross-world or cross-platform assets | User value: Use assets across experiences where supported.
      - Interoperability standards | User value: Predictable asset and identity behavior.

---

## 17. Micropayment Network

- **Domain:** Small-value payments
  - **Capability Area:** Execution
    - **Feature Group:** Throughput
      - High-volume, low-value transactions | User value: Pay per use without high fees.
      - Batch and netting | User value: Lower cost through aggregation.
    - **Feature Group:** Settlement
      - Real-time or near-real-time settlement | User value: Instant confirmation.
      - Finality guarantee | User value: No reversal after confirmation.
  - **Capability Area:** UX & pricing
    - **Feature Group:** Pricing
      - Sub-unit and fractional pricing | User value: Pay for tiny units of value.
      - Fee cap or zero fee for micropayments | User value: Viable economics for small amounts.
  - **Capability Area:** Use cases
    - **Feature Group:** Triggers
      - Pay-per-action and streaming payments | User value: Pay as you consume.
      - Prepaid balance and top-up | User value: Control spend with a prepaid balance.

---

## 18. Payment Orchestration Layer

- **Domain:** Routing & optimization
  - **Capability Area:** Routing
    - **Feature Group:** Routing logic
      - Multi-acquirer and PSP routing | User value: Best approval and cost per transaction.
      - Fallback and retry rules | User value: Higher success rate when one path fails.
    - **Feature Group:** Optimization
      - Cost and approval optimization | User value: Lower fees and higher success.
      - Route by method, geography, or rule | User value: Control where transactions go.
  - **Capability Area:** Unification
    - **Feature Group:** API
      - Single API for multiple methods | User value: One integration for many payment options.
      - Normalized response and webhooks | User value: Consistent handling and notifications.
  - **Capability Area:** Intelligence
    - **Feature Group:** Analytics
      - Performance and cost analytics | User value: Optimize routing and cost over time.
      - Decline and error analysis | User value: Fix acceptance and routing issues.

---

## 19. Embedded Finance Provider

- **Domain:** Embedded products
  - **Capability Area:** Lending
    - **Feature Group:** Credit
      - Embedded lending at checkout | User value: Finance purchase in the same flow.
      - BNPL and installment options | User value: Pay over time without separate application.
  - **Capability Area:** Payments
    - **Feature Group:** Acceptance
      - Embedded checkout and pay-in | User value: Pay without leaving brand experience.
      - Issued cards and accounts | User value: Spend with brand-linked card or account.
  - **Capability Area:** Savings & insurance
    - **Feature Group:** Savings
      - Embedded savings or round-up | User value: Save in context of spending.
    - **Feature Group:** Insurance
      - Embedded insurance at point of sale | User value: Add coverage where relevant.
- **Domain:** Platform
  - **Capability Area:** Integration
    - **Feature Group:** APIs
      - APIs and SDKs for embedding | User value: Integrate finance without building from scratch.
    - **Feature Group:** Compliance
      - BaaS and regulated entity partnership | User value: Offer regulated products with partner license.

---

## 20. Treasury Management System

- **Domain:** Cash & liquidity
  - **Capability Area:** Visibility
    - **Feature Group:** Balances
      - Multi-bank and multi-entity balance view | User value: Single view of cash positions.
      - Cash flow forecasting | User value: Plan liquidity and funding.
    - **Feature Group:** Consolidation
      - In-house bank and netting | User value: Optimize internal flows and external transactions.
  - **Capability Area:** Execution
    - **Feature Group:** Payments
      - Bulk and batch payments | User value: Pay many counterparties efficiently.
      - Approval workflows and limits | User value: Control and audit who can pay what.
  - **Capability Area:** Investment
    - **Feature Group:** Short-term investment
      - Investment sweep and short-term instruments | User value: Earn on idle cash within policy.
      - Counterparty and limit management | User value: Stay within risk limits.
- **Domain:** Risk & reporting
  - **Capability Area:** Risk
    - **Feature Group:** Exposure
      - FX and interest rate exposure | User value: See and hedge market risk.
    - **Feature Group:** Reporting
      - Regulatory and management reporting | User value: Meet internal and external reporting needs.

---

## 21. Clearing & Settlement Network

- **Domain:** Clearing
  - **Capability Area:** Trade capture
    - **Feature Group:** Matching
      - Trade matching and confirmation | User value: Agreement on terms before settlement.
      - Novation and central counterparty | User value: Counterparty risk reduced by CCP.
  - **Capability Area:** Netting
    - **Feature Group:** Netting
      - Multilateral netting | User value: Lower settlement obligations and liquidity need.
      - Settlement obligation report | User value: Know what to deliver and when.
- **Domain:** Settlement
  - **Capability Area:** Settlement
    - **Feature Group:** Delivery
      - DvP and PvP settlement | User value: Simultaneous exchange of assets and cash.
      - Settlement finality and cut-off | User value: Certainty of finality by cut-off.
  - **Capability Area:** Liquidity
    - **Feature Group:** Liquidity
      - Liquidity facility and bridging | User value: Settle when timing mismatches exist.
      - Collateral management | User value: Pledge and manage collateral for clearing.

---

## 22. Digital Identity Platform

- **Domain:** Identity lifecycle
  - **Capability Area:** Issuance
    - **Feature Group:** Verification
      - Identity verification and document check | User value: Prove identity for access or compliance.
      - Credential issuance and storage | User value: Hold verifiable credentials for reuse.
  - **Capability Area:** Presentation
    - **Feature Group:** Sharing
      - Selective disclosure and consent | User value: Share only what is needed.
      - Verifiable presentation to relying parties | User value: Prove attributes without revealing full identity.
  - **Capability Area:** Recovery
    - **Feature Group:** Recovery
      - Recovery and account recovery | User value: Regain access after loss of device or credential.
- **Domain:** Trust & interoperability
  - **Capability Area:** Trust
    - **Feature Group:** Trust framework
      - Issuer and verifier trust framework | User value: Rely on accepted issuers and standards.
  - **Capability Area:** Interop
    - **Feature Group:** Standards
      - Interoperable standards (e.g. W3C, mDL) | User value: Use identity across ecosystems.

---

## 23. Custody Infrastructure

- **Domain:** Asset safekeeping
  - **Capability Area:** Key management
    - **Feature Group:** Key storage
      - HSM and multi-sig key storage | User value: Assets protected by institutional-grade controls.
      - Key generation and backup | User value: Keys created and recoverable under policy.
  - **Capability Area:** Operations
    - **Feature Group:** Movement
      - Withdrawal policy and whitelisting | User value: Only approved destinations can receive assets.
      - Cold and warm segregation | User value: Balance between security and operational need.
  - **Capability Area:** Multi-asset
    - **Feature Group:** Support
      - Multi-asset and multi-chain support | User value: One custody solution for many assets.
      - Staking and delegation from custody | User value: Earn yield while keeping assets in custody.
- **Domain:** Client experience
  - **Capability Area:** Reporting
    - **Feature Group:** Reporting
      - Balance and transaction reporting | User value: Full audit trail and reconciliation.
    - **Feature Group:** API
      - API for integration and automation | User value: Integrate custody into internal systems.

---

## 24. Regulatory / Compliance Infrastructure

- **Domain:** KYC/AML
  - **Capability Area:** Onboarding
    - **Feature Group:** Verification
      - Identity verification and document OCR | User value: Onboard customers with less friction.
      - Sanctions and PEP screening | User value: Block or escalate high-risk parties.
  - **Capability Area:** Ongoing
    - **Feature Group:** Monitoring
      - Transaction monitoring and alerts | User value: Detect suspicious patterns.
      - Ongoing screening and list updates | User value: Stay current with sanctions and PEP lists.
  - **Capability Area:** Reporting
    - **Feature Group:** Reporting
      - SAR/STR filing workflow | User value: Meet reporting obligations with audit trail.
      - Regulatory reporting templates | User value: Produce reports in required format.
- **Domain:** Policy & control
  - **Capability Area:** Policy
    - **Feature Group:** Rules
      - Rule engine and scenario configuration | User value: Encode and change policies without code.
    - **Feature Group:** Audit
      - Audit trail and evidence retention | User value: Demonstrate compliance to auditors and regulators.

---

## 25. Observability / Risk Platform

- **Domain:** Observability
  - **Capability Area:** Visibility
    - **Feature Group:** Metrics
      - Business and technical metrics | User value: Monitor health and performance.
      - Dashboards and alerting | User value: React to thresholds and anomalies.
  - **Capability Area:** Tracing
    - **Feature Group:** Tracing
      - Request and flow tracing | User value: Follow a transaction across systems.
      - Latency and dependency map | User value: Find bottlenecks and dependencies.
  - **Capability Area:** Logging
    - **Feature Group:** Logs
      - Centralized log search and retention | User value: Debug and investigate incidents.
      - Log correlation with traces | User value: Link logs to specific requests or flows.
- **Domain:** Risk
  - **Capability Area:** Risk signals
    - **Feature Group:** Fraud
      - Fraud and abuse detection | User value: Reduce financial and reputational loss.
    - **Feature Group:** Operational risk
      - Operational risk and outage detection | User value: Detect and respond to failures early.
  - **Capability Area:** Compliance
    - **Feature Group:** Compliance monitoring
      - Compliance drift and control monitoring | User value: Stay within policy and regulation.

---

## Taxonomy Summary

| Industry Category | Domain Count | Representative Features (sample) |
|-------------------|-------------|-----------------------------------|
| 1–25 (all) | 2–3 per category | 5–15 per category; one user value per feature |

**Conventions:**
- **Level 1:** Industry category (25).
- **Level 2:** Domain (broad capability area).
- **Level 3:** Capability area (sub-domain).
- **Level 4:** Feature group (cluster of related features).
- **Level 5:** Feature (named capability).
- **Level 6:** User value (one-line benefit; shown after `|`).

All entries are derived from publicly known product capabilities and industry standards; no implementation or proprietary design is implied.
