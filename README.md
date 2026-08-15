# Nestora

## Save Together, Achieve Together

Nestora is a decentralised community savings and financial services platform built on **BOT Chain**.

It brings familiar community savings models such as rotating contribution pools into a Web3 environment, allowing users to create and participate in savings pools, work towards financial goals, and access bill payment functionality from one platform.

Nestora combines community savings, smart contracts and blockchain infrastructure to provide a more transparent and programmable approach to group savings.

---

## Live Application

**Live App:**  
https://nestora-five.vercel.app/

**GitHub Repository:**  
https://github.com/Falsettooppa/Nestora

---

# The Problem

Community savings models such as Ajo, Esusu and rotating savings groups are widely used across Africa.

However, many of these systems still depend on:

- Manual record keeping
- Centralised coordinators
- Informal trust between participants
- Difficulty tracking contributions
- Limited transaction transparency
- Separate platforms for different financial activities

As these groups grow, managing contributions, participants and distributions can become increasingly difficult.

---

# The Solution

Nestora provides blockchain-powered infrastructure for community savings.

Users can:

- Create contribution pools
- Explore and join existing pools
- Make contributions through their connected wallet
- Participate in structured savings cycles
- Create and participate in goal-based funding
- Access supported bill payment functionality
- Verify blockchain transactions on BOT Chain

The goal is not to replace the community savings model people already understand, but to provide better infrastructure for managing it.

---

# Core Features

## Contribution Pools

Contribution Pools are the core savings functionality of Nestora.

Users can create or join structured community savings pools and participate according to the rules defined by each pool.

The pool infrastructure is powered by smart contracts deployed on BOT Chain.

---

## GoalFund

GoalFund provides a goal-based funding model.

Instead of participating in a rotating savings pool, users can work towards a specific financial target.

Examples include:

- Education
- Business funding
- Equipment
- Personal projects
- Community initiatives

This gives Nestora two complementary savings models:

**Contribution Pools** — save together with a community.

**GoalFund** — work towards a specific financial goal.

---

## Bill Payments

Nestora also includes a Bills section for supported payment services.

This extends the platform beyond savings and allows users to access financial utility from the same ecosystem.

Nestora's BillPayment smart contract is deployed on BOT Chain Mainnet.

---

## Web3 Wallet

Users connect an EVM-compatible wallet to interact with Nestora.

The connected wallet acts as the user's Web3 identity and is used to authorise blockchain transactions.

Users maintain control of their wallet and approve transactions directly before they are submitted to the blockchain.

---

# BOT Chain Integration

Nestora is built and deployed on **BOT Chain**.

The platform uses BOT Chain smart contracts to provide the blockchain infrastructure for its savings and payment functionality.

Relevant blockchain interactions are signed by the user's wallet and processed on-chain.

This provides publicly verifiable transaction records and removes the need to rely solely on a centralised database for blockchain-based operations.

### BOT Chain Network

| Parameter | Value |
|---|---|
| Network | BOT Chain Mainnet |
| Chain ID | 677 |
| Native Token | BOT |
| Explorer | https://scan.bohr.life/ |

---

# Mainnet Smart Contracts

Nestora has three primary smart-contract deployments on BOT Chain Mainnet.

## NestoraFactory

```text
0x1b021caa0d4c981f4695C2cD7c5c45e8A76c34cC

SavingsFactory
0xD15De4c3ec402c2Eb412d9173153f4451228434c
BillPayment
0xdA4B884765483CfA5a48d121cBd6EC774c92Bd74

These contracts form the main blockchain infrastructure behind Nestora's savings and payment functionality.

Testnet Deployment

During development and testing, Nestora's contracts were also deployed and verified on BOT Chain Testnet.

The verified testnet deployments include:

0x0E5D148163693A582A7e30b060471CB7AB96A37D
0xf2B774eE4d570163431fce0417d4f3A0C233270c
0xD5Da4972c7b3Ed8bCfe53328Ef200254431DE124
0x558257537429e6ff865a355249e4e310d8425691
0xF64fb0b9715EA83C5FF114e05733933A8d5b5969

These deployments were used during development and testing before the Mainnet deployment.

How Nestora Works
                    ┌─────────────────────┐
                    │        User         │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Nestora Web App   │
                    └──────────┬──────────┘
                               │
             ┌─────────────────┼─────────────────┐
             │                 │                 │
             ▼                 ▼                 ▼
      Contribution          GoalFund           Bills
         Pools
             │                 │                 │
             └─────────────────┼─────────────────┘
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
1. Connect Wallet

The user opens Nestora and connects an EVM-compatible wallet.

2. Explore Pools

The user navigates to Contribution Pools and views available savings pools.

3. Join or Create a Pool

The user can participate in an existing pool or create a new community savings pool.

4. Make a Blockchain Transaction

When an operation requires blockchain interaction, the user's wallet prompts them to approve the transaction.

The transaction is then processed on BOT Chain.

5. GoalFund

Users can create or participate in goal-based funding through GoalFund.

6. Bills

Users can access supported bill payment functionality through the Bills section.

Technology Stack
Frontend
Next.js 15
React 19
Tailwind CSS
JavaScript
Web3
Solidity
Wagmi
Viem
Ethers.js
EVM-compatible wallets
BOT Chain
Backend and Data
Next.js
MongoDB
Deployment
Vercel
BOT Chain Mainnet
Getting Started
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

Install dependencies:

npm install
Environment Variables

Create a .env.local file in the frontend directory.

The application requires the environment variables defined by the project configuration.

Example:

VITE_CHAIN_ID=677
VITE_NESTORA_FACTORY_ADDRESS=0x1b021caa0d4c981f4695C2cD7c5c45e8A76c34cC
VITE_SAVINGS_FACTORY_ADDRESS=0xD15De4c3ec402c2Eb412d9173153f4451228434c
VITE_BILL_PAYMENT_ADDRESS=0xdA4B884765483CfA5a48d121cBd6EC774c92Bd74

Use the exact environment variable names required by the current application configuration.

Never commit private keys, seed phrases or other sensitive credentials.

Run Locally

Start the development server:

npm run dev

The application will normally be available at:

http://localhost:3000
Build for Production
npm run build

Start the production server:

npm run start
Security

Nestora uses user-controlled wallets for blockchain transactions.

Users should:

Verify transaction details before signing.
Never share private keys or seed phrases.
Verify smart-contract addresses before interacting with contracts.
Only use trusted Nestora deployments.

Smart-contract addresses are publicly available so that users and reviewers can independently verify the deployed contracts.

Why Nestora?

Community savings already work because people understand the concept of contributing together towards financial goals.

The challenge is providing infrastructure that makes these systems easier to manage, more transparent and more programmable.

Nestora combines:

Community Savings + Smart Contracts + Web3 + Payments

The platform keeps the familiar savings experience while using blockchain technology to provide verifiable infrastructure underneath it.

Target Users

Nestora is initially designed for:

Students
Friends and family savings groups
Young professionals
Informal savings communities
Small community organisations
Individuals working towards financial goals
Web3 users interested in decentralised financial applications
Future Development

Potential future improvements include:

Additional community savings models
More automated pool management
Expanded bill payment services
Improved transaction history
Savings analytics
Additional wallet integrations
Mobile optimisation
More financial utilities
Deeper BOT Chain ecosystem integrations
BOT Chain Africa Builder Challenge 2026

Nestora was developed for the BOT Chain Africa Builder Challenge 2026.

The project demonstrates how blockchain infrastructure can be applied to an existing and familiar financial practice — community savings — while extending the experience into goal-based funding and payments.

Project Links

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

Nestora aims to make community-based financial participation more accessible, transparent and programmable.

Community savings do not have to disappear as financial technology evolves.

They can evolve with it.

Save Together. Achieve Together.


### One correction I deliberately made


I changed the stack from the previous README to **Next.js 15 + React 19**, because your actual `package.json` confirms:


```text
next: 15.5.21
react: ^19.0.0
