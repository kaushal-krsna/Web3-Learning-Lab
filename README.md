# Web3 Learning Lab

This repository is my public Web3 learning lab.

I am learning Web3 from first principles with the goal of becoming credible in wallet infrastructure, transaction systems, blockchain indexing, and trust/security tooling.

My background is in AI systems, backend workflows, reliability, auditability, and production engineering. I am not approaching Web3 as a generic beginner. I am using this repository to build a strong technical foundation and document my progress publicly.

## Goal

The goal of this repository is to build small, practical experiments that help me understand how Web3 systems actually work.

Over time, this repo will include:

* blockchain fundamentals
* wallet and keypair generation
* public/private key experiments
* message signing and verification
* EVM wallet scripts
* Solana keypair scripts
* RPC calls
* balance checkers
* transaction inspection tools
* encoding, hashing, and cryptography notes
* small CLI tools
* tests and architecture notes

## Why I Am Learning Web3

Web3 is not just about tokens or speculation.

At the engineering level, Web3 combines several important areas:

* distributed systems
* cryptography
* financial infrastructure
* security
* ownership
* identity
* transaction integrity
* public auditability
* decentralized coordination

My long-term interest is in building secure Web3 systems that help users understand wallet activity, transaction risk, approvals, asset movement, and trust signals.

## My Positioning

I am positioning myself as:

> An AI systems engineer moving into Web3, focused on wallet intelligence, transaction safety, indexing, and trust infrastructure.

This repo is the first step in that journey.

## 90-Day Direction

Over the next 90 days, I am working toward building public proof across these areas:

1. Wallet and cryptography fundamentals
2. EVM and Solana basics
3. Solana account and transaction inspection
4. Message signing and verification
5. RPC-based scripts and CLI tools
6. Anchor and Solana program development
7. EVM smart contracts
8. Web3 trust and risk tooling
9. Public documentation and technical notes

## Daily Learning Rule

Every day must produce visible proof.

That proof can be:

* a commit
* a script
* a test
* a README update
* a technical note
* an architecture diagram
* a demo screenshot
* a small working feature
* a public learning post

No invisible learning.

## Day 1 - Blockchain Fundamentals

On Day 1, I studied the history and motivation behind blockchains.

Topics covered:

* why Bitcoin was created
* problems with centralized currencies
* gold as a store of value
* Bitcoin as digital gold
* bits and bytes
* encodings such as ASCII, hex, base64, and base58
* hashing vs encryption
* symmetric vs asymmetric encryption
* public/private keypairs
* digital signatures
* how transactions are signed
* how blocks contain transactions
* how miners/validators maintain the ledger
* proof of work
* forks and confirmations

## My Current Understanding

A blockchain is a public ledger maintained by many independent machines instead of one central authority.

A wallet is not the same as a bank account. A wallet is a tool for managing keys and signing messages.

A public key can be shared with others. A private key must remain secret. When a user sends a transaction, they sign it with their private key. The network can verify the signature using the public key.

Blocks contain transactions. Miners or validators propose new blocks. In proof-of-work systems like Bitcoin, miners must solve a computational puzzle before proposing a block. This makes rewriting blockchain history extremely difficult.

## What I Am Building First

The first experiments in this repository will be:

* generate an EVM wallet
* generate a Solana keypair
* sign and verify messages
* check wallet balances using RPC
* inspect transactions
* understand account models through scripts

## Tech Stack

Initial stack:

* TypeScript
* Node.js
* viem
* @solana/web3.js
* tsx

More tools will be added as the repo grows.

## Setup

Install dependencies:

```bash
npm install
```

Run the development script:

```bash
npm run dev
```

Run TypeScript checks:

```bash
npm run typecheck
```

## Notes

Learning notes will live inside the `notes/` folder.

Each note should be written in my own words and should answer:

* what I learned
* why it matters
* what confused me
* what I need to build next

## Long-Term Projects This Repo Supports

This learning lab supports my larger Web3 roadmap, including:

* Solana Anchor Lab
* Web3 Trust Copilot
* Solana Wallet Companion
* EVM Staking Lab

This repository is the foundation layer before those larger projects.

## Status

Current phase:

```txt
Phase 1: Web3 fundamentals and proof-of-work base
```

Current focus:

```txt
Wallets, signatures, keypairs, RPC calls, and blockchain fundamentals
```

## Principle

I am not trying to rush through tutorials.

I am trying to build durable understanding through code, notes, commits, and public proof.
