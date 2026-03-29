---
date: 2026-03-25
type: github-discovery
tags: [business-analyst, automation, github, tools]
---

# 🛠️ BA Tool of the Day — 2026-03-25

## Repository
- **Name:** ydata-profiling
- **GitHub URL:** https://github.com/ydataai/ydata-profiling
- **Stars:** ⭐ 13,400+
- **License:** MIT
- **Last Updated:** 2026-03

## What It Does
ydata-profiling is a Python library that generates comprehensive exploratory data analysis (EDA) reports from any pandas or Spark DataFrame with a single line of code. It goes far beyond `df.describe()` — producing interactive HTML reports with statistics, visualizations, correlations, missing data analysis, and automatic data quality alerts. It's the fastest way for a non-developer BA to understand a dataset end-to-end.

## Key Features
- One-line profiling: `ProfileReport(df)` generates a full interactive HTML report
- Automatic data type inference (categorical, numerical, date, text, images)
- Data quality alerts — flags missing values, high correlation, skewness, duplicates, and constant columns
- Dataset comparison mode — compare two DataFrames side-by-side (e.g., before/after migration)
- Time-series analysis with ACF/PACF plots for temporal data
- Integrates with Great Expectations, Streamlit, Airflow, Kedro, and Spark

## Installation
```bash
pip install ydata-profiling
# For Jupyter notebook widget support:
pip install ydata-profiling[notebook]
```

## How to Use It in Your BA Workflow (Obsidian)

### 1. Rapid Data Discovery for Requirements Gathering
When you receive a new dataset from a stakeholder (CSV export, database dump, API response), run a one-liner before your first requirements meeting:
```python
from ydata_profiling import ProfileReport
import pandas as pd

df = pd.read_csv("customer_data.csv")
report = ProfileReport(df, title="Customer Data Discovery")
report.to_file("customer_data_profile.html")
```
Open the HTML report, screenshot the key stats and alerts, and paste them into an Obsidian note like `[[Data Discovery - Customer Module]]`. This gives you concrete talking points: "47% of phone numbers are missing — do we need validation rules?" Use this to drive requirements conversations with evidence instead of assumptions.

### 2. Data Quality Assessment for BRDs and FRDs
Before writing a Business Requirements Document, profile the source data to document its current state. The automatic **Alerts** section flags issues like high cardinality, constant values, and highly correlated columns. Copy these alerts into your BRD under a "Current State Data Quality" section in Obsidian:
```markdown
## Current State Data Quality (from ydata-profiling)
- ⚠️ `email` column: 12% missing values — need validation rule
- ⚠️ `status` column: 89% single value ("Active") — consider removing from reports
- ⚠️ `order_date` and `ship_date` correlation: 0.97 — may be redundant
```
This transforms your BRD from opinion-based to evidence-based.

### 3. Before/After Comparison for UAT and Migration Testing
Use the **compare** feature to validate data migrations or system changes. Profile the source and target datasets, then generate a comparison report:
```python
from ydata_profiling import ProfileReport

source_report = ProfileReport(source_df, title="Legacy System")
target_report = ProfileReport(target_df, title="New System")
comparison = source_report.compare(target_report)
comparison.to_file("migration_comparison.html")
```
Save the comparison findings in Obsidian under `[[UAT - Data Migration Validation]]` with screenshots. This is concrete evidence for your test case sign-off — no manual row-by-row checking needed.

### 4. Stakeholder Communication — Translating Data into Plain Language
Export the profiling report as HTML and share it directly with non-technical stakeholders. The visualizations (histograms, bar charts, heatmaps) tell the story without SQL. In your Obsidian meeting notes, create a summary template:
```markdown
## Data Briefing for [[Stakeholder Name]]
**Dataset:** Customer Orders Q1 2026
**Records:** 45,230 | **Columns:** 18
**Top Issues Found:**
1. 3,400 duplicate order IDs (7.5%) — needs dedup rule
2. Revenue column has 200 outliers above $50K — confirm with finance
3. 4 columns are 100% empty — candidates for removal
**Action Items:** [link to profiling report HTML]
```
This turns a raw dataset into an executive-ready briefing in minutes.

### 5. Gap Analysis for System Integration Projects
When integrating two systems, profile both datasets independently and compare their schemas, data types, and value distributions. Document gaps in Obsidian:
```markdown
## Integration Gap Analysis — CRM vs ERP
| Field | CRM (Salesforce) | ERP (Oracle) | Gap |
|-------|------------------|--------------|-----|
| Customer ID | String, 0% null | Integer, 2% null | Type mismatch + nulls |
| Status | 5 unique values | 12 unique values | Value mapping needed |
| Created Date | UTC timezone | Local timezone | TZ conversion required |
```
ydata-profiling's type detection and unique value counts give you this mapping automatically. Link the gap analysis to your `[[Integration Requirements]]` note with `[[wikilinks]]` for full traceability.

## Why This Tool Today
Today's pick focuses on the data analysis/reporting angle of BA work. ydata-profiling is uniquely valuable because it requires zero SQL or advanced Python knowledge — a single line of code produces a report that would take hours to build manually. With 13K+ stars and MIT license, it's battle-tested and actively maintained. For BAs who spend time profiling data before writing requirements, this tool eliminates the most tedious part of the job.

---
*Auto-generated by Claude | Daily BA GitHub Discovery*
