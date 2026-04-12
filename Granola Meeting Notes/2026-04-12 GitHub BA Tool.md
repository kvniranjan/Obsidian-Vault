---
date: 2026-04-12
type: github-discovery
tags: [business-analyst, automation, github, tools]
---

# 🛠️ BA Tool of the Day — 2026-04-12

## Repository
- **Name:** Excalidraw
- **GitHub URL:** https://github.com/excalidraw/excalidraw
- **Stars:** ⭐ 121,000+
- **License:** MIT
- **Last Updated:** 2026-04 (actively maintained)

## What It Does
Excalidraw is a free, open-source virtual whiteboard that lets you sketch diagrams, wireframes, and flows with a distinctive hand-drawn visual style. Running entirely in the browser with no account required, it is an infinite canvas where you can draw shapes, add text, connect elements with arrows, embed images, and annotate anything — all in a format that deliberately looks informal and exploratory rather than polished and final. This low-fidelity aesthetic is actually a strategic advantage for Business Analysts: stakeholders are far more willing to challenge and revise a hand-drawn sketch than a slick diagram, which means you get better feedback earlier.

The tool supports real-time collaboration through end-to-end encrypted sessions — you share a link and collaborators join the same live canvas instantly, with no sign-up or installation barrier. All session data is encrypted client-side so the Excalidraw server never sees your content, making it suitable for sensitive project work. The native file format is `.excalidraw`, which is plain JSON, meaning files are human-readable, version-controllable with git, and importable by other tools. You can also export to PNG, SVG, and clipboard for embedding in documents or presentations.

With over 121,000 GitHub stars as of April 2026, Excalidraw is one of the most widely adopted open-source tools in its category. It is actively maintained by a dedicated core team, ships frequent updates, and has a rich library of community-contributed shape templates (excalidraw-libraries) covering everything from AWS architecture diagrams to BPMN flows — giving BAs a head start on common diagramming tasks without drawing from scratch.

## Key Features
- Infinite canvas with hand-drawn style shapes, text, arrows, and freehand drawing for low-fidelity diagramming
- Real-time collaboration via end-to-end encrypted sessions — no account required, just share a link
- Privacy-first: all data stays in browser localStorage unless you explicitly export or share; server never sees your content
- Export to PNG, SVG, and clipboard; import images and embed them directly on the canvas
- `.excalidraw` file format is plain JSON — portable, version-controllable, and readable without the app
- Extensive community shape library (excalidraw-libraries) with templates for UML, BPMN, wireframes, flowcharts, AWS/Azure diagrams, and more
- Mermaid-to-Excalidraw converter for turning code-based diagrams into editable visual canvases

## Installation
```bash
# Option 1: Use the hosted app — no installation required
# Navigate to https://excalidraw.com in any browser and start drawing immediately
# No account, no login, no data uploaded unless you start a collaboration session

# Option 2: Self-host with Docker (for teams with data sovereignty requirements)
docker run -p 3000:80 excalidraw/excalidraw

# Option 3: Install as a desktop Progressive Web App (PWA)
# Open https://excalidraw.com in Chrome/Edge → browser menu → "Install Excalidraw"
# Runs offline and saves directly to your filesystem

# Option 4: Use the npm package to embed Excalidraw in your own web app
npm install @excalidraw/excalidraw
```

## How to Use It in Your BA Workflow (Obsidian)

### 1. Live Requirements Workshop Facilitation
Replace physical or virtual sticky-note sessions with a shared Excalidraw canvas. Before a requirements elicitation workshop, set up the canvas with labelled zones for each topic area — "As-Is Process", "Pain Points", "Desired Outcomes", "Out of Scope". Share the collaboration link with attendees at the start of the session. As participants contribute ideas verbally, sketch them as text nodes and connect related concepts with arrows in real time. The hand-drawn style signals that everything is still open for discussion, which typically produces more candid input than a polished diagram would. After the workshop, export the canvas as a PNG and embed it in your Obsidian meeting note, then save the `.excalidraw` file in your vault folder alongside it for future editing.

### 2. Low-Fidelity Wireframing for Rapid UI Feedback
Use Excalidraw's wireframe shape library to sketch screen layouts and user flows before committing to a formal prototype in Penpot or Figma. Hand-drawn wireframes communicate intent without implying a finished design, which encourages stakeholders to focus on functionality and flow rather than colours and fonts. Draw each screen as a box with rough UI elements, connect screens with labelled arrows showing navigation, and annotate with business rules directly on the canvas. Share the collaboration link with the product owner and developers for asynchronous mark-up — they can add comments as sticky-note shapes. Export the agreed wireflow as SVG and embed it in your Obsidian user story or feature specification note as the visual acceptance criteria.

### 3. Process and Data Flow Diagramming
Use the BPMN and flowchart templates from excalidraw-libraries to sketch process flows during discovery, without the setup overhead of a dedicated BPMN tool. For early-stage analysis where the process is still being understood, Excalidraw's freeform canvas is faster than a constrained modelling tool — you can draw rough swim lanes, add decision diamonds, and annotate exceptions all in one fluid session. Once the process is agreed at this sketch level, hand it off to a more formal tool (like the BPMN Assistant discovered earlier) for the baseline artefact. Store the `.excalidraw` source file in Obsidian alongside the formal BPMN export so the design history is preserved and the sketch can be retrieved if the process needs to be revisited.

### 4. Stakeholder Impact and Relationship Mapping
Create visual stakeholder maps on the Excalidraw canvas: place each stakeholder as a labelled circle, group them by organisational unit using rectangles, and draw directional arrows to show communication flows, dependencies, and influence relationships. Add colour coding (using Excalidraw's fill colours) to indicate support level — green for champions, yellow for neutral, red for resistors. This visual map is far more effective in a steering committee than a table of names and interest ratings. Export as PNG and embed in your Obsidian stakeholder register note. Because the file is plain JSON, you can also diff the `.excalidraw` file between project phases to see exactly which relationships changed — a lightweight change log for your stakeholder landscape.

### 5. Decision and Option Analysis Canvases
When analysing solution options or competing approaches, lay out each option as a column on an Excalidraw canvas with rows for criteria — cost, risk, complexity, time-to-market, strategic fit. Use arrows and annotations to link criteria to evidence from elicitation sessions. The freeform canvas lets you add context notes that don't fit in a structured matrix, such as "SME raised concerns in workshop 2" as a sticky note next to the relevant cell. Share the live canvas during the options-review meeting so stakeholders can annotate directly, creating a collaborative decision record. Export the final annotated canvas as PNG, embed it in your Obsidian decision log note, and save the `.excalidraw` source alongside it. This single file captures both the structured comparison and the informal discussion trail in one versioned artefact.

## Why This Tool Today
None of the previously discovered tools support real-time collaborative visual thinking on a freeform canvas — Freeplane is a hierarchical mind mapper, Penpot is a high-fidelity design tool, and BPMN Assistant is a constrained modelling environment. Excalidraw fills a fundamentally different role: it is the fastest, lowest-friction way to capture and share visual thinking with any stakeholder, anywhere, with no installation or sign-up barrier. Its hand-drawn aesthetic is not just aesthetic — it is a deliberate collaboration strategy that gets better requirements feedback earlier in the project lifecycle.

---
*Auto-generated by Claude | Daily BA GitHub Discovery*
