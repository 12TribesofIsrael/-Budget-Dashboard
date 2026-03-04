# 💰 Budget Dashboard

A personal finance dashboard for tracking monthly bills, income, and account balances — all in a single HTML file. No installation, no login, no subscription required.

## How to Use

1. Download `dashboard.html`
2. Double-click it to open in any browser (Chrome recommended)
3. That's it — no setup needed

## Features

- **Click to mark paid** — tap any bill row to toggle between DUE and PAID
- **Due This Week** — automatically shows what's coming up in the next 7 days
- **Alerts** — flags over-limit and near-limit credit cards, plus past-due bills
- **Edit Mode** — click ✏️ Edit to add, edit, or delete any bill or income source
- **Income tracking** — income sources count toward your monthly net
- **Account snapshot** — quick view of balances and credit card utilization
- **Monthly summary** — live income vs. expenses vs. net calculation
- **Auto-saves** — all status changes and edits persist in your browser automatically
- **Monthly reset** — prompts to reset all statuses at the start of each new month

## Edit Mode

Click **✏️ Edit** in the top-right corner to unlock full customization:

| Action | How |
|--------|-----|
| Edit a bill | Click any row → modal opens with all fields |
| Add a bill | Click `＋ Add to [CATEGORY]` at the bottom of any section |
| Add income | Click `＋ Add Income Source` in the Income section |
| Delete | Open a bill in the modal → click 🗑 Delete |
| Change category | Use the Category dropdown — set to 💚 INCOME to move it to income |
| Pause a bill | Set Status to ON HOLD in the modal |

## Categories

| Category | Contents |
|----------|----------|
| 🏠 MANDATORY | Mortgage, car notes, credit cards, insurance, loans, taxes |
| 💻 SYSTEM | Subscriptions and software tools |
| 🎯 MISC | YMCA, timeshare, haircuts, misc expenses |
| 👪 MARNAYSHA | Family support payments |
| 📈 INVESTMENTS | Crypto purchases (Bitcoin, Ethereum) |
| 💚 INCOME | Paychecks, client payments, Turo rental income |

## Data & Privacy

- All data is stored **locally in your browser** (localStorage) — nothing is sent anywhere
- Your CSV files (`bills.csv`, accounts CSV) are **not** included in this repo for privacy
- To back up your data: export from browser DevTools → Application → Local Storage

## Version

**V1** — March 2026
