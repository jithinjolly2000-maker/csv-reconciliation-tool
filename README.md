# CSV Reconciliation Tool

A browser-based tool to **reconcile two CSV files**. Load two files (or the built-in
sample), pick a key column, and it matches records and surfaces:

- ✅ **Exact matches** — rows that agree on every compared field
- ❌ **Field mismatches** — same key, different values (shown field-by-field, A vs B)
- 🟡 **Only in A** — keys missing from file B
- 🟣 **Only in B** — keys missing from file A

…plus a **match rate** and a one-click **CSV export** of whatever view you're looking at.

> **Live tool:** https://jithinjolly2000-maker.github.io/csv-reconciliation-tool/

## 🔒 Private by design

Everything runs **100% in your browser** — the CSV parsing, matching and export are all
client-side JavaScript. **No file is ever uploaded to a server.** You can use it on real
data safely, or click **Load sample data** to see it work on a worked example (invoices
with a few deliberate amount / currency / status discrepancies and some one-sided rows).

## Why I built it

Reconciling data across sources — spotting mismatches and records that exist on one side
only — is core to the audit and controls work I do. This is a clean, reusable version of
that reconciliation step that anyone can run without installing anything.

## Features

- Drag-and-drop or file-picker upload for two CSVs
- Robust CSV parsing (quoted fields, embedded commas and newlines, BOM)
- Auto-detects a likely key column; choose which columns to compare
- Field-level mismatch highlighting (strikethrough A value, bold B value)
- Summary cards + match rate
- Export the current result view back out as CSV

## Tech

- Vanilla **HTML / CSS / JavaScript** — no frameworks, no dependencies, one `index.html`.
- Hosted free on **GitHub Pages**.

## Run locally

Open `index.html` in a browser.

---

Built by **Jithin J** · [github.com/jithinjolly2000-maker](https://github.com/jithinjolly2000-maker)
