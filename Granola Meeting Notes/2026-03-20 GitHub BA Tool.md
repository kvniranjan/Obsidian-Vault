---
date: 2026-03-20
type: github-discovery
tags: [business-analyst, automation, github, tools]
---

# 🛠️ BA Tool of the Day — 2026-03-20

## Repository
- **Name:** PM4Py
- **GitHub URL:** https://github.com/process-intelligence-solutions/pm4py
- **Stars:** ⭐ 930
- **License:** AGPL-3.0
- **Last Updated:** 2026-03 (v2.7.22, actively maintained)

## What It Does
PM4Py is a Python library for process mining — it lets you discover, analyze, and optimize business processes from event log data. Built by a Fraunhofer FIT spin-off, it implements state-of-the-art algorithms for process discovery (Alpha Miner, Inductive Miner, Heuristics Miner), conformance checking, and performance analysis. Think of it as turning raw system logs into visual process maps that reveal bottlenecks, deviations, and inefficiencies.

## Key Features
- Process discovery algorithms (Alpha, Inductive, Heuristics miners) that generate Petri nets and BPMN models from event logs
- Conformance checking to compare actual processes against designed models and find deviations
- Performance analysis with bottleneck detection and cycle time measurement
- Support for XES, CSV, and Parquet event log formats via pandas/polars
- Process visualization with graphviz-based flowcharts, dotted charts, and social network graphs

## Installation
```bash
pip install -U pm4py
```
Requires Python 3.9–3.14. For visualization, also install Graphviz system package:
- Windows: `choco install graphviz`
- Mac: `brew install graphviz`

## How to Use It in Your BA Workflow (Obsidian)

### 1. Mine As-Is Processes from System Logs for Gap Analysis
Export event logs from your core banking or ERP system (e.g., Oracle Flexcube transaction logs) as CSV. Run PM4Py's Inductive Miner to auto-discover the actual process flow, then save the generated BPMN/Petri net diagram as a PNG. Embed it in an Obsidian note alongside your designed To-Be process to visually highlight gaps:
```python
import pm4py
log = pm4py.read_xes("loan_approval_log.xes")
process_tree = pm4py.discover_process_tree_inductive(log)
bpmn = pm4py.convert_to_bpmn(process_tree)
pm4py.save_vis_bpmn(bpmn, "loan_process_actual.png")
```
Then in Obsidian: `![[loan_process_actual.png]]` next to your requirements note for side-by-side comparison.

### 2. Generate Data-Backed Evidence for BRDs and Change Requests
Instead of relying on stakeholder interviews alone, use PM4Py's performance analysis to extract hard metrics — average cycle times, bottleneck activities, rework loops. Paste these stats directly into your BRD's "Current State Analysis" section:
```python
# Get case durations and bottleneck stats
stats = pm4py.get_all_case_durations(log)
bottlenecks = pm4py.discover_performance_dfg(log)
```
Create an Obsidian note template: `Templates/BRD Current State.md` with placeholders for `{{avg_cycle_time}}`, `{{top_bottleneck}}`, `{{rework_rate}}` that you fill from PM4Py output.

### 3. Conformance Checking for UAT and Post-Go-Live Validation
After a system change goes live, compare actual process execution against the designed model to verify the implementation matches requirements. PM4Py's conformance checking produces a fitness score and pinpoints exactly where deviations occur:
```python
net, im, fm = pm4py.discover_petri_net_inductive(log)
conformance = pm4py.conformance_diagnostics_token_based_replay(log, net, im, fm)
fitness = pm4py.fitness_token_based_replay(log, net, im, fm)
```
Save results as a post-go-live validation note in Obsidian: `[[2026-03-20 Loan Process Conformance Check]]` with fitness score and deviation list, linked to the original requirements note.

### 4. Stakeholder-Ready Process Maps for Communication
Generate clean, visual process maps that non-technical stakeholders can immediately understand. PM4Py produces directly-follows graphs with frequency and performance annotations — perfect for steering committee decks or walkthrough sessions:
```python
dfg, start, end = pm4py.discover_dfg(log)
pm4py.save_vis_dfg(dfg, start, end, "process_map_frequency.png")
# Performance variant with time annotations
pm4py.save_vis_performance_dfg(dfg, start, end, "process_map_performance.png")
```
Store these in `Obsidian Vault/Attachments/` and reference them across multiple notes — your stakeholder update, your process analysis note, and your recommendation doc all link to the same source-of-truth diagram.

### 5. Social Network Analysis to Map Stakeholder Handoffs
Use PM4Py's organizational mining to discover who hands off work to whom, identifying key stakeholders and communication bottlenecks in your process. This is invaluable for stakeholder analysis and RACI matrix creation:
```python
# Discover handoff patterns between roles/teams
sna = pm4py.discover_handover_of_work_network(log)
pm4py.save_vis_sna(sna, "handoff_network.png")
```
Create an Obsidian note `[[Stakeholder Handoff Analysis]]` embedding the network diagram, then link it to your `[[RACI Matrix]]` and `[[Stakeholder Register]]` notes. The data reveals which handoffs are most frequent and where delays accumulate — direct input for process improvement recommendations.

## Why This Tool Today
PM4Py was selected because process mining is one of the most powerful yet underutilized techniques in a Business Analyst's toolkit. While most BA tools focus on creating documentation, PM4Py works backwards from actual data — letting you discover what really happens in your processes rather than what people say happens. With 930 stars and active development (updated today), it's the de facto standard for Python-based process mining.

---
*Auto-generated by Claude | Daily BA GitHub Discovery*
