# Workplace Operations Command Center — Version 3 (Phase 1)

**Independent workplace services portfolio case study, with simulated data only.** Not affiliated with potential employers. No performance or financial results are claimed as actual employment outcomes.

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


## V3 Phase 2 — Team performance & coaching (2026-10-24)

- Simulated four-person staff roster with capacity hours, task completion counts, quality inputs, training deadlines, development goals.
- Workstream assignment form, cumulative workload utilization calculation, per-person over-allocation warning.
- Coaching action log with focus area, next steps and follow-up date; CSV export and local reset.
- The team uses invented identities and static scenario metrics, not real personnel records or evidence of actual people management.
- Example measurement date is fixed at 2026-10-24 for deterministic results.
- Metrics are decision-support prompts, not employee evaluations or substitutes for supervisory judgment.
- LocalStorage stores demonstration edits only; avoid entering personal or sensitive data.

### Phase 2 acceptance checks

1. Assigned hours aggregate by employee and across team.
2. An assignment above capacity raises an over-allocation flag.
3. Training due dates prior to 2026-10-24 are flagged overdue.
4. Coaching logs save, render and survive local refresh.
5. Reset restores fictional sample.
6. Team CSV exports workload and quality indicators.

## Phase 3: Workplace hospitality and employee experience

The interactive dashboard adds fictional employee service requests (owner, due date, status), feedback scores and documented service-recovery actions, plus simulated amenity-readiness inspections. Low scores of 1–2 require a follow-up action. KPIs include overdue open requests, mean satisfaction among rated requests, low-score counts and amenities needing attention. Records can be edited, exported as CSV and reset using browser-local storage. Fixed evaluation date: 2026-10-24. This is a portfolio demonstration, not potential employers data or evidence of actual employee survey performance.


## Phase 4 — Event Operations & Budget Management

Adds event requests, approved budgets, fictional vendor/PO commitments, staff allocations, budget-variance and capacity warnings, closeout expenses, attendance, optional attendee feedback, CSV export and reset. The event register is simulated and persists only in browser localStorage. Fixed evaluation date: 2026-10-24. Completed-event actuals replace commitments for event exposure, rather than being added to them. Event costs do **not** automatically post to existing budget or invoice ledgers; PO identifiers are demonstrative and do not authorize expenditure. The portfolio demonstrates decision rules, not actual potential employers operations.


## Phase 5: Executive management analytics

Executive overview integrates rules-derived risk flags from annual budget modeling, vendor scorecards, contract alerts, team capacity (including planned event hours), employee requests, amenities, and event exceptions. Risks are ranked High/Medium/Low. Users can record an accountable owner, decision, due date and status, and export the exception register to CSV. Dashboard recomputes when opened. Notes are stored locally in the browser. All data and conclusions are fictional and illustrate decision controls only; events are not double-counted into operating budget actuals and invoices are not approved through the dashboard.


## Debug and release audit (2026-10-24)
- Restored and verified canonical five-module HTML source on this branch; earlier GitHub source was behind the local complete release.
- Corrected executive contract exceptions to use `Monitored` for healthy contracts.
- Corrected expired insurance / contracts severity detection to case-insensitive matching.
- Static validation: 153 HTML identifiers checked against 143 JavaScript static references, zero missing, JavaScript syntax passes.
- Interactive Chromium testing was blocked by this runtime's administrator navigation policy; browser acceptance testing and GitHub Pages setup remain pending.
- `workplace-operations-v3/index.html` is the canonical all-in-one app; all data is simulated.
