# Day 1 - History of Blockchains

## Class

Class 1: History of Blockchains

## Goal

The goal of this note was to understand why blockchains were created, why Bitcoin became important, and what computer science concepts make blockchain possible.

This was not mainly a coding class. It was a foundation class.

The main question was:

> Why do we need a currency or ledger that is not controlled by one government, bank, company, or person?

---

# 1. Why Blockchain Was Created

Blockchain became popular after people started losing trust in centralized financial systems.

One important historical background was the 2008 global financial crisis. During that time, many people saw that banks, governments, and central financial institutions had a lot of power over money and financial decisions.

The core problem was:

> If one central authority controls money, that authority can decide how much money exists, who receives support, and how the financial system behaves.

This creates trust issues.

Bitcoin introduced a new idea:

> Can we create money that no single government, bank, or company controls?

That idea led to the first major blockchain-based currency: Bitcoin.

---

# 2. Problems With Traditional Currency

Traditional currency is controlled by governments and central banks.

For India, that means the RBI and the government have influence over the money supply.

For the US, that means the Federal Reserve and the US government.

The main problem discussed in class was:

> Who gets to decide when more money should be printed?

When more money is printed, the value of existing money can decrease. This is one reason inflation happens.

Example:

If the government prints too much money, then the amount of money in the system increases. But if the amount of goods and services does not increase at the same rate, prices can rise.

So even if a person has the same salary, their purchasing power can decrease.

## Simple Example

If ₹100 could buy 10 items earlier, but later ₹100 can buy only 7 items, then the number is the same but the value has reduced.

This is why inflation matters.

---

# 3. Why Gold Became a Store of Value

Before modern currency, people used barter.

Example:

* I have milk.
* You have wheat.
* We exchange milk for wheat.

But barter does not scale well because both people must want what the other person has.

Gold became useful because it had properties that made it suitable as a store of value.

## Why Gold Worked

Gold has these properties:

1. It is scarce.
2. It is hard to produce suddenly.
3. It has global demand.
4. People have trusted it for a long time.
5. It can preserve purchasing power during inflation.
6. It is not easy for one government to create unlimited gold.

Gold does not produce income like real estate or a business, but people still value it because of trust, scarcity, and history.

---

# 4. Currency Backed by Gold

Earlier, currency was connected to gold.

The idea was:

> Instead of carrying gold directly, people could use paper currency that represented gold.

So if someone had currency, they could theoretically exchange it for gold.

But over time, currency became disconnected from gold.

Once currency is no longer backed by something scarce, the government or central bank has much more control over how much currency exists.

That creates the same problem again:

> People must trust the authority managing the currency.

---

# 5. Bitcoin as Digital Gold

Bitcoin tried to copy some properties of gold in digital form.

Gold is physical.

Bitcoin is digital.

But Bitcoin tries to have similar properties:

1. Limited supply
2. Predictable issuance
3. No single owner
4. Global transferability
5. Hard to fake
6. Public verification
7. No central government control

The class framed Bitcoin as:

> A digital version of gold that can be sent over the internet.

Bitcoin is not valuable because it is physical. It is valuable only if people collectively believe it is a useful store of value or currency.

Important distinction:

> Trust in Bitcoin is different from Bitcoin's price.

The price may go up or down. But the trust question is about whether the system works as designed.

---

# 6. What Is a Blockchain?

A blockchain is a public ledger made of blocks.

Each block contains many transactions.

These blocks are connected together in order.

That is why it is called a blockchain:

> block + chain = chain of blocks

A blockchain stores transaction history in a way that many machines can verify.

Instead of one bank maintaining the ledger, many independent machines maintain and verify it.

---

# 7. Why Blockchain Is Called a Ledger

A ledger is a record of who owns what and what transactions happened.

Example:

```txt
Kaushal has 10 BTC
Kaushal sends 1 BTC to Aman
Kaushal now has 9 BTC
Aman now has 1 BTC
```

In a bank, the bank maintains this ledger.

In Bitcoin, many independent machines maintain and verify this ledger.

This is the core shift:

> From centralized ledger to decentralized ledger.

---

