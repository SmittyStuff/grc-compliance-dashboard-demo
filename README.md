# GRC Compliance Dashboard — Demonstration

A self-contained, single-page **executive GRC compliance dashboard** that
aggregates **six program modules** — ISO 27001 Control Program, Enterprise Risk
Register, Vendor/TPRM, Internal Audit, Incident Response, and
Data-Protection/Privacy — into one board-ready view, built from a
**dashboard-as-code** data pipeline:

- **KPIs / KRIs** — six board-level indicators, each with a target, current
  value, and red-amber-green status (control coverage, overdue remediation,
  mean time-to-remediate, vendor coverage, high risks open, findings closed).
- **Module compliance breakdown** — 56 controls across 6 modules with a
  filterable, expandable table and an inline compliant/partial/missing bar.
- **Risk trend** — an inline SVG showing inherent → residual risk with a
  ~46% residual-risk reduction and a scoring-methodology note.
- **Remediation tracker** — 8 corrective-action plans with owner, due date,
  progress, and overdue flags.
- **Data pipeline (dashboard as code)** — the same rollup in **Python
  (pandas)**, **SQL**, **Bash** (scheduled orchestrator), and **PowerShell**
  (Microsoft Graph / SharePoint), plus a data-flow diagram and the KPI-tracker
  and control-status **CSV artifacts** that drive the numbers.

Control sources are the **NIST Cybersecurity Framework**, **ISO/IEC 27001**, and
the **AICPA SOC 2 Trust Services Criteria**.

## 🔗 Live demo

**https://itnet-steven-smith.github.io/grc-compliance-dashboard-demo/**

## About

All organisations, controls, metrics, and evidence are **fictional** and
included only to demonstrate methodology and deliverables.

## Tech

A single `index.html` — no build step, no dependencies. All styling and
interactivity (KPI grid, status filter, expandable module rows, code tabs, and
the inline SVG risk chart and data-flow diagram) are inline vanilla
HTML/CSS/JS, so it deploys anywhere static files are served.

## Run locally

```bash
python3 -m http.server 8080
# then visit http://localhost:8080
```

---

Part of the portfolio of Steven Smith — Information Security Consultant.
