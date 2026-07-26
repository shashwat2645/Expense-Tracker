# 💸 EX.TRACK — Expense Tracker

A **zero-dependency, single-file** expense tracker that runs entirely in your browser. No server, no database, no installation needed — just open `expense-tracker.html` and start tracking.

---

## ✨ Features

- ➕ Add **income & expense** transactions with description, amount, category, date, and note
- 📊 Live **summary cards** — Total Income, Total Expenses, Net Balance
- 📉 **Category breakdown chart** with animated progress bars (top 6 categories)
- 🔍 **Search & filter** transactions — All / Income / Expense
- 📅 Transactions **grouped by date**
- 💱 **Multi-currency** support — ₹, $, €, £ (preference is saved)
- 🔔 **Toast notifications** on every action
- 🗑️ Delete individual transactions (with confirmation)

### 💾 Data Management
| Feature | Description |
|---|---|
| 🟢 Auto-save | Every change is instantly saved to browser localStorage |
| ⬇️ Backup JSON | Download a full `.json` backup file with one click |
| ⬆️ Restore JSON | Re-import your backup — safely merges without duplicates |
| ⬇️ Export CSV | Export all transactions for Excel / Google Sheets |
| 🗑️ Clear All | Wipe all data with a confirmation prompt |

---

## 🚀 Getting Started

**No installation. No server. No setup.**

1. Download or clone this repo
2. Open `expense-tracker.html` in any browser
3. Start tracking!

```bash
git clone https://github.com/shashwat2645/expense-tracker.git
cd expense-tracker
# Then just open expense-tracker.html in your browser
```

> ✅ Works in Chrome, Firefox, Edge, Safari — any modern browser.

---

## 📁 Project Structure

```
expense-tracker/
└── expense-tracker.html    # The entire app — HTML + CSS + JS in one file
```

That's it. One file.

---

## 🖥️ Preview

### Dashboard
- Three stat cards at the top showing Income, Expenses, and Net Balance in real time
- Color-coded: green for income, red for expenses, blue for balance

### Add Transaction
- Toggle between **Income** and **Expense**
- Pick from 12 categories: Food & Dining, Transport, Shopping, Entertainment, Health, Bills & Utilities, Education, Travel, Salary, Freelance, Investment, Other
- Select your currency (saved automatically)

### Transaction List
- Grouped by date, newest first
- Category icon + color for every transaction
- Live search across description and category
- Filter by All / Income / Expense

---

## 💾 How Data is Saved

All data is stored in your browser's **localStorage** under the keys:
- `extrack_txns` — array of all transactions
- `extrack_settings` — preferences like currency

> ⚠️ localStorage is browser-specific. If you clear browser data or switch browsers, your data will be lost. Use the **Backup JSON** feature regularly to keep a safe copy.

### Backup & Restore Workflow

**To back up:**
1. Click **⬇ Backup JSON** in the Data Management section
2. A `.json` file is downloaded to your computer — keep it safe!

**To restore:**
1. Click **⬆ Restore from JSON**
2. Select your backup file
3. Transactions are merged — no duplicates created

---

## 📦 Categories

| Category | Emoji |
|---|---|
| Food & Dining | 🍽 |
| Transport | 🚗 |
| Shopping | 🛍 |
| Entertainment | 🎮 |
| Health | 💊 |
| Bills & Utilities | ⚡ |
| Education | 📚 |
| Travel | ✈️ |
| Salary | 💼 |
| Freelance | 💻 |
| Investment | 📈 |
| Other | 📦 |

---

## 🎨 Tech Details

- **Pure HTML/CSS/JS** — no frameworks, no build tools, no npm
- **Google Fonts** — Syne (headings) + DM Mono (body) loaded via CDN
- **localStorage API** for persistent data storage
- **Blob API** for JSON and CSV file downloads
- **FileReader API** for JSON import/restore
- Dark theme with CSS variables throughout

---

## 🔒 Privacy

All your data stays **100% on your device**. Nothing is sent to any server. There are no analytics, no tracking, no external API calls (except loading Google Fonts).

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first.

1. Fork the repo
2. Create your branch: `git checkout -b feature/my-feature`
3. Commit: `git commit -m 'Add my feature'`
4. Push: `git push origin feature/my-feature`
5. Open a pull request

