<div align="center">

# 🔄 CSV Reconciliation Tool

### Match two CSV files · surface mismatches, exact matches & one-sided rows · export results

[![View Live Demo](https://img.shields.io/badge/▶_Try_It_Live-2d5bd7?style=for-the-badge&logoColor=white)](https://jithinjolly2000-maker.github.io/csv-reconciliation-tool/)

![Built with](https://img.shields.io/badge/Built_with-Vanilla_JS-f7df1e?style=flat-square&logo=javascript&logoColor=black)
![No dependencies](https://img.shields.io/badge/Dependencies-none-0a7a52?style=flat-square)
![Privacy](https://img.shields.io/badge/Privacy-100%25_in--browser-17854a?style=flat-square)
![Hosting](https://img.shields.io/badge/Hosted_on-GitHub_Pages-222?style=flat-square&logo=github)

</div>

---

Load two CSV files (or the built-in sample), pick a key column, and the tool reconciles them.

## ✨ What it finds

| Result | Meaning |
|--------|---------|
| ✅ **Exact matches** | Rows that agree on every compared field |
| ❌ **Field mismatches** | Same key, different values — shown field-by-field (A vs B) |
| 🟡 **Only in A** | Keys missing from file B |
| 🟣 **Only in B** | Keys missing from file A |

…plus a **match rate** and a one-click **CSV export** of whatever view you're looking at.

## 🔒 Private by design

Everything runs **100% in your browser** — the CSV parsing, matching and export are all
client-side JavaScript. **No file is ever uploaded to a server.** Use it on real data
safely, or click **Load sample data** for a worked example (invoices with deliberate
amount / currency / status discrepancies and some one-sided rows).

## 🧰 Tech

- **Vanilla HTML / CSS / JavaScript** — no frameworks, no dependencies, one `index.html`
- Robust CSV parsing (quoted fields, embedded commas & newlines, BOM)
- Auto-detects a likely key column; choose which columns to compare
- Field-level mismatch highlighting + export back to CSV
- Hosted free on **GitHub Pages**

## 💡 Why I built it

Reconciling data across sources — spotting mismatches and records that exist on one side
only — is core to the audit and controls work I do. This is a clean, reusable version of
that reconciliation step that anyone can run without installing anything.

## ▶️ Run locally

```bash
start index.html      # Windows — no build step
```

<div align="center">

---

**Built by Jithin J** · [GitHub](https://github.com/jithinjolly2000-maker) · [LinkedIn](https://www.linkedin.com/in/jithin2k)

</div>
