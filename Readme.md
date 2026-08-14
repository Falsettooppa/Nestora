# Nestora

## Save Together, Achieve Together

Nestora is a decentralised community savings and financial services platform built on BOT Chain.

The platform brings traditional community savings models such as rotating contribution pools into a Web3 environment, allowing users to create and participate in savings pools, work towards financial goals, and access supported bill payment functionality.

Nestora is designed to make community-based financial activities more transparent, structured and accessible through blockchain technology.

---

## Live Application

**Live Demo:**  
https://nestora-five.vercel.app/

**GitHub Repository:**  
https://github.com/Falsettooppa/Nestora

---

## The Problem

Community savings models are widely used by individuals, students, families, friends and informal groups.

However, traditional savings groups often depend on:

- Manual record keeping
- Centralised coordinators
- Informal trust
- Limited transaction transparency
- Difficulties tracking contributions
- Separate platforms for savings and everyday payments

These limitations can make community savings difficult to manage as the number of participants grows.

Nestora addresses this by combining community savings with blockchain infrastructure.

---

## The Solution

Nestora provides a decentralised environment where users can:

- Create community savings pools
- Join existing contribution pools
- Make contributions through their connected wallet
- Participate in structured savings cycles
- Create and support goal-based funding campaigns
- Access supported bill payment functionality
- Verify blockchain transactions independently

Instead of replacing the familiar concept of community savings, Nestora provides digital infrastructure that makes the model more transparent and programmable.

---

# Core Features

## 1. Contribution Pools

Nestora allows users to create and participate in structured community savings pools.

Users can discover available pools, review pool information and participate according to the rules defined for each pool.

The underlying smart-contract infrastructure enables relevant pool operations and transactions to be processed on BOT Chain.

---

## 2. GoalFund

GoalFund provides a goal-based savings and funding model.

Instead of participating in a rotating savings pool, users can work towards a specific financial objective.

Examples include:

- Education
- Business funding
- Equipment
- Personal projects
- Community initiatives

This gives Nestora two complementary savings models:

**Community rotation** through contribution pools and  
**Goal-based funding** through GoalFund.

---

## 3. Bill Payments

Nestora also includes a Bills section for supported payment services.

This extends the platform beyond savings by connecting community finance with everyday financial activities.

The BillPayment smart contract is deployed on BOT Chain Mainnet as part of the platform's blockchain infrastructure.

---

## 4. Web3 Wallet Integration

Users connect an EVM-compatible wallet to interact with Nestora.

The connected wallet serves as the user's Web3 identity and is used to authorise blockchain transactions.

This allows users to maintain direct control over transaction signing through their own wallet.

---

# BOT Chain Integration

Nestora uses **BOT Chain Mainnet** as its blockchain infrastructure.

The application interacts with smart contracts deployed on BOT Chain for its decentralised functionality.

### BOT Chain Mainnet

| Parameter | Value |
|---|---|
| Network | BOT Chain Mainnet |
| Chain ID | 677 |
| Native Token | BOT |
| Explorer | https://scan.bohr.life/ |

---

# Mainnet Smart Contracts

The following contracts are deployed for the Nestora Mainnet deployment.

### NestoraFactory

**Contract:**  
`0x1b021caa0d4c981f4695C2cD7c5c45e8A76c34cC`

### SavingsFactory

**Contract:**  
`0xD15De4c3ec402c2Eb412d9173153f4451228434c`

### BillPayment

**Contract:**  
`0xdA4B884765483CfA5a48d121cBd6EC774c92Bd74`

These contracts provide the smart-contract infrastructure used by the Nestora application for its decentralised savings and payment functionality.

---

# Testnet Deployment

Nestora's contracts were also deployed and verified during development on BOT Chain Testnet.

The verified testnet contracts include:

1. `0x0E5D148163693A582A7e30b060471CB7AB96A37D`

2. `0xf2B774eE4d570163431fce0417d4f3A0C233270c`

3. `0xD5Da4972c7b3Ed8bCfe53328Ef200254431DE124`

4. `0x558257537429e6ff865a355249e4e310d8425691`

5. `0xF64fb0b9715EA83C5FF114e05733933A8d5b5969`

These deployments were used for testing and verification before the Mainnet deployment.

---

# How Nestora Works

