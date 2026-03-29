---
date: 2026-03-29
type: github-discovery
tags: [business-analyst, automation, github, tools]
---

# 🛠️ BA Tool of the Day — 2026-03-29

## Repository
- **Name:** Doorstop
- **GitHub URL:** https://github.com/doorstop-dev/doorstop
- **Stars:** ⭐ 600+
- **License:** LGPLv3
- **Last Updated:** 2026-01 (v3.1)

## What It Does
Doorstop is a requirements management tool that stores textual requirements as YAML files alongside source code in version control. It builds a hierarchical tree of documents (requirements, test cases, specs) with traceable links between them, validates traceability chains, and publishes documents in HTML and Markdown formats.

## Key Features
- Each requirement stored as an individual YAML file — version-controlled, diff-friendly, and human-readable
- Hierarchical document tree with parent-child relationships between requirement sets
- Bidirectional traceability links between items (e.g., requirement → test case → design spec)
- Automated integrity checks that flag broken links, orphaned items, and incomplete coverage
- Multi-format publishing to HTML and Markdown with a single CLI command
- Full Python API for scripting custom workflows and reports
- Cross-platform support (Linux, macOS, Windows) with pre-commit hook integration

## Installation
```bash
pip install doorstop

# Initialize a new requirements tree in your project
doorstop create REQ ./requirements
doorstop create TST ./tests --parent REQ

# Add a requirement
doorstop add REQ

# Link a test to a requirement
doorstop link TST001 REQ001

# Validate traceability
doorstop

# Publish all documents as HTML
doorstop publish all ./output
```

## How to Use It in Your BA Workflow (Obsidian)

### 1. Build a Living Requirements Traceability Matrix
Initialize Doorstop in your project repo with three document levels: `BRD` (business requirements), `FRD` (functional requirements), and `TST` (test cases). Run `doorstop create BRD ./docs/brd`, `doorstop create FRD ./docs/frd --parent BRD`, and `doorstop create TST ./docs/tst --parent FRD`. Each requirement becomes a YAML file you can edit in any text editor. In Obsidian, create a `Requirements/` folder with an index note that links to the published HTML matrix: `[Traceability Matrix](file:///path/to/output/index.html)`. Run `doorstop publish all ./output` to regenerate the matrix whenever requirements change — giving you a live RTM without Excel.

### 2. Requirements-to-Test Coverage Validation
After each sprint planning or requirements workshop, add new requirements with `doorstop add BRD` and link corresponding test cases with `doorstop link TST042 FRD018`. Then run `doorstop` (no arguments) to validate the entire tree. The tool flags any requirement without a linked test case, any test case without a parent requirement, and any broken links. Capture the validation output in an Obsidian note: create `Requirements/Coverage Report YYYY-MM-DD.md` and paste the output. Use Obsidian tags like `#coverage/gap` or `#coverage/complete` to track which areas need attention in your next stakeholder review.

### 3. Version-Controlled Change Impact Analysis
Because every requirement is a YAML file in git, you can run `git log --oneline -- docs/brd/` to see exactly when each business requirement changed, who changed it, and why. In Obsidian, create a `Change Log.md` note with a Dataview query that pulls from your `Requirements/` folder. When a stakeholder asks "what changed since last release?", run `doorstop publish all` on the current branch vs. the release tag and diff the HTML output. This gives you a concrete, auditable change impact analysis — not a verbal summary from memory.

### 4. Stakeholder Review Packages via Published HTML
Before a requirements review meeting, run `doorstop publish all ./review-package` to generate a clean HTML site with all BRD items, their linked FRD items, and test coverage status. Share this as a static site (GitHub Pages, internal web server, or just a zip file). In your Obsidian meeting note, add a "Pre-Read" section: `- [Requirements Review Package v2.1](file:///path/to/review-package/index.html)`. After the meeting, update individual YAML items with feedback using `doorstop edit BRD005`, and the changes are automatically tracked in git — creating a full audit trail from review comment to requirement change.

### 5. Cross-Document Gap Analysis for Completeness
Create a script using Doorstop's Python API to generate a gap analysis report. Example:
```python
import doorstop
tree = doorstop.build()
brd = tree.find_document('BRD')
for item in brd:
    if not item.links:
        print(f"GAP: {item.uid} — '{item.text[:60]}' has no linked FRD")
```
Run this weekly and save the output as `Requirements/Gap Analysis YYYY-MM-DD.md` in Obsidian. Tag each gap with `#gap/unlinked` or `#gap/no-test`. Over time, this builds a historical record of how requirements coverage improves sprint over sprint — valuable evidence for process maturity assessments and audit readiness.

## Why This Tool Today
Doorstop addresses the most persistent pain point in BA work: maintaining a traceable, auditable link between business requirements, functional specs, and test cases — without relying on heavyweight proprietary tools like DOORS or Jama. Its YAML-per-requirement approach means every change is a git commit, making it uniquely suited for teams that already use version control. For a BA working in Obsidian, it bridges the gap between freeform notes and structured requirements management.

---
*Auto-generated by Claude | Daily BA GitHub Discovery*