# 8. Bits and Bytes

Before understanding wallets, public keys, hashing, and signatures, we need to understand how computers store data.

Computers store everything as 0s and 1s.

A bit is the smallest unit of data.

A bit can be:

```txt
0 or 1
```

A byte is a group of 8 bits.

```txt
1 byte = 8 bits
```

Everything in a computer eventually becomes bits:

* numbers
* strings
* images
* videos
* programs
* keys
* signatures
* transactions

## Simple Idea

Humans read text.

Computers store bytes.

So when we send a message like:

```txt
hello
```

the computer actually sends a sequence of bytes.

---

# 9. Binary Representation

Binary is a number system using only 0 and 1.

Humans usually use decimal, which is base 10.

Computers use binary, which is base 2.

Example:

```txt
Decimal 0 = Binary 0
Decimal 1 = Binary 1
Decimal 2 = Binary 10
Decimal 3 = Binary 11
Decimal 4 = Binary 100
Decimal 5 = Binary 101
```

In binary, each position represents a power of 2.

Example:

```txt
Binary: 101
```

This means:

```txt
1 * 2² + 0 * 2¹ + 1 * 2⁰
= 4 + 0 + 1
= 5
```

So:

```txt
101 in binary = 5 in decimal
```

---

# 10. Why Encodings Exist

Computers store bytes, but humans need readable formats.

Encoding is a way to represent data in a human-readable or system-compatible format.

Different encodings were discussed:

* ASCII
* UTF-8
* Hexadecimal
* Base64
* Base58

## Why Encoding Matters in Web3

Public keys and private keys are actually bytes.

But humans cannot easily copy and share raw bytes.

So wallets show keys and addresses using encodings such as Base58 or hexadecimal.

Example:

A Solana public key is not originally a normal string. It is bytes represented in a human-readable format, often Base58.

---

# 11. ASCII

ASCII maps characters to numbers.

Example:

```txt
A -> 65
B -> 66
a -> 97
b -> 98
```

So when a computer stores a character, it stores the number behind that character.

That number is eventually stored in binary.

## Simple Flow

```txt
Character -> Number -> Binary -> Bytes
```

Example:

```txt
A -> 65 -> binary representation -> stored in memory
```

---

# 12. Hexadecimal

Hexadecimal is base 16.

It uses:

```txt
0 1 2 3 4 5 6 7 8 9 A B C D E F
```

Hex is useful because it represents binary data more compactly.

Each hex character can represent 4 bits.

Example:

```txt
Binary: 1111
Hex: F
Decimal: 15
```

Hex is common in Ethereum.

Ethereum addresses and transaction hashes are often shown in hexadecimal format.

---

# 13. Base64

Base64 is another encoding format.

It uses uppercase letters, lowercase letters, numbers, plus sign, and slash.

It is often used to represent binary data as text.

Example use cases:

* encoding files
* encoding images
* transferring binary data in text-based systems

---

# 14. Base58

Base58 is similar in spirit to Base64 but removes confusing characters.

It removes characters that look visually similar, such as:

```txt
0 and O
I and l
```

This makes it easier for humans to copy and read.

Base58 is important in Web3 because Solana public keys are commonly shown in Base58.

## Important Point

A wallet address may look like a normal string, but internally it represents bytes.

The encoding is just the display format.

---

# 15. Hashing

Hashing converts input data into a fixed-size output.

Input can be:

* text
* file
* transaction
* block
* password
* message

Output is usually a random-looking fixed-size string.

Example:

```txt
Input: hello
Hash: random-looking fixed-size output
```

## Properties of Hashing

A good hash function has these properties:

1. Same input always gives the same output.
2. Small input change creates a very different output.
3. Output has fixed size.
4. It is one-way.
5. It is computationally hard to find the original input from the hash.
6. It is extremely hard to find two different inputs with the same hash.

## One-Way Meaning

If I hash a message, I can get the hash.

But from the hash alone, I should not be able to easily recover the original message.

This is why hashing is used for passwords.

A secure app should not store your actual password. It should store the hash of your password.

---

# 16. Hashing vs Encryption

Hashing and encryption are different.

