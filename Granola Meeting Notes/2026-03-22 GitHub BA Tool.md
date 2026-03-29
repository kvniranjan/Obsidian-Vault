---
date: 2026-03-22
type: github-discovery
tags: [business-analyst, automation, github, tools]
---

# 🛠️ BA Tool of the Day — 2026-03-22

## Repository
- **Name:** MeetingMind
- **GitHub URL:** https://github.com/misbahsy/meetingmind
- **Stars:** ⭐ 497
- **License:** MIT
- **Last Updated:** 2024-10 (stable, 22 commits)

## What It Does
MeetingMind is an AI-powered meeting analysis app that processes meeting recordings and generates comprehensive, structured summaries in under 30 seconds. It automatically extracts tasks, decisions, questions, insights, deadlines, attendees, follow-ups, risks, and agenda items from audio files — turning raw meeting content into actionable intelligence.

## Key Features
- Audio recording and file upload for meeting capture
- AI-powered transcription via Groq Whisper
- Automatic extraction of 9 metadata categories: tasks, decisions, questions, insights, deadlines, attendees, follow-ups, risks, agenda items
- Dashboard interface for reviewing and browsing processed meetings
- Meeting history with detailed analytics and search
- Langflow-based customizable AI workflow pipeline
- SQLite or PostgreSQL storage for meeting archives

## Installation
1. Clone: `git clone https://github.com/misbahsy/meetingmind.git`
2. Install dependencies: `npm install`
3. Set up Langflow backend server locally
4. Upload the provided Langflow workflow file
5. Configure `.env.local` with your Langflow URL and Groq API keys
6. Initialize database: `npx prisma db push`
7. Run: `npm run dev` → opens at `localhost:3000`

> **Note:** Audio files must be under 25 MB (Groq Whisper limit). Use FFmpeg to compress larger files.

## How to Use It in Your BA Workflow (Obsidian)

### 1. Convert Stakeholder Meetings into Structured Requirements Notes
After every stakeholder meeting, upload the recording to MeetingMind. It extracts decisions, tasks, and follow-ups automatically. Copy the structured output into an Obsidian note using this template:
```
## Meeting: [[Project Name]] — YYYY-MM-DD
### Decisions Made
- [paste from MeetingMind decisions]
### Requirements Identified
- [paste from MeetingMind insights + tasks]
### Open Questions
- [paste from MeetingMind questions]
### Follow-ups
- [paste from MeetingMind follow-ups with deadlines]
```
This bridges the gap between raw meeting audio and a traceable requirements log in your vault.

### 2. Auto-Generate Risk Registers from Discovery Sessions
MeetingMind's risk extraction is a goldmine for BAs. After running a discovery or sprint planning session through the tool, pull the "risks" output into your Obsidian risk register note:
```
## Risk Log — [[Project Name]]
| Risk | Source Meeting | Date | Mitigation | Owner |
|------|---------------|------|------------|-------|
| [MeetingMind risk item] | [[Meeting Note]] | 2026-03-22 | TBD | TBD |
```
Link each risk back to its source meeting note with `[[wikilinks]]` for full traceability.

### 3. Build a Decisions Log Across Multiple Meetings
Use MeetingMind's "decisions" extraction across a series of project meetings to maintain a living decisions log in Obsidian. After each meeting analysis, append to a single `Decisions — [[Project Name]].md` file:
```
### 2026-03-22 — Sprint Review
- Decision: API versioning will use URL path strategy (v1/v2)
- Decision: Auth module deferred to Phase 2
Source: [[2026-03-22 Sprint Review]]
```
Use Obsidian Dataview to query all decisions across projects: `TABLE decision FROM "Meetings" WHERE type = "decision"`.

### 4. Extract Action Items and Sync with Task Management
MeetingMind identifies tasks with owners and deadlines. After processing, create actionable task entries in Obsidian using the Tasks plugin format:
```
- [ ] Review API contract with vendor 📅 2026-03-25 👤 @sarah [[2026-03-22 Vendor Call]]
- [ ] Draft UAT test cases for payment module 📅 2026-03-28 👤 @niranjan [[2026-03-22 Sprint Planning]]
```
The `[[wikilink]]` back to the meeting note provides context for every task. Query all open tasks with Obsidian Tasks: `not done` + `path includes Meetings`.

### 5. Feed Meeting Insights into BRD/FRD Drafts
Use MeetingMind's "insights" and "questions" categories to populate your BRD sections directly. After analyzing a requirements gathering session, map the output:
- **Insights** → Business Requirements (what stakeholders need)
- **Questions** → Assumptions & Open Items section
- **Deadlines** → Timeline/Milestones table
- **Attendees** → Stakeholder Matrix

Create a BRD template note in Obsidian and use `![[Meeting Note#Insights]]` embedded links to pull live content from meeting notes into your BRD draft, keeping documentation always in sync with the latest discussions.

## Why This Tool Today
MeetingMind was selected because it directly addresses the most time-consuming part of a BA's job: turning unstructured meeting conversations into structured, actionable artifacts. Its automatic extraction of 9 distinct metadata categories (especially risks, decisions, and follow-ups) maps perfectly onto the documents BAs maintain daily, and its output integrates naturally with Obsidian's linking and querying capabilities.

---
*Auto-generated by Claude | Daily BA GitHub Discovery*
