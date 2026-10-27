# Data Center Operations Framework

## Overview

This project demonstrates an end-to-end operations system for managing data center environments using a structured, KPI-driven approach.

It is designed to reflect how high-performing operations teams ensure uptime, manage risk, optimize capacity, and maintain audit-ready systems.

---

## Why This Project

This project showcases how operational systems can be designed—not improvised—to manage complex environments.

It reflects a real-world approach where:

- Performance is measurable
- Processes are repeatable
- Systems are monitored continuously
- Improvements are driven by data

---

## Operating Philosophy

Operate the data center like a production system:

- Measurable
- Repeatable
- Monitored
- Preventive
- Continuously improved

---

## Core Framework (5 Pillars)

### 1. Infrastructure Reliability

Ensures uptime, redundancy, and system stability.

**KPIs:**
- Uptime %
- MTTR (Mean Time to Repair)
- MTBF (Mean Time Between Failures)

---

### 2. Capacity & Resource Planning

Optimizes rack space, power, and cooling usage.

**KPIs:**
- Rack utilization %
- Power utilization %
- Cooling utilization %
- Capacity forecast accuracy

---

### 3. Incident Management

Structured response to minimize downtime and prevent recurrence.

**Process:**
Detect → Alert → Respond → Resolve → RCA → Prevent

**KPIs:**
- Time to detect
- Time to resolve
- Repeat incident rate
- SLA compliance %

---

### 4. Compliance & Risk Control

Maintains audit readiness and operational integrity.

**Controls:**
- Access logs
- Change tracking
- Maintenance logs
- Incident documentation

---

### 5. Workflow Optimization & Automation

Improves efficiency and reduces manual operations.

**KPIs:**
- Automated task %
- Ticket backlog
- Preventive maintenance completion %
- Cost per rack

---

## System Overview

The data center operates as a closed-loop system:

Monitoring → Detection → Response → Resolution → Analysis → Prevention

Every incident feeds back into:

- Preventive maintenance
- Process improvement
- KPI optimization

---

## Dashboard (Operational Visibility)

This project includes an Excel-based KPI dashboard (`dashboard/data_center_operations_dashboard.xlsx`) designed to simulate real-world monitoring and executive reporting across six sheets:

| Sheet | Contents |
|---|---|
| Dashboard | Executive KPI tiles, operational summary, capacity by zone, trend table |
| KPI_Tracker | Monthly KPI data — uptime, MTTR, MTBF, SLA compliance, PM completion |
| Incident_Log | Full incident history with TTA, TTR, root cause, and preventive action |
| Capacity | Zone-level rack, power, and cooling utilization with dynamic risk flags |
| PM_Checklist | Preventive maintenance tasks with live completion rate formula |
| Lists | Dropdown validation lists for data entry consistency |

Dashboard metric definitions and visual requirements are documented in `dashboard/dashboard_metric_definitions.md`.

---

## Project Structure

```
data/
  incident_log_sample.csv       → Sample incident records with severity, zone, TTR, root cause
  kpi_tracker_sample.csv        → Monthly KPI data across all tracked metrics

dashboard/
  dashboard_metric_definitions.md   → Dashboard requirements, sections, visuals, and filters
  data_center_operations_dashboard.xlsx → Live Excel KPI dashboard (6 sheets)

docs/
  case_study.md                 → Full implementation case study with simulated results
  executive_summary.md          → Leadership-facing performance summary template
  incident-scenarios.md         → Three worked incident scenarios (cooling, power, network)
  interview_positioning.md      → 60-second answer, skills demonstrated, closing line
  operating_model.md            → Core roles, daily workflow, escalation matrix
  system_overview.md            → Closed-loop system model and workflow diagram

templates/
  incident_report_template.md       → Structured incident report with all required fields
  preventive_maintenance_checklist.md → Daily, weekly, and monthly maintenance checks
  root_cause_analysis_template.md   → RCA framework with timeline, corrective actions, verification
```

---

