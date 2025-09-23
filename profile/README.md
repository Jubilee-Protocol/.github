# Jubilee Protocol

## A Hybrid L2/L3 Architecture for Decentralized Asset Management and Permanent Provenance

Jubilee is a hybrid Layer 2/Layer 3 protocol designed to unify Ethereum's programmability with Bitcoin's permanence. It operates as a high-performance, EVM-compatible ZK-Rollup (L2) on Ethereum while using the Bitcoin blockchain as a Layer 3 (L3) for immutable data anchoring.

This unique architecture creates a symbiotic "best-of-both-worlds" solution, enabling sophisticated DeFi applications with a dual-security proposition previously unseen in the blockchain ecosystem.

---

## Table of Contents

  - The Problem: A Foundational Compromise
  - The Solution: A Symbiotic Superstructure
  - Protocol Architecture: A Three-Layer Stack
    - L1: The Security & Settlement Layer (Ethereum)
    - L2: The Execution & Programmability Layer (Jubilee)
    - L3: The Data Finality & Archival Layer (Bitcoin)
  - Core Products: The Jubilee Asset Suite
    - jBTCi: The Jubilee Bitcoin Index
    - jETHs: The Jubilee Ethereum Staked Index
  - The $JUBL Token: Governance and Utility
  - Roadmap
  - Security and Risk Factors
  - Disclaimer

---

## The Problem: A Foundational Compromise

The decentralized web has evolved along two separate tracks:
*   **Ethereum:** The leader for smart contracts, dApps, and DeFi, offering rich programmability.
*   **Bitcoin:** The most secure and immutable ledger, serving as the ultimate store of value and digital truth.

This division forces a trade-off, leading to siloed liquidity and a fragmented security posture where developers cannot easily leverage the strengths of both networks simultaneously.

## The Solution: A Symbiotic Superstructure

The Jubilee Protocol bridges this divide by creating a multi-layered system that harmonizes both networks:
1.  It operates as a high-speed, low-cost ZK-Rollup on Ethereum (L2) for execution.
2.  It periodically anchors cryptographic hashes of its state to the Bitcoin blockchain (L3) for permanent provenance.

This allows Jubilee to offer a fast, programmable DeFi environment while anchoring critical data to the most secure ledger ever created, unlocking new forms of capital efficiency and system resilience. The protocol's development is stewarded by the non-profit **Hundredfold Foundation**.

## Protocol Architecture: A Three-Layer Stack

Jubilee's innovation lies in its hybrid, multi-layered architecture that leverages the unique strengths of each blockchain.

### L1: The Security & Settlement Layer (Ethereum)

Ethereum is the foundational layer, providing the bedrock of security and finality for the entire system.
*   **State Verification:** Jubilee's state transitions are verified on Ethereum L1 via ZK-SNARKs or ZK-STARKs, ensuring the integrity of every L2 transaction without requiring L1 re-execution.
*   **Data Availability:** Compressed transaction data is posted to Ethereum as `calldata`, guaranteeing that the L2 state is always fully recoverable.
*   **Asset Custody:** Immutable smart contracts on Ethereum manage the canonical bridges, locking assets on L1 to mint 1:1 backed assets on Jubilee.

### L2: The Execution & Programmability Layer (Jubilee)

This is the high-performance environment where all user interactions and application logic reside.
*   **EVM Compatibility:** Built using the ZK Stack, Jubilee is fully EVM-compatible, allowing developers to deploy existing Solidity contracts and use familiar tools (Hardhat, Foundry) without modification.
*   **High Throughput & Low Cost:** By processing transactions off-chain, Jubilee dramatically increases throughput and reduces costs compared to direct L1 interactions.
*   **Native Gas Token:** `jETH`, a bridged representation of ETH, is used for gas fees, aligning incentives between L1 and L2.

### L3: The Data Finality & Archival Layer (Bitcoin)

Bitcoin provides a supplementary layer for data permanence and immutable archival.
*   **Mechanism:** An off-chain service bundles hashes of L2 state and embeds them into a Bitcoin transaction using the `OP_RETURN` opcode.
*   **Function:** This creates a permanent, globally verifiable timestamp for critical data, leveraging Bitcoin's immense proof-of-work security. This acts as a "digital notary" service, which is invaluable for auditing, compliance, and high-value contracts.

## Core Products: The Jubilee Asset Suite

Jubilee is a platform for a suite of innovative, yield-generating financial products built as composable ERC-4626 tokenized vaults.

### jBTCi: The Jubilee Bitcoin Index

A decentralized index fund that holds a diversified basket of leading Bitcoin representations on Ethereum (e.g., wBTC, tBTC, jBTC). It is designed to systematically exploit minor price deviations between these assets, generating arbitrage profits that accrue to the index holders. This transforms a non-yield-bearing asset into a productive one.

### jETHs: The Jubilee Ethereum Staked Index

A diversified index of yield-bearing, liquid-staked Ethereum (LST) tokens. The value of jETHs grows from two sources:
1.  The base staking yield from the underlying LSTs.
2.  Arbitrage alpha generated by trading between LSTs when their prices deviate.

## The $JUBL Token: Governance and Utility

`$JUBL` is the native utility and governance token of the Jubilee Protocol, designed to be integral to its security, decentralization, and economic sustainability.

*   **Governance:** `$JUBL` holders can vote on critical protocol decisions within the Jubilee DAO.
*   **Staking:** The token is staked to secure the decentralized sequencer set and the jBTC bridge's TSS network. Stakers are rewarded with a share of protocol revenue and `$JUBL` emissions.
*   **Fee Discounts:** Can be used to pay for protocol fees at a discounted rate.
*   **Access to Features:** May be required to access future premium services.

### Tokenomics
*   **Total Supply:** 1,000,000,000 `$JUBL`
*   **Allocation:**
    *   **Community & Ecosystem:** 40%
    *   **Staking Rewards:** 25%
    *   **Foundation & Core Team:** 20%
    *   **Investors (Private):** 10%
    *   **Public Sale / Liquidity:** 5%

## Roadmap

The Jubilee rollout follows a phased, two-year deployment plan:

1.  **Phase 1: "Yoke" (H2 2025 - H1 2026)**
    *   **Objective:** Establish core technical infrastructure and cultivate the community.
    *   **Deliverables:** Core L2 ZK-Rollup contracts, internal audits, and private testnet launch.

2.  **Phase 2: "Harvest" (H2 2026)**
    *   **Objective:** Launch the Jubilee L2 Mainnet and introduce the `$JUBL` token.
    *   **Deliverables:** Mainnet deployment, Token Generation Event (TGE), and initial liquidity mining.

3.  **Phase 3: "Wisdom" (H1 2027)**
    *   **Objective:** Deploy the core yield-generating index products (jBTCi, jETHs).
    *   **Deliverables:** Activation of the Rebalancing Engine and the "Choice Yield" mechanism for stakers.

4.  **Phase 4: "Heritage" (H2 2027+)**
    *   **Objective:** Activate the L3 Bitcoin settlement layer and transition to full community ownership.
    *   **Deliverables:** Activation of the L3 Settlement Service and progressive decentralization of the Sequencer, Prover, and bridge networks.

## Security and Risk Factors

Security is paramount and is addressed through a multi-layered model including L1 security from Ethereum, L3 permanence from Bitcoin, economic security via `$JUBL` staking, and rigorous smart contract audits.

## Disclaimer

The Jubilee Protocol is under development, and its features, design, and implementation are subject to change. 
