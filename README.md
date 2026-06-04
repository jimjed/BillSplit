# 💸 Bill Split

A standalone, client-side web application designed to make receipt splitting quick, itemized, and friction-free. Perfect as a companion tool for **Splitwise**.

🚀 **Live Link:** [https://jimjed.github.io/BillSplit/](https://jimjed.github.io/BillSplit/)

## 🚀 The Splitwise Problem This Solves

While **Splitwise** is excellent at tracking who owes whom and settling balances, it has significant pain points when dealing with single bills containing itemized details:

1. **Manual Proportional Tax & Tip Distribution**  
   If Alice orders a $10 item and Bob orders a $20 item, and the bill includes 10% tax and 20% tip, manually calculating each person's exact share of tax and tip is tedious math. This app automatically calculates the proportional tax and tip weight for every single individual.
   
2. **Visual Itemized Portion Grid (Fractional Sharing)**  
   Splitwise doesn't offer a grid interface to easily divide individual items. In this app, you can assign fractional portions (e.g., Alice had `1.5` portions, Bob had `0.5` portions, and Charlie had `0`) or custom percentage splits for every item, dynamically calculating the totals.

3. **Instant Auditing & Copy-to-Chat Text**  
   Before adding a transaction to Splitwise, friends often want to see a breakdown of exactly what they are paying for. This app generates a clean, readable text summary you can paste directly into a group chat, exports a spreadsheet-ready CSV with actual Excel formulas, and stores a persistent calculation history ledger.

4. **Zero-Setup & Offline First**  
   No signup, login, or network connection to a backend database is required. Everything runs entirely locally in your browser (including OCR scanning and offline PWA caching). You calculate the numbers locally, then enter the final figures into Splitwise.

---

## ✨ Features

- 📸 **Receipt OCR Scanner**: Take a picture of your receipt to automatically extract item names and prices locally using `Tesseract.js` (no images are uploaded to any server). Features a **Preprocessing Control Panel** (Contrast adjustment slider and text-dilation toggle) with real-time visual canvas previews, and an **Interactive Verification List** to modify, add, or delete items inline before pushing them to the ledger.
- ✏️ **Manual Matrix Grid**: Add items and assign portion weights (Count mode) or percentages (% mode) to members of your group.
- 👥 **Group Presets**: Create and save groups of friends (e.g., roommates, weekend trip) to instantly load member details without re-entering names.
- 📜 **Calculations History Ledger**: Access a persistent record of all past calculations, complete with detailed sub-pages, shareable summaries, CSVs, and deletion options.
- ☀️🌙 **Aesthetics & Dark Mode**: A responsive UI with a dark/light mode toggle.

---

## 🛠️ How to Use with Splitwise

1. Open `BillSplit.html` in any browser.
2. Load a saved group or add people manually.
3. Upload a receipt photo or enter items/prices manually.
4. Distribute the portions in the manual grid (click **Split Evenly** to divide an item equally).
5. Enter the overall **Tax ($)** and **Tip ($)**.
6. Click **Calculate**.
7. Copy the final totals for each person and add them to a single bill in **Splitwise** (or copy/paste the breakdown text to your group chat for absolute transparency).

---

## 📦 Getting Started

You can run the application in two ways:

1. **Web Version:** Access the live page directly at [https://jimjed.github.io/BillSplit/](https://jimjed.github.io/BillSplit/)
2. **Local Version:** Clone or download this repository, and open [index.html](index.html) in any web browser.
