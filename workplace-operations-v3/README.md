# Workplace Operations Command Center — Version 3 (Phase 1)

**Independent workplace services portfolio case study, with simulated data only.** Not affiliated with Roblox. No performance or financial results are claimed as actual employment outcomes.

## Modules
- Facilities budgeting: FY2026 illustrated operating plan, month/category variance, scenario modeling, CSV export.
- Vendor performance: weighted quality, timeliness, responsiveness and cost metrics; intervention categories.
- Invoice exception review: synthetic purchase order match, duplicate checks, vendor and receipt checks, overspend alerts.
- Work-order SLAs: priority-specific response and resolution clocks as of fixed 2026-10-24 12:00 UTC.
- **V3 Procurement & Contracts:** synthetic contract register with renewal and insurance expiration alerts; RFQ comparative sourcing (40% price, 35% quality, 25% delivery); savings comparison against prior quoted annual pricing; vendor risk signals; downloadable contracts.

## Test it
Open `index.html` in any modern browser. It uses local CSS and JS and no network requests. Select **Procurement & contracts**. Add bids, reject duplicate RFQ/vendor pairs, add a contract and see metrics update; export CSV. In Budget, **Reset demo** clears local changes across modules. No server or credentials are required.

## Management caveats
- Fully fictional organizations, events, scores, spend and dates.
- Contract figures are not automatically booked to actuals, accounts payable or PO limits. The data models illustrate management controls, not production-grade accounting.
- Prior quoted price minus contract value represents *illustrative negotiated price improvement*, not cash savings achieved.
- RFQ price comparisons assume comparable scope; evaluation is advisory, not automatic contract authorization.
- Renewal alerts use a fixed as-of of 2026-10-24, including expiry at 60 days and insurance at 30 days; expired statuses take priority.
- All changes stay in your browser via localStorage; no authentication, audit trail, live collaboration, or real vendor data.

## GitHub Pages
Publish repository `/` or copy this folder's files to a GitHub Pages source directory. The `index.html` relies on adjacent `app.js` and `styles.css`.

## Future phases
2. Team supervision/coaching. 3. Employee experience/hospitality. 4. Event operations. 5. Integrated executive analytics and controlled record relationships.