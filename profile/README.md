<div align="center">

# Talent Index KE

**Kenya's builder community for developers who ship.**

[![Programme](https://img.shields.io/badge/Mini%20Hack-Active-e84142?style=flat-square)](https://team1-kenya-mini-hack.vercel.app)
[![Network](https://img.shields.io/badge/Network-Avalanche%20Fuji-e84142?style=flat-square)](https://docs.avax.network)
[![Sessions](https://img.shields.io/badge/Sessions-Tue%20%26%20Thu%208PM%20EAT-333?style=flat-square)](#)
[![Org](https://img.shields.io/badge/GitHub-Talent--Index-181717?style=flat-square&logo=github)](https://github.com/Talent-Index)

</div>

---

Talent Index KE is a structured builder community for Kenyan developers building real products. We run cohort programmes, IRL events, and hands-on hackathons where every session ends with something deployed — not just discussed.

Every project in this organisation started as a real problem a Kenyan developer decided to solve. A savings platform for boda boda riders. A certificate issuance system. A crypto-to-M-Pesa payment gateway. A blockchain game. These are not tutorial projects. They are products built by developers who want their code in production.

The active programme is **Mini Hack** — three cohorts, each one month long, each anchored on Avalanche C-Chain. Payments. Gaming. Agentic AI. Every graduate has a deployed product on Fuji testnet, an Avalanche Academy certification, and a demo video.

---

## Mini Hack 2026

Three cohorts. Three tracks. One blockchain.

### Cohort 1 — Payments on Avalanche
> **Status: Active**

Build a hybrid payment product that bridges M-Pesa and USDC on Avalanche C-Chain.

**What you build:** M-Pesa STK Push integrations, USDC payment contracts, hybrid payment backends, merchant dashboards

**Tech stack:** Solidity, Hardhat, ethers.js, Core Wallet, Daraja API, Ngrok, Node.js, Express

**Certifications:** Avalanche Fundamentals + Payments module on Builders Hub

**Template:** [minihack-cohort1-template](https://github.com/Talent-Index/minihack-cohort1-template)

---

### Cohort 2 — Gaming and Gamified Solutions on Avalanche
> **Status: Upcoming**

Build a game or gamified system with NFT assets, on-chain game logic, and token economies on Avalanche.

**What you build:** NFT in-game assets, ERC-20 reward tokens, on-chain leaderboards, gamified loyalty programmes, Avalanche subnet deployments

**Tech stack:** Solidity, Hardhat, ethers.js, Core Wallet, OpenZeppelin ERC-721/1155, Pinata IPFS, WebSockets, Node.js

**Certifications:** Avalanche Gaming + Token Design module on Builders Hub

**Prerequisite:** Cohort 1 completion or equivalent (Solidity basics, Hardhat, ERC-20 on Fuji)

**Template:** [minihack-cohort2-template](https://github.com/Talent-Index/minihack-cohort2-template)

---

### Cohort 3 — Agentic AI Systems on Avalanche
> **Status: Upcoming**

Build autonomous AI agents that reason about on-chain data, trigger transactions, and operate as production-ready systems on Avalanche.

**What you build:** Claude API tool-calling agents, blockchain-aware wallet advisors, RAG knowledge agents, autonomous USDC payment triggers with human-in-the-loop safety

**Tech stack:** Anthropic Claude API, Alchemy, The Graph, ethers.js, Chroma vector DB, Core Wallet, Node.js, Hardhat

**Certifications:** Avalanche AI + Agentic Systems module on Builders Hub

**Prerequisite:** Cohort 1 completion or equivalent (ethers.js, smart contract deployment, async Node.js)

**Template:** [minihack-cohort3-template](https://github.com/Talent-Index/minihack-cohort3-template)

---

## Programme details

**Sessions:** Every Tuesday and Thursday at 8:00 PM EAT on Google Meet

**Office hours:** Thursdays 6:00 PM to 7:00 PM EAT on Discord voice, before the main session

**Quest submissions:** Plug and Play platform — max 5 quests per week, Sunday midnight EAT deadline

**Certifications:** Avalanche Academy on Builders Hub — mandatory for every cohort, tracked as a primary KPI

**IRL events:**
- Night of Code — 19 June 2026, mid-cohort overnight build event
- Builders Connect — last Saturday of each month, Demo Day and graduation, attendance mandatory for certification

---

## Joining Mini Hack

When you are accepted into a cohort, you receive an invitation to this organisation. Once you accept:

**Step 1 — Fork your cohort template**

Go to your cohort template repo and click **Use this template** or **Fork**. Fork to your personal GitHub account.

**Step 2 — Clone and set up**

```bash
git clone git@github.com:YOUR-HANDLE/minihack-cohortN-template.git
cd minihack-cohortN-template
npm install
cp .env.example .env
npx hardhat compile
```

**Step 3 — Create your weekly branch**

```bash
git checkout -b week-{N}-{your-github-handle}
```

**Step 4 — Build and submit**

Open a pull request against the `main` branch of your own fork. Title format:

```
[Cohort N Week N] Your Name - Deliverable title
```

Post the PR link in `#submissions` on Discord before Sunday midnight EAT. Complete all weekly quests on Plug and Play by the same deadline.

**Step 5 — Earn your certification**

Complete the relevant Avalanche Academy module each week and upload your certificate via Plug and Play. Your Builders Hub account is Quest 1 of every cohort — create it in Week 1.

---

## Accounts to create before Week 1

| Account | Where | Required for |
|---------|-------|-------------|
| GitHub | github.com | All cohorts — use your real name |
| Avalanche Builders Hub | core.app/builders-hub | All cohorts — Quest 1, primary KPI |
| Core Wallet on Fuji | core.app | All cohorts — required wallet |
| Alchemy or Infura | alchemy.com | All cohorts — RPC access |
| Safaricom Daraja sandbox | developer.safaricom.co.ke | Cohort 1 only |
| Pinata | pinata.cloud | Cohort 2 only — IPFS for NFT metadata |
| Anthropic API | console.anthropic.com | Cohort 3 only — Claude API access |

Fuji testnet AVAX faucet: [core.app/tools/testnet-faucet](https://core.app/tools/testnet-faucet)

---

## Tools to install before Week 1

```bash
# Verify Node.js 20 LTS
node --version   # must show v20.x.x

# Verify Git
git --version

# Install Hardhat (inside your project after forking)
npm install --save-dev hardhat

# Install ethers.js
npm install ethers
```

Also install: VS Code, Postman, Core Wallet browser extension, Ngrok (Cohort 1)

---

## Assessment

All weekly deliverables are graded on five criteria:

| Criterion | Weight | What the reviewer checks |
|-----------|--------|--------------------------|
| Functionality | 35% | Features work correctly on Fuji testnet |
| Integration depth | 25% | Wallet + API + on-chain layers connected |
| Code quality | 20% | Readable, commented, tested |
| Documentation | 10% | README explains what you built and how to run it |
| Demo presentation | 10% | Live product walkthrough at Builders Connect |

**Grade bands:** Distinction 90-100% / Merit 75-89% / Pass 60-74% / Incomplete below 60%

Week 4 final project carries 40% of the overall cohort grade. Weeks 1-3 together carry 60%.

**Late submissions:** Accepted up to 48 hours after the deadline with a 20% penalty. Beyond 48 hours receives zero for that week. Three consecutive zeros results in removal from the cohort without a certificate.

---

## For existing Talent Index members

If you are already part of this org and want your project included in programme showcases and the monthly builder recognition:

Tag your repo with relevant topics — `avalanche`, `web3-kenya`, `fuji-testnet`, `mini-hack`, `m-pesa`, `solidity` — so it surfaces in searches and gets picked up by the showcase review.

Post your project in the [Builder Spotlight](https://github.com/Talent-Index/.github/discussions) discussion category. The technical lead reviews all submissions monthly.

Read [CONTRIBUTING.md](https://github.com/Talent-Index/.github/blob/main/CONTRIBUTING.md) for the full guide on structuring your project for review.

---

## Community

| Channel | Purpose |
|---------|---------|
| Discord | Primary — questions, peer help, session links, weekly digests |
| GitHub Discussions | Builder Spotlight, Announcements, Resources, Help |
| Plug and Play | Quest submissions and Avalanche Academy certificate uploads |
| Discord `#submissions` | Weekly PR submission links |
| Discord `#help` | Technical questions — include what you tried and the exact error |

Discord and all programme links: [team1-kenya-mini-hack.vercel.app](https://team1-kenya-mini-hack.vercel.app)

---

## Core team

**Joseph Njoroge (Scotch)** — Technical Lead, Mini Hack
Avalanche Technical Ambassador. Co-founder, SynchStack Solutions.
Owns the curriculum, session delivery, code reviews, and end-of-cohort reporting.

**Lavender** — Programme Lead
Owns programme strategy, partner relationships, KPI reporting to the Avalanche Foundation, and IRL event logistics.

---

## Documentation

| Resource | Link |
|----------|------|
| Programme landing page | [team1-kenya-mini-hack.vercel.app](https://team1-kenya-mini-hack.vercel.app) |
| Cohort 1 template | [minihack-cohort1-template](https://github.com/Talent-Index/minihack-cohort1-template) |
| Cohort 2 template | [minihack-cohort2-template](https://github.com/Talent-Index/minihack-cohort2-template) |
| Cohort 3 template | [minihack-cohort3-template](https://github.com/Talent-Index/minihack-cohort3-template) |
| Contributing guide | [CONTRIBUTING.md](https://github.com/Talent-Index/.github/blob/main/CONTRIBUTING.md) |
| Org Discussions | [Builder Spotlight and Announcements](https://github.com/Talent-Index/.github/discussions) |
| Avalanche Builders Hub | [core.app/builders-hub](https://core.app/builders-hub) |
| Avalanche docs | [docs.avax.network](https://docs.avax.network) |

---

<div align="center">

*Build with intent. Ship with pride.*
**Team1 Kenya | 2026**

</div>
