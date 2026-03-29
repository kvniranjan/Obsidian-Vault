---
date: 2026-03-25
type: skill
category: Business Analysis
tags: [business-analyst, skill, process-mining, data-analysis, process-improvement, python]
source: GitHub
---

# PM4Py - Process Mining for Business Analysts

## What is it?
PM4Py (Process Mining for Python) is an open-source Python library that extracts, visualizes, and analyzes real business process behavior from system event logs. Instead of relying on documented "should-be" processes, PM4Py reveals how processes *actually* execute by mining data from transactional systems like ERP, CRM, or ticketing tools.

## Why it matters for Business Analysts
BAs are often handed process documentation that doesn't reflect reality. PM4Py closes the gap between the "as-documented" and "as-executed" process by:
- Automatically discovering process flows from data (no manual observation needed)
- Identifying where variants, deviations, and bottlenecks actually occur
- Providing quantifiable evidence for process improvement recommendations
- Enabling conformance checking — comparing actual behavior against defined models
- Producing visual output (diagrams, heatmaps) ready for stakeholder presentations

This shifts BA process analysis from anecdotal to data-driven.

## How to use it in BA Workflows

### Step 1: Export Event Log from Source System
Extract a CSV or XES file from your system (SAP, Jira, ServiceNow, Salesforce) with columns:
- `case_id` — the unique process instance (e.g., order number, ticket ID)
- `activity` — the step performed (e.g., "Approve", "Escalate")
- `timestamp` — when it happened

### Step 2: Load and Discover the Process
```python
import pm4py
import pandas as pd

# Load event log
df = pd.read_csv("process_log.csv")
event_log = pm4py.format_dataframe(df, case_id='case_id', activity_key='activity', timestamp_key='timestamp')

# Discover process model (Inductive Miner algorithm)
process_tree = pm4py.discover_process_tree_inductive(event_log)
pm4py.view_process_tree(process_tree)
```

### Step 3: Visualize as BPMN or Petri Net
```python
bpmn_model = pm4py.convert_to_bpmn(process_tree)
pm4py.view_bpmn(bpmn_model)
```

### Step 4: Analyze Performance
```python
# See average time per activity
from pm4py.statistics.sojourn_time.log import get as soj_time
soj = soj_time.apply(event_log)
```

### Step 5: Conformance Checking
Compare actual execution to your target BPMN model to identify deviations and non-conforming cases.

## Key Features
- **Process Discovery**: Automatically generate Petri nets, BPMN, and process trees from raw logs
- **Conformance Checking**: Measure how well actual processes conform to reference models
- **Performance Analysis**: Calculate cycle times, waiting times, and bottleneck metrics
- **Variant Analysis**: Identify the most common (and most problematic) process variants
- **Visualization**: Export to SVG/PNG for presentations and reports
- **Multi-format Support**: Reads XES (standard process mining format) and CSV logs

## GitHub Resources
- [PM4Py Official Repo](https://github.com/process-intelligence-solutions/pm4py) — Core library with notebooks and examples
- [Process Mining Knowledge Base](https://github.com/lisenkovkv/process_mining) — Curated list of process mining resources
- [Awesome Process Mining](https://github.com/TheWoops/awesome-processmining) — Tools, papers, and community resources

## Related Skills
- [[BPMN Assistant (LLM-Powered)]]
- [[bpmn-io Web Modeler]]
- [[Automated Business Analysis Workflow (n8n + AI)]]
