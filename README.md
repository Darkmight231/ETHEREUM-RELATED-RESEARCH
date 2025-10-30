# Ethereum Security Research

This repository is my public journal for analyzing protocol-level concepts, deconstructing real-world vulnerabilities, and exploring secure-by-design patterns in the EVM.

This work is part of my journey into Web3 security and my preparation for contributing to the Ethereum ecosystem.

## 🗂️ Table of Contents

### 1. 🕵️ Vulnerability Post-Mortems
A collection of deep-dive analyses into historical Ethereum hacks.

* [Analysis of the Parity Multisig Wallet Hack](./vulnerability-post-mortems/parity-wallet-hack/README.md)
* [Analysis of The DAO Reentrancy Attack](./vulnerability-post-mortems/the-dao-hack/README.md)
* *(...add more as you write them)*

### 2. 📜 EIP Analysis
Notes and security implications for key Ethereum Improvement Proposals.

* [EIP-155: Replay Protection](./eip-analysis/EIP-155.md)
* [EIP-4337: Account Abstraction](./eip-analysis/EIP-4337.md)
* *(...add more as you write them)*

### 3. 🛡️ Secure Pattern Implementations
Reference implementations of smart contract patterns that prevent common vulnerabilities.

* [Reentrancy Guard (`nonReentrant`)](./secure-patterns/reentrancy-guard/README.md)
* [Two-Step Access Control (`Ownable2Step`)](./secure-patterns/access-control/README.md)

### 4. 🚩 CTF Writeups
Solutions and explanations for common smart contract security challenges.

* [Ethernaut Solutions](./ctf-writeups/ethernaut/README.md)
* [Damn Vulnerable DeFi Solutions](./ctf-writeups/damnvulnerable-defi/README.md)