## Key Deliverables

- Excel KPI dashboard with live formulas across 6 sheets
- Incident tracking system with severity, zone, and time metrics
- Root Cause Analysis (RCA) framework
- Preventive maintenance checklist (daily / weekly / monthly)
- KPI tracking model (uptime, MTTR, MTBF, SLA, PM completion)
- Executive reporting structure
- Capacity tracking system with dynamic risk flagging
- Worked incident scenarios (cooling failure, power fluctuation, network latency)
- Interview positioning guide

---

## Example Use Case

A cooling failure in one zone triggers a monitoring alert.

- Alert is acknowledged
- Workload is redistributed
- Technician is dispatched
- Issue is resolved

Root cause analysis identifies airflow obstruction.

A preventive inspection process is implemented to eliminate recurrence.

See `docs/incident-scenarios.md` for three fully worked examples.

---

## Case Study

This project includes a full case study (`docs/case_study.md`) demonstrating:

- Implementation of a structured operations framework
- Development of KPI dashboard and reporting
- Standardization of incident management
- Introduction of preventive maintenance cycles

**Simulated Results:**
- MTTR reduced by 30%
- Repeat incidents reduced by 40%
- SLA compliance improved to 98%
- Preventive maintenance completion increased to 99%

---

## Skills Demonstrated

- Operations leadership
- Incident response management
- KPI design and tracking
- Capacity planning
- Risk and compliance control
- Process improvement
- Dashboard development
- Systems thinking

---

## Interview Positioning

> "I approach data center operations as a production system where every process is measurable, repeatable, and continuously improved. I focus on reliability, structured incident response, capacity optimization, and building systems that prevent issues before they occur."

Full interview guide including 60-second answer, skills breakdown, and closing line: `docs/interview_positioning.md`

---

## Author

Built by an operations leader with experience in production systems, inventory control, compliance, and workflow optimization, transitioning these principles into data center and infrastructure operations.


## Interactive Data Center Operations Lab (new)

Open [the browser-based lab](index.html) for illustrative KPI trends, incident response training, and capacity-risk scenarios. The lab requires no account and exports fictional CSV datasets. It complements—rather than replaces—the existing Excel workbook and project documentation.

**Community:** [Roadmap](ROADMAP.md) · [Contributing](CONTRIBUTING.md) · [Open issues](https://github.com/StiliIlist/data-center-operations-framework/issues). The GitHub Pages public site requires separate activation under repository Settings → Pages (`main` / root).

**Disclaimer:** All scenarios and companies are fictional; the lab is not affiliated with any actual data center operator. Its simplified scenarios do not substitute for real engineering, electrical safety, security, or incident-response procedures.


## Phase 2: Incident Lifecycle and RCA Lab

The interactive lab now includes fictional incident ownership, ordered stage progression (Detected → Acknowledged → Investigating → Resolved → RCA Complete → Verified), timestamp checks, root-cause documentation, corrective actions, required verification evidence, timeline review, local browser storage, reset, and CSV export.

**Training assumptions:** All example incidents are synthetic. The stage timestamp input is interpreted as UTC by convention; users must enter UTC wall-clock times. This module is a learning prototype, not a production incident system. No real system telemetry or safety-critical control is connected. A completed corrective action is not verified unless the demonstration's verification stage and evidence are recorded. Full manual browser testing is pending.


## Phase 3 — Preventive maintenance and compliance lab

The new browser module tracks five synthetic preventive-maintenance tasks, inspection owner, due date, inspection date, observation evidence, and statuses (Scheduled, Overdue, Completed, Requires action). It exposes links from three fictional incidents to associated maintenance follow-up tasks; this is a reference-only association, not automatic work-order creation or closure. Dates are evaluated against fixed demo date 2026-10-26 and all edits remain local to the browser. Completion requires inspection date and evidence. Users can reset and export the maintenance register as CSV. The displayed completion count is not a formal regulatory compliance score. Manual cross-browser testing remains pending.