## Hashing

Hashing is one-way.

```txt
input -> hash
```

You cannot normally reverse the hash to get the original input.

Used for:

* password storage
* data integrity
* block hashes
* transaction hashes
* proof of work

## Encryption

Encryption is reversible if you have the correct key.

```txt
plain text -> encrypted text -> plain text
```

Used for:

* hiding information
* secure communication
* protecting sensitive data

## Main Difference

```txt
Hashing cannot be reversed.
Encryption can be reversed with the correct key.
```

---

# 17. Symmetric and Asymmetric Encryption

There are two broad types of encryption:

## Symmetric Encryption

The same key is used to encrypt and decrypt.

```txt
same key -> encrypt
same key -> decrypt
```

Problem:

Both parties need the same secret key.

## Asymmetric Encryption

Two keys are used:

```txt
public key
private key
```

The public key can be shared.

The private key must remain secret.

This is the foundation for wallets and digital signatures.

---

# 18. Public Key and Private Key

A Web3 wallet is based on a public/private keypair.

## Public Key

The public key can be shared with others.

People can use it to send funds to you or verify your signatures.

## Private Key

The private key must never be shared.

It is used to sign messages and transactions.

If someone gets your private key, they can control your funds.

## Simple Rule

```txt
Public key = safe to share
Private key = never share
```

---

# 19. Wallets

A wallet is not exactly like a bank account.

A wallet is mostly a key management and signing tool.

It helps you:

1. Create or import private keys.
2. Derive public keys or addresses.
3. View balances.
4. Sign messages.
5. Sign transactions.

The wallet does not hold coins inside itself.

The blockchain stores the ledger.

The wallet proves that you are allowed to move funds by signing transactions with your private key.

## Important Mental Model

> A wallet is not an account manager. It is a signing interface.

---

# 20. Digital Signatures

A digital signature proves that a message was approved by the holder of a private key.

Example:

```txt
Message: Send 1 SOL to Aman
Private key: used to sign the message
Signature: proof that the private key approved it
Public key: used by others to verify the signature
```

The private key signs.

The public key verifies.

## Why This Matters

When you send crypto, the blockchain does not need your private key.

It only needs:

1. the transaction message
2. the signature
3. your public key

Then the network verifies:

> Was this transaction really signed by the owner of the private key?

If yes, the transaction can be accepted.

---

# 21. What Happens When You Send a Transaction

Suppose Kaushal wants to send 1 BTC to Aman.

The flow is:

```txt
1. Aman shares his public address.
2. Kaushal creates a transaction: send 1 BTC to Aman.
3. Kaushal's wallet signs the transaction using Kaushal's private key.
4. The signed transaction is sent to the blockchain network.
5. Validators/miners verify the signature.
6. If valid, the transaction is included in a block.
7. Kaushal's balance decreases.
8. Aman's balance increases.
```

The important point:

> The private key is never sent to the blockchain.

Only the signed transaction is sent.

---

# 22. How a Decentralized Blockchain Works

To create a decentralized blockchain, you need software that many people can run.

For Bitcoin, people run Bitcoin software.

These machines are connected to each other.

They receive transactions, verify them, bundle them into blocks, and maintain the ledger.

There is no single server.

Instead, many machines participate in the network.

---

# 23. Miners and Validators

In Bitcoin, miners collect transactions and propose blocks.

A miner does not get to randomly change balances.

Every transaction must have a valid signature.

If a miner creates a fake transaction, other nodes can reject it.

Example:

A miner cannot simply say:

```txt
Take 100 BTC from Kaushal and give it to me.
```

Why?

Because the miner does not have Kaushal's private key and cannot create Kaushal's valid signature.

---

# 24. Blocks

A block contains a batch of transactions.

Example:

```txt
Block 100:
- Kaushal sends 1 BTC to Aman
- Ravi sends 0.5 BTC to Neha
- Priya sends 2 BTC to Dev
```

Instead of processing every transaction separately as an isolated record, transactions are grouped into blocks.

Each new block is added after the previous block.

This forms the blockchain.

---

# 25. Block Rewards

Miners are incentivized to propose valid blocks.

