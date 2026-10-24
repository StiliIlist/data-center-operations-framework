# Workplace Operations Command Center — Version 2

**Interactive portfolio case study: facilities budgeting, vendor evaluation, invoice reconciliation, and work-order SLA reporting.**

> **SIMULATED DATA ONLY.** All vendors, PO amounts, costs, work orders, invoices, targets, and outcomes are invented for demonstration. Not affiliated with Roblox; not proof of past employment or actual operational results.

## Modules

1. **Budget** — FY2026 illustrative $384,000 operating plan, category and monthly variances, scenario planning and CSV exports.
2. **Vendor scorecards** — 35% on-time delivery, 30% quality, 20% responsiveness, 15% cost control; action bands, editing and export.
3. **Invoice control** — synthetic PO ledger and invoice-to-PO/vendor/receipt matching; detects repeated invoice identifiers, missing POs, cross-vendor mismatches, missing receipt, payment anomalies and PO overages. PO capacity is consumed only by matched invoices in register order. Status indicates preliminary data validation, **not payment authorization or a full accounting reconciliation**.
4. **Work orders / SLAs** — priority-specific acknowledgment and closure targets, fixed evaluation date and overdue alerts. Demo target hours: Critical 1/4, High 4/24, Normal 8/72. All durations are calendar hours in UTC. Ticket closure must follow acknowledgment. Unclosed tickets can be pending or overdue.

## Run / deploy

Open `index.html` locally. Host the same static files using GitHub Pages by placing them together at the configured published location. No build step, framework, keys or server needed.

## Data governance and methodology

- Data is deterministic and entirely synthetic.
- The baseline represents full FY2026, **not actual YTD amounts**.
- Sample invoices do **not** feed the budget actuals automatically; the modules illustrate complementary management controls without implying a verified accounting integration.
- Work-order SLA analytics use an explicit fixed as-of instant, **2026-10-24 12:00 UTC**, so results are reproducible.
- Response SLA met rate uses all tracked tickets as denominator; resolution SLA met rate uses closed tickets as denominator. Open overdue counts distinct open tickets with any overdue clock.
- Duplicate IDs are detected ignoring case and whitespace normalization; duplicates are flagged after the first occurrence.
- All edits remain in the current browser's localStorage and can be reset through the **Reset demo** button in Budget.
- Browser exports are CSV; no external data transfer or login.
- Production software would require authentication, robust financial approvals, PO line items, invoice date and tax handling, event/audit history, supplier contracts and SLA exceptions such as holiday schedules.

## Interview talking point

> I designed a simulated workplace management dashboard to demonstrate how to connect budget accountability and vendor performance to internal controls and SLA-based service delivery. The framework makes exceptions visible before finance approval, highlights outstanding tickets, and documents why management action is required. The data is fictional; the controls and decision rules are my own portfolio exercise.

## Project files

`index.html`, `styles.css`, and `app.js` are a standalone static website. Works offline in modern browsers.