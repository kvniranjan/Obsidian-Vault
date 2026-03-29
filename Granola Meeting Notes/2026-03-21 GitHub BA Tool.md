---
date: 2026-03-21
type: github-discovery
tags: [business-analyst, automation, github, tools]
---

# 🛠️ BA Tool of the Day — 2026-03-21

## Repository
- **Name:** BPMN Assistant
- **GitHub URL:** https://github.com/jtlicardo/bpmn-assistant
- **Stars:** ⭐ 112
- **License:** MIT
- **Last Updated:** 2026-03 (actively maintained, 269 commits)

## What It Does
BPMN Assistant is an LLM-powered tool that lets you create, edit, and interpret Business Process Model and Notation (BPMN) diagrams using natural language. You describe a process in plain English, and it generates a fully rendered BPMN 2.0 diagram. It also supports uploading flowchart images and converting them into editable BPMN XML.

## Key Features
- **Natural language → BPMN diagram:** Describe a process in text, get a standards-compliant BPMN diagram
- **Diagram editing via chat:** Ask the AI to modify tasks, gateways, or flows conversationally
- **Diagram interpretation:** Upload a BPMN file and get a plain-text explanation of the process
- **Image-to-BPMN conversion:** Upload a whiteboard photo or flowchart screenshot and convert it to BPMN (OpenAI models)
- **Multi-LLM support:** Works with Claude Opus 4.6, Claude Sonnet 4.5, GPT-5.2, GPT-4.1, Gemini 3, and Kimi K2.5
- **Full BPMN element support:** User tasks, service tasks, exclusive/parallel/inclusive gateways, timer/message events, and more
- **Drag-and-drop BPMN files** for instant rendering and editing
- **Hosted version available** — no local setup required

## Installation
**Quickest option:** Use the hosted version at `bpmn-frontend.onrender.com` — just enter your API key in the browser (stored locally).

**Local Docker deployment:**
```bash
git clone https://github.com/jtlicardo/bpmn-assistant.git
cd bpmn-assistant
cp src/bpmn_assistant/.env.example src/bpmn_assistant/.env
# Add your API key (ANTHROPIC_API_KEY, OPENAI_API_KEY, etc.) to .env
docker-compose up --build
# Access at http://localhost:8080
```

## How to Use It in Your BA Workflow (Obsidian)

### 1. Rapid Process Mapping from Meeting Notes
After a stakeholder meeting, paste your Granola meeting transcript into BPMN Assistant with a prompt like: *"Create a BPMN diagram for the invoice approval process described here: [paste notes]"*. Export the generated `.bpmn` file, convert it to an image, and embed it directly in your Obsidian meeting note with `![[invoice-approval-process.png]]`. This turns raw meeting conversations into formal process diagrams in under 2 minutes.

### 2. As-Is vs To-Be Process Documentation
For gap analysis, generate two BPMN diagrams — one for the current state and one for the proposed state. Prompt: *"Create a BPMN diagram for the current manual employee onboarding process: HR receives request → manager approval → IT ticket → badge creation → orientation scheduling"*, then a second: *"Now modify this to add automated IT provisioning via ServiceNow after manager approval and parallel badge + orientation scheduling"*. Save both as images in an Obsidian note under `## As-Is Process` and `## To-Be Process` headings for a clear visual gap analysis.

### 3. Converting Whiteboard Photos to Formal Diagrams
After a workshop, photograph the whiteboard flowchart and upload it to BPMN Assistant using the vision feature (OpenAI models). It converts the hand-drawn diagram into a clean, editable BPMN file. Export the polished version and link it in your Obsidian BRD or FRD document: `![[whiteboard-to-bpmn-returns-process.png]]`. This eliminates the manual re-drawing step that typically takes hours.

### 4. Generating Process Descriptions for Stakeholder Sign-Off
Use the **interpretation** feature in reverse: upload an existing `.bpmn` file from your system documentation and ask it to *"Explain this process in plain English, step by step, including decision points and exception paths"*. Copy the generated text into an Obsidian note formatted as a process narrative under your `[[Project Requirements]]` page. Non-technical stakeholders who can't read BPMN diagrams can now review and approve the process in plain language.

### 5. Iterative Requirements Refinement via Chat
Start with a rough process description from your initial requirements and refine it conversationally: *"Add an error handling path after the payment gateway step — if payment fails, retry once then escalate to manual review"*. Each iteration produces an updated diagram without starting over. Export the final version and maintain a version history in Obsidian by saving each iteration as `v1`, `v2`, etc. in a `Process Diagrams/` folder, linking them in your requirements traceability note with `[[Payment Process v3]]`.

## Why This Tool Today
BPMN Assistant was selected because process diagramming is one of the most time-consuming BA tasks, and this tool eliminates the friction of learning complex modeling tools like Visio or Camunda Modeler. Its support for Claude models means it integrates naturally with an Anthropic-powered workflow, and the ability to convert whiteboard photos and meeting notes directly into standards-compliant BPMN diagrams is a genuine productivity multiplier for BAs working in Obsidian.

---
*Auto-generated by Claude | Daily BA GitHub Discovery*
