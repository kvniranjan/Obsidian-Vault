---
date: 2026-05-25
type: skill
category: Business Analysis
tags: [business-analyst, skill, process-mining, process-modeling, bpmn, workflow-analysis, event-log, as-is-process, process-discovery]
source: GitHub
---

# Cortado - Interactive Process Mining and Discovery Tool

## What is it?
Cortado is an open-source, end-user process mining tool dedicated to interactive and incremental process discovery, developed by Fraunhofer FIT. It allows business analysts to gradually build accurate process models by selecting and incorporating real process behavior from event logs rather than auto-generating a single monolithic model. The tool runs as a standalone desktop application (Windows, Linux, macOS) built with Angular and Electron, backed by a Python core library.

## Why it matters for Business Analysts
Cortado bridges the gap between raw system event data and formal process models, enabling BAs to perform data-driven AS-IS process analysis without requiring deep technical expertise. The incremental discovery approach lets analysts add process variants one at a time, maintaining control and explainability over the resulting model rather than accepting a black-box auto-discovered result. This is invaluable when conducting process audits, gap analysis between documented and actual processes, or preparing for workflow redesign initiatives. The built-in temporal performance analysis also surfaces bottlenecks and timing deviations directly within the discovered model.

## How to use it in BA Workflows
1. **AS-IS Process Documentation** - Import event logs exported from ERP, CRM, or BPM systems (XES format) and use Cortado's Variant Explorer to visually inspect all recorded process variants before building the official model.
2. **Conformance Gap Analysis** - Incrementally add the "happy path" variants to a model, then compare the remaining unselected variants to identify deviations from the intended process — a structured way to find compliance gaps.
3. **Process Simplification for Stakeholders** - Start with a minimal, clean process model covering the most frequent cases and progressively add edge cases, producing tiered diagrams suited to different stakeholder audiences (executive summary vs. detailed operational view).
4. **Bottleneck and Performance Analysis** - Use the temporal performance analysis feature to annotate the discovered model with real timing data, giving BAs concrete evidence for SLA violations or inefficiency hotspots to present in requirements workshops.
5. **Pre-Automation Scoping** - Before handing off a process to an automation team (RPA, BPMN execution), use Cortado to produce a verified, data-backed process model as the authoritative specification, reducing ambiguity in handoff.

## Key Features
- **Variant Explorer** - Visual interface for browsing all distinct process execution paths observed in the event log
- **Incremental Model Building** - Add selected variants to a Petri net model one at a time, maintaining analyst control over scope
- **Manual Model Editing** - Edit the process model under construction to correct or refine auto-suggested structures
- **Temporal Performance Analysis** - Model-based and model-independent timing overlays showing throughput times and waiting times
- **Export Formats** - Save discovered models as `.ptml` (Petri net) or `.pnml` for use in downstream BPMN/process tools
- **Import Support** - Loads industry-standard `.xes` event log files and initial `.ptml` process models
- **Standalone Desktop App** - No server setup required; cross-platform builds available from GitHub Releases

## Technology Stack
- **Languages:** TypeScript (Angular frontend), Python (cortado-core algorithm library)
- **Runtime:** Electron (desktop packaging), Node.js
- **Dependencies:** PM4Py (underlying process mining algorithms), Angular, Electron
- **License:** GPL-3.0

## GitHub Resources
- [cortado-tool/cortado](https://github.com/cortado-tool/cortado) - Main desktop application for interactive process discovery
- [cortado-tool/cortado-core](https://github.com/cortado-tool/cortado-core) - Python library implementing the incremental discovery algorithms

## Related Skills
- [[PM4Py - Process Mining for Business Analysts]]
- [[Camunda - BPMN Process Orchestration Framework]]
- [[SpiffArena - BPMN Workflow Automation Platform]]
- [[Flowable Engine - BPMN and BPM Workflow Automation Platform]]