In Bitcoin, when a miner successfully proposes a block, they receive a block reward.

This is how new BTC enters the system.

The class discussed that Bitcoin issuance is predictable.

Unlike government currency, where money can be printed based on central decisions, Bitcoin has programmed issuance rules.

The reward decreases over time.

This is part of Bitcoin's scarcity design.

---

# 26. Proof of Work

Proof of work is the consensus mechanism used by Bitcoin.

The question is:

> Who gets to propose the next block?

If anyone could propose blocks freely, people could spam the network or create many fake identities.

Proof of work solves this by requiring miners to solve a computationally hard puzzle.

The miner must find a value called a nonce.

The goal is to find a nonce such that the block's hash satisfies a required condition.

Example condition:

```txt
The hash must start with a certain number of zeros.
```

The only practical way to find this nonce is trial and error.

Miners keep trying different nonce values until someone finds a valid one.

---

# 27. Why Proof of Work Is Expensive

Many miners around the world are trying to solve the same puzzle.

The miner with more compute power has a higher chance of finding the solution first.

This is why Bitcoin mining uses a lot of electricity and hardware.

The work itself is not doing useful AI or scientific computation.

Its purpose is security:

> It makes attacking or rewriting the chain expensive.

---

# 28. Why Not One IP = One Vote?

A naive idea could be:

> Give every machine or IP address one vote.

But this is weak.

One person could create many machines or many identities.

This is called a Sybil problem.

Proof of work makes influence depend on computational power, not just number of fake identities.

That makes attacking the network much harder.

---

# 29. Forks

Sometimes two miners may find valid blocks at almost the same time.

Then the network may temporarily split.

Some nodes see one block first.

Other nodes see another block first.

This creates a fork.

For a short time, there may be two possible versions of the chain.

Eventually, one chain becomes longer.

Bitcoin follows the rule that the longest valid chain is accepted.

The other branch is abandoned.

---

# 30. Confirmations

Because forks can happen, one block is not always enough to consider a transaction final.

If your transaction is included in a block, and more blocks are added after it, the transaction becomes harder to reverse.

Each new block after your transaction is called a confirmation.

Example:

```txt
Transaction included in block 100
Block 101 added = 1 confirmation
Block 102 added = 2 confirmations
Block 103 added = 3 confirmations
```

For expensive transactions, people often wait for multiple confirmations.

Why?

Because rewriting the chain becomes harder as more blocks are added after your transaction.

---

# 31. Why Rewriting History Is Hard

Each block contains:

1. transactions
2. the previous block's hash
3. a nonce/proof-of-work result

If someone changes an old transaction, that block's hash changes.

Then the next block becomes invalid because it depended on the old hash.

So the attacker would need to redo proof of work for:

```txt
the changed block
+ every block after it
```

Meanwhile, the honest network keeps adding new blocks.

This makes rewriting old history computationally impractical.

---

# 32. Simple Blockchain Flow

Here is the complete simplified flow:

```txt
1. User creates transaction.
2. Wallet signs transaction using private key.
3. Signed transaction is broadcast to the network.
4. Miners/validators verify the signature.
5. Valid transactions are collected into a block.
6. Miners compete using proof of work.
7. Winning miner proposes the block.
8. Other nodes verify the block.
9. Block is added to the chain.
10. More blocks after it increase confidence/finality.
```

---

# 33. Most Important Mental Models

## Mental Model 1

A blockchain is not magic.

It is a replicated ledger maintained by many machines.

## Mental Model 2

A wallet does not store coins.

A wallet stores keys and signs transactions.

## Mental Model 3

The blockchain does not need your private key.

It only needs your public key, transaction, and signature.

## Mental Model 4

Hashing makes tampering visible.

If data changes, the hash changes.

## Mental Model 5

Proof of work makes rewriting history expensive.

## Mental Model 6

Bitcoin is digital scarcity plus public verification.

## Mental Model 7

Confirmations reduce the chance that a transaction will be reversed due to a fork.

---

# 34. Key Terms

## Blockchain

A chain of blocks containing transactions.

## Block

A group of transactions added to the ledger.

