# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a personal finance tracking system using CSV files — not a software project. There is no build system, tests, or code.

## Files

| File | Purpose |
|------|---------|
| `dashboard.html` | **Main app** — open in any browser to track bill status. Single HTML file, no install needed. |
| `bills.csv` | Source data: monthly recurring bills, revenue streams, and cash flow summary |
| `_Budget 2025 - Accounts.csv` | Source data: all financial accounts with limits, balances, and available amounts |
| `Bills/` | Empty directory, likely for storing bill documents |

## Data Structure

### bills.csv
- Tracks items by category: SYSTEM, MANDATORY, REGISTERED AGENTS, MISC, INVESTMENT
- Columns: Item, Bills, Status, Per Month, Total Limit/Debt, Due Date, Payment Method
- Payment methods reference account nicknames: DCU, Truist, NIHFCU, Langley
- Revenue sources (income rows) are intermixed with expense rows
- Monthly shortfall as of last update: ~-$1,350

### _Budget 2025 - Accounts.csv
- Columns: Account Name, Limit, Used, Available
- Account types: Cash, Checking/Savings, Investment (Fidelity, Schwab), Digital Wallets, Credit Cards, Crypto (Coinbase, Ledger), Loans

## Working with This Project

When the user asks to analyze, update, or extend this project:

- **To read/edit CSVs:** Use the Read tool directly; both files are plain CSV
- **To build a tool or script:** Prefer Python (pandas) or a Google Sheets-compatible approach
- **To add automation:** Scripts should go in a new `scripts/` folder; outputs in `output/`
- **Column math:** Totals rows exist at the bottom of each section — recalculate when rows are added/removed

## Key Business Context

- Primary income: BayHealth paycheck ($4,000 bi-weekly)
- Side income: client work, Turo car rentals
- Business entity: Born Made Bosses Business LLC (several related accounts now closed)
- Investment strategy: recurring Bitcoin and Ethereum purchases via Coinbase
- Several subscriptions are marked on-hold or canceled — do not treat as active obligations