```text
                    ┌─────────────────────┐
                    │       User          │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Nestora Web App   │
                    └──────────┬──────────┘
                               │
              ┌────────────────┼────────────────┐
              │                │                │
              ▼                ▼                ▼
       Contribution        GoalFund          Bills
          Pools
              │                │                │
              └────────────────┼────────────────┘
                               │
                               ▼
                       EVM Wallet
                               │
                               ▼
                    ┌─────────────────────┐
                    │  BOT Chain Mainnet  │
                    │     Chain ID 677    │
                    └──────────┬──────────┘
                               │
                               ▼
                    Nestora Smart Contracts

                    User Flow
Step 1 — Connect Wallet

The user opens Nestora and connects an EVM-compatible wallet.

Step 2 — Explore Pools

The user navigates to Contribution Pools to discover available savings pools.

Step 3 — Join or Create a Pool

Users can participate in an existing pool or create a new community savings pool.

Step 4 — Interact with the Smart Contract

When a blockchain operation is required, the user's wallet prompts them to approve the transaction.

The transaction is then processed on BOT Chain.

Step 5 — GoalFund

Users can access GoalFund to create or participate in goal-based funding.

Step 6 — Bills

Users can access supported bill payment functionality from the Bills section.

Technology Stack
Frontend
React
Vite
JavaScript
Tailwind CSS
Blockchain
Solidity
EVM-compatible smart contracts
BOT Chain Mainnet
BOT Chain Testnet
Wallet integration
Development
Node.js
npm
Git
Vercel
Project Structure
Nestora/
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── hooks/
│   │   └── ...
│   │
│   ├── public/
│   ├── package.json
│   └── ...
│
├── contracts/
│   └── ...
│
└── README.md

The exact directory structure may vary depending on the current repository version.

Running Locally
Prerequisites

Make sure you have:

Node.js 20+
npm
Git
An EVM-compatible wallet
Clone the Repository
git clone https://github.com/Falsettooppa/Nestora.git
Navigate into the frontend:
cd Nestora/frontend

cd Nestora/frontend

Install dependencies:

npm install

Start the development server:

npm run dev

Open the local application in your browser.
Environment Configuration

Create the appropriate .env file required by the application.

Example:

VITE_CHAIN_ID=677
VITE_NESTORA_FACTORY_ADDRESS=0x1b021caa0d4c981f4695C2cD7c5c45e8A76c34cC
VITE_SAVINGS_FACTORY_ADDRESS=0xD15De4c3ec402c2Eb412d9173153f4451228434c
VITE_BILL_PAYMENT_ADDRESS=0xdA4B884765483CfA5a48d121cBd6EC774c92Bd74

Use the exact environment variable names required by the current source code.

Never commit private keys, seed phrases or other sensitive credentials.

Security

Nestora uses user-controlled wallets for blockchain transactions.

Users should:

Verify transaction details before signing.
Never share private keys or seed phrases.
Verify smart-contract addresses before interacting with contracts.
Only connect wallets to trusted Nestora deployments.

The deployed contracts and their addresses are publicly verifiable on the BOT Chain explorer.

Future Development

Future versions of Nestora may include:

Additional savings models
Improved pool automation
Expanded bill payment support
More wallet integrations
Improved transaction history and analytics
Mobile-first improvements
Additional community financial tools
Deeper integration with the BOT Chain ecosystem
Hackathon Submission

Nestora was developed for the:

BOT Chain Africa Builder Challenge 2026

The project demonstrates how blockchain infrastructure can be applied to a familiar financial model — community savings — while extending the platform into goal-based funding and payments.

Deployment

Live Application:
https://nestora-five.vercel.app/

GitHub:
https://github.com/Falsettooppa/Nestora

BOT Chain Mainnet Chain ID:
677

Mainnet Contracts

NestoraFactory

0x1b021caa0d4c981f4695C2cD7c5c45e8A76c34cC

SavingsFactory

0xD15De4c3ec402c2Eb412d9173153f4451228434c

BillPayment

0xdA4B884765483CfA5a48d121cBd6EC774c92Bd74

Vision

Nestora's vision is to make community-based financial participation more accessible, transparent and programmable.

Community savings do not need to disappear in the transition to Web3.

They can evolve.

Save Together. Achieve Together.

Licence

This project is currently developed as a hackathon project.

Add an appropriate open-source licence if the repository is intended to be publicly licensed.



### One correction before you commit this


I would **not include the five Testnet contract addresses individually in the final README unless you want the development history exposed**. For a hackathon judge, the three **Mainnet contracts** are the important ones.


More importantly, your README currently needs the **exact explorer links for those three Mainnet contracts**. The five links you sent are for the Testnet contracts, so don't accidentally attach those links to the Mainnet addresses.


Also, your form says:


> **BOT Chain Mainnet Chain ID: 677**


So your README and deployed frontend should consistently use **677**, not the testnet chain ID.


If you want, I can also **:contentReference[oaicite:2]{index=2}**.