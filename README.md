# Turbin3 Enrollment Prerequisites (TS & Rust)

This repository contains the TS & Rust code developed as part of the Turbin3 Builders Cohort enrollment prerequisites. The project is an essential part of the assessment.

---

## Project Overview

The core purpose of this TS & Rust code is to:
1.  **Generate a new Solana keypair**
2.  **Request and claim devnet SOL tokens**
3.  **Perform native Solana token transfers**
4.  **Empty the development wallet** 
5.  **Interact with the Turbin3 enrollment dApp & miniting NFT**

## 📦 Prerequisites

- [Rust](https://www.rust-lang.org/tools/install)
- [Node.js](https://nodejs.org/)
- [Yarn](https://yarnpkg.com/)

## TypeScript Workflow (airdrop)

### Setup

Navigate to the directory and install dependencies:

```bash
cd airdrop
yarn install

```
```bash
yarn keygen
yarn airdrop
yarn drain-wallet
```

### Generate Client
Before running the main scripts, generate the TypeScript client from the program's Interface Description Language (IDL):

```bash 
yarn generate-client
```

### Enroll

The enroll command handles both initialization and the final submission:

```bash
yarn enroll
```

## Rust Workflow (airdrop2)

### setup

```bash
cd airdrop2
```

```bash
cargo test keygen -- --nocapture
cargo test claim_airdrop -- --nocapture
cargo test transfer_sol -- --nocapture
```

### Enroll

```bash
cargo test submit_rs -- --nocapture
```
