# Scotty Pumpkin (SPUMP) — Token Creation & Program Interaction

## Overview

The **Scotty Pumpkin (SPUMP)** token was created on Solana by interacting with the **official SPL Token Program**, a deployed on-chain smart contract that governs token minting, transfers, and supply management.

This repository does **not contain or deploy the SPL Token Program itself**. Instead, it documents the token created by interacting with that program via Solana SDKs.

---

## Token Details

* **Project Name:** Scotty Pumpkin
* **Token Symbol:** SPUMP
* **Mint Address:** `mint address`

---

## SPL Token Program (Smart Contract)

The SPUMP token was created by interacting with the **SPL Token Program**, which is a core Solana system program responsible for fungible token logic.

* **Program Name:** SPL Token Program (Legacy)
* **Program ID:** `TokenkegQfeZyiNwAJbNbGKPFXCWuBvf9Ss623VQ5DA`
* **Source Repository (Reference Only):**
  https://github.com/solana-labs/solana-program-library

---

## Important Clarification

This repository:

* Does NOT contain the SPL Token smart contract code
* Does NOT deploy or modify the SPL Token Program
* Does NOT own or control the SPL Token Program

Instead:

* ✔ The SPUMP token was created by calling instructions on the deployed SPL Token Program
* ✔ Token minting was performed using official Solana SDKs (e.g., `@solana/spl-token`)
* ✔ The SPL Program is an external, immutable on-chain program maintained by the Solana ecosystem

---

## SPL Program Status (Reference Context)

The Solana Program Library (SPL) is a collection of on-chain programs deployed on Solana. The SPL repository has been modularized into separate program repositories under the `solana-program` organization.

Key programs include:

* SPL Token
* Token-2022
* Associated Token Account
* Memo Program
* Stake Pool
* Governance Programs

Only a subset of these programs are deployed on mainnet and actively maintained.

---

## Program Interaction Model

The SPUMP token lifecycle was created through interaction with the SPL Token Program:

1. **Mint Creation**

   * A new mint account was initialized via SPL instructions

2. **Token Supply Management**

   * Mint authority controls supply issuance

3. **Transfers**

   * Standard SPL transfer instructions govern token movement

4. **Account Management**

   * Token accounts (ATAs) store balances per wallet

---

## Security & Responsibility Disclaimer

* The SPL Token Program is an independent, audited, and widely used Solana system program.
* It is **not owned, deployed, or controlled** by the Scotty Pumpkin project.
* All token logic execution occurs on-chain within the SPL Program.

Users should understand that:

* The SPL Token Program is external infrastructure
* This repository only represents a token created using that infrastructure
* Smart contract execution and security are handled by Solana protocol-level programs

---

## Conclusion

The **Scotty Pumpkin (SPUMP)** token exists as a result of interacting with the Solana **SPL Token Program**, a core on-chain smart contract system.

This repository documents the token and its metadata, but does not contain or manage the underlying SPL smart contract implementation.

---