## Transaction

A signed instruction to move value or update state.

## Ledger

A record of balances and transactions.

## Public Key

A shareable key used to receive funds or verify signatures.

## Private Key

A secret key used to sign messages and transactions.

## Wallet

A tool for managing keys and signing transactions.

## Hash

A fixed-size output generated from input data.

## Encryption

A reversible way to hide data using a key.

## Digital Signature

Proof that a message was signed by a private key.

## Miner

A participant that proposes blocks in proof-of-work systems.

## Validator

A participant that verifies or proposes blocks, depending on the blockchain.

## Nonce

A number miners change repeatedly to find a valid block hash.

## Proof of Work

A system where miners must solve a hard computational puzzle to propose blocks.

## Fork

A temporary split where two possible chains exist.

## Confirmation

A block added after the block containing your transaction.

---

# 35. What I Should Be Able to Explain After This Class

After revising this note, I should be able to explain:

1. Why Bitcoin was created.
2. Why traditional currency has trust problems.
3. Why gold became a store of value.
4. Why Bitcoin is sometimes called digital gold.
5. What a blockchain is.
6. What bits and bytes are.
7. Why encodings like hex, Base64, and Base58 exist.
8. What hashing is.
9. How hashing differs from encryption.
10. What public and private keys are.
11. How digital signatures work.
12. What a wallet actually does.
13. What happens when I send a blockchain transaction.
14. What miners/validators do.
15. What proof of work is.
16. Why rewriting blockchain history is hard.
17. What forks are.
18. Why confirmations matter.

---

# 36. My One-Line Summary

Blockchain is a way for many independent machines to maintain a shared transaction ledger, where ownership is controlled by private keys, transactions are verified using signatures, and history is protected using hashes and consensus.

---

# 37. Revision Questions

Use these questions to test myself.

## Conceptual Questions

1. Why did Bitcoin emerge after distrust in centralized finance?
2. What problem does money printing create?
3. Why did gold become a trusted store of value?
4. Why is Bitcoin compared to gold?
5. What does it mean that Bitcoin has predictable supply?
6. What is a blockchain in simple words?
7. What is stored inside a block?
8. Why do we need many machines in a blockchain network?

## Computer Science Questions

1. What is a bit?
2. What is a byte?
3. Why do computers use binary?
4. What is encoding?
5. Why do public keys need encoding?
6. What is the difference between ASCII, hex, Base64, and Base58?
7. Why is Base58 useful for public keys?

## Cryptography Questions

1. What is hashing?
2. Why is hashing one-way?
3. Why does a small input change completely change the hash?
4. What is encryption?
5. What is the difference between hashing and encryption?
6. What is symmetric encryption?
7. What is asymmetric encryption?
8. What is a public key?
9. What is a private key?
10. Why should a private key never be shared?

## Wallet and Transaction Questions

1. Why is a wallet not the same as a bank account?
2. What does a wallet actually store?
3. What does it mean to sign a transaction?
4. How does the network verify a transaction?
5. Does the blockchain need my private key?
6. What happens when I send 1 BTC or 1 SOL to someone?

## Mining and Consensus Questions

1. What does a miner do?
2. Why can't a miner create fake transactions?
3. What is proof of work?
4. What is a nonce?
5. Why does proof of work require computation?
6. Why is proof of work expensive?
7. Why not just let every IP address vote?
8. What is a fork?
9. Why does the longest valid chain win?
10. Why should we wait for confirmations?

---

# 38. Things I Am Still Not Fully Clear On

I should revisit these later:

* exact math behind public/private key generation
* elliptic curve cryptography
* exact Bitcoin transaction structure
* exact difference between Bitcoin mining and Solana validation
* mempool behavior
* how transaction fees and tips are prioritized
* how Solana differs from Bitcoin at the architecture level
* how wallets derive addresses from seed phrases

These are not blockers for Day 1.

---

# 39. Day 1 Status

Status: Completed foundation class.

Next step:

Build scripts to generate:

1. an EVM wallet
2. a Solana keypair

And write the next note:

`notes/day-02-wallets-keypairs-and-signatures.md`
