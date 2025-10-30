# Ethereum Upgrade Roadmap (Post-Merge)

This document summarizes the major Ethereum upgrades since the transition to Proof-of-Stake, outlining the key EIPs (Ethereum Improvement Proposals) and their impact on the network.

# 1. The Merge (Paris Upgrade)

Date: September 15, 2022

Consensus Layer: Paris

Execution Layer: Bellatrix

## What Happened:

The Merge marked the official transition of Ethereum's consensus mechanism from Proof-of-Work (PoW) to Proof-of-Stake (PoS). This was achieved by merging the original Execution Layer (Mainnet) with the new PoS Consensus Layer (the Beacon Chain).

## Key Changes:

Energy Reduction: Network energy consumption dropped by ~99.95%.

Mining Ended: Mining was replaced by validators who stake ETH to create and validate new blocks.

Block Time: Block times became stable at ~12 seconds.

Finality: The concept of "finality" was introduced. Blocks are now considered finalized after ~2 epochs (approx. 12.8 minutes), making chain reorganizations extremely unlikely.

No Gas Fee Reduction: Contrary to common misconception, The Merge did not reduce gas fees or increase transaction throughput.

# 2. Shanghai/Capella Upgrade

Date: April 12, 2023

Execution Layer: Shanghai

Consensus Layer: Capella

## What Happened:

This was the first major upgrade after The Merge, primarily focused on enabling validator withdrawals.

## Key Changes:

Staking Withdrawals (EIP-4895): For the first time, validators could withdraw their staked ETH (both partial and full withdrawals). This de-risked staking and led to a surge in participation and the growth of Liquid Staking Protocols (LSPs) like Lido and Rocket Pool.

Gas Cost Reductions: Several EIPs were included to reduce gas costs for developers in specific scenarios:

EIP-3651: Warm COINBASE (reduces cost for builders).

EIP-3855: PUSH0 Opcode (introduces a new, gas-efficient opcode for pushing 0 onto the stack).

EIP-3860: Limit and meter initcode (limits max initcode size).

# 3. Dencun Upgrade (Proto-Danksharding)

Date: March 13, 2024

Execution Layer: Cancún

Consensus Layer: Deneb

## What Happened:

The Dencun upgrade was a massive step forward for Layer 2 scaling, introducing "Proto-Danksharding."

## Key Changes:

Proto-Danksharding (EIP-4844): This EIP introduced "blobs" (Binary Large Objects).

Blobs are a new, separate, and temporary data space for rollup (L2) transactions.

Data in blobs is not stored in the EVM state forever; it is pruned after ~18 days.

This separates L2 data from L1 computation, creating a new fee market and drastically reducing L2 transaction costs.

Impact: Layer 2 fees on rollups like Arbitrum, Optimism, and Base dropped by up to 90%, making them highly competitive.

Other Improvements: Included various other EIPs for efficiency and security, such as EIP-1153 (Transient Storage Opcodes) and EIP-6780 (restricting SELFDESTRUCT).

# 4. Pectra Upgrade (Upcoming)

Planned: Late 2024 / Early 2025

Execution Layer: Prague

Consensus Layer: Electra

This upcoming upgrade is focused on improving validator economics and user experience (UX) through Account Abstraction.

## Expected Inclusions:

EIP-7251: Increases the max effective balance for a validator from 32 ETH to 2,048 ETH. This will allow large staking providers to consolidate their validators, reducing the total number of validators on the network and decreasing network overhead.

Account Abstraction (EIP-3074 / EIP-7702): These EIPs aim to give regular Externally Owned Accounts (EOAs) smart contract-like capabilities, such as transaction batching and sponsored transactions, without forcing users to migrate to a new smart contract wallet.

Staking UX: Improvements to the staking and withdrawal process.

Future: Verkle Trees

Timeline: Likely after Pectra.

What it is: A major data structure upgrade that will replace the current Merkle Patricia Trees. Verkle Trees will allow for much more efficient state proofs, which is a critical step toward enabling stateless clients and further improving network scalability.
