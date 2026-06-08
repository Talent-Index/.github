# Contributing to Talent Index KE

This guide covers how to contribute to projects in this organisation, whether you are an active Mini Hack cohort builder or an existing Talent Index member building independently.

---

## Mini Hack builders

### Weekly submission workflow

Every weekly deliverable follows the same process. Do not deviate from it — submissions that do not follow this format will not be reviewed.

**Step 1 — Fork the cohort template**

Fork the cohort template repository to your personal GitHub account. Do this once at the start of the cohort. Do not fork again each week.

```
https://github.com/Talent-Index/minihack-cohort1-template
```

**Step 2 — Create your weekly branch**

Branch naming is not optional. Use this exact format:

```
week-{N}-{your-github-handle}
```

Examples:
```
week-1-scotch
week-3-wanjiku
week-4-kipchoge
```

Create the branch from `main`:

```bash
git checkout main
git pull origin main
git checkout -b week-3-your-handle
```

**Step 3 — Build your deliverable**

Work on your weekly deliverable on this branch. Commit often with clear messages. Your commit history is part of your submission — it shows your process.

Good commit messages:
```
add ERC-20 contract with mint and transfer functions
fix STK Push callback handler for duplicate transactions
add unit tests for token balance and allowance
```

Bad commit messages:
```
fix
update
wip
aaa
```

**Step 4 — Open a pull request**

Open a PR against the `main` branch of your own fork (not the template repo). Use this title format:

```
[Cohort 1 Week 3] Your Name - Deliverable title
```

Fill in every section of the PR template. A PR with empty sections will not be reviewed and will receive zero for that week.

**Step 5 — Submit your PR link**

Post the PR link in the `#submissions` Discord channel before Sunday midnight EAT. Then complete all weekly quests on Plug and Play before the same deadline.

---

### Environment setup checklist

Before Week 1 Session 1, confirm all of these are done:

- [ ] Node.js 20 LTS installed (`node --version` shows `v20.x.x`)
- [ ] Git installed and configured with your real name and email
- [ ] VS Code installed
- [ ] Postman installed
- [ ] Core Wallet installed and configured on Fuji testnet
- [ ] MetaMask installed and configured on Fuji testnet
- [ ] Fuji testnet AVAX claimed from the faucet
- [ ] GitHub account created with your real name
- [ ] Avalanche Builders Hub account created at `core.app/builders-hub`
- [ ] Infura or Alchemy free tier account created
- [ ] Safaricom Daraja sandbox account created (Cohort 1 only)
- [ ] Added to the Team1Kenya GitHub org (accept the invitation email)

Fuji testnet RPC details for manual configuration:
```
Network name: Avalanche Fuji Testnet
RPC URL: https://api.avax-test.network/ext/bc/C/rpc
Chain ID: 43113
Currency symbol: AVAX
Block explorer: https://testnet.snowtrace.io
```

---

### PR template reference

When you open a PR, you will see a template. Fill in every section:

```markdown
## What I built
[Describe what you built this week in 2-4 sentences]

## What works
[List the features or components that are working correctly]

## What does not work yet
[Be honest. List anything broken, incomplete, or not yet tested]

## Live deployment
[Link to deployed frontend URL or testnet contract — required from Week 2 onwards]

## Snowtrace link
[Link to your deployed contract on Fuji testnet — required from Week 2 onwards]

## Notes for the reviewer
[Anything you want the reviewer to know before they look at your code]
```

---

### Late submission policy

Deliverables and quests are due Sunday midnight EAT.

- Up to 48 hours late: accepted with a 20% grade penalty
- Beyond 48 hours: zero for that week, but you may continue in the programme
- Three consecutive zeros: removal from the cohort without a certificate

If you have a genuine emergency, DM the technical lead before the deadline. After the deadline, late appeals are not considered.

---

### Code standards

Your code does not need to be perfect. It needs to be readable, intentional, and documented.

**Required in every submission:**

- A `README.md` that explains what you built and how to run it locally
- Environment variable examples in a `.env.example` file — never commit a `.env` file with real keys
- Comments on any logic that is not immediately obvious
- At least basic error handling — no unhandled promise rejections, no silent failures

**Solidity contracts specifically:**

- Compile without warnings before you submit
- Include at least one test file with passing tests
- Never hardcode private keys or API keys in Solidity or in any committed file

---

## Existing Talent Index members

If you are an existing member building independently, this section is for you.

### Tagging your repository

Help your project get found and featured. Add these GitHub topics to any Avalanche-related repo:

- `avalanche` — for any project built on Avalanche
- `fuji-testnet` — if deployed to Fuji
- `web3-kenya` — for all web3 projects from Kenyan builders
- `mini-hack` — if built during or inspired by a Mini Hack cohort
- `m-pesa` — for any M-Pesa integration
- `solidity` — for smart contract work

To add topics: go to your repo page, click the gear icon next to "About", and add topics there.

### README standards for existing projects

A good README makes your project discoverable, understandable, and usable by other developers. Use this structure:

```markdown
# Project Name

One sentence describing what this project does and for whom.

## The problem

What real problem does this solve? Who experiences it?

## How it works

A brief technical explanation. What is the stack? How do the components connect?

## Getting started

### Prerequisites
List what needs to be installed before this project can run.

### Installation
Step-by-step commands to get the project running locally.

### Environment variables
List every environment variable with a description. Example values where safe.

## Architecture
A diagram or written explanation of how the components connect.

## Contributing
How can another developer run tests, submit a PR, or report a bug?

## Licence
```

### Getting your project featured

Projects that get featured in the org showcase and in programme communications meet these criteria:

- Deployed to a live URL or to Fuji testnet with a verifiable contract address
- A README that someone other than the author can follow to run the project
- A demo video or screenshots showing the product working
- Clean commit history with meaningful commit messages

If your project meets these criteria, post it in the `#builder-spotlight` Discord channel. The technical lead reviews all submissions for the monthly showcase.

---

## Questions

For technical questions: post in `#help` on Discord with what you are trying to do, what you have tried, and the exact error message.

For programme questions: DM the community manager on Discord.

For unresolved technical blockers after trying `#help`: tag `@scotch` in Discord.

Office hours run every Thursday from 6:00 PM to 7:00 PM EAT on Discord voice, before the evening session.