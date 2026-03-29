# Contributing to TakeOne

This document is a guide for anyone picking up TakeOne to build — whether you're a solo developer, a team, or an open-source contributor.

---

## Project Context

TakeOne is an AI-powered creative studio where specialized agents collaborate to produce short-form video. The repo currently contains the **complete product specification and UI prototypes** — no backend code has been written yet. You're building from a well-defined blueprint.

## Where to Start

### 1. Understand the Product (30 min)

Read these PRD sections in order:

- **Section 1** — Problem statement and market sizing. Understand *why* this exists.
- **Section 3** — Product overview and agent architecture. The core mental model.
- **Section 2** — User personas (Sarah, Marcus, Ravya). Who you're building for.

### 2. Understand the Architecture (1 hr)

- **PRD Section 5** — Technical architecture. Covers the 6-layer prompt assembly engine, project graph schema, agent orchestration, and infrastructure.
- **`docs/tech-architecture.pdf`** — Visual diagrams of the system topology.

### 3. Explore the UI (30 min)

Open any `.html` file from `design/` in your browser. The two theme folders (`cinematic-dark`, `ivory-light`) contain the same screens in different visual treatments. Start with `cinematic-dark` — it's the most complete set.

Recommended exploration order:
1. `01-homepage.html` — Landing page
2. `03-new-project.html` — Project creation flow
3. `04-scriptwriter-agent.html` — First agent interaction
4. `05-storyboard-*.html` — Visual planning (3 variants)
5. `06-reel-editor-*.html` — Timeline editing
6. `08-cinematographer*.html` — Camera/composition controls
7. `09-project-export.html` — Output delivery

### 4. Check Open Decisions

PRD Section 12 lists decisions that still need to be made — agent visibility in UI, video length limits, and other architectural choices. Review these before you start coding.

---

## Suggested Build Order

Based on the PRD roadmap:

### Phase 1: Foundation (Months 1–3)
- Project creation and management (the project graph)
- Scriptwriter Agent (simplest agent, validates the orchestration model)
- Basic auth and user accounts
- Credit system skeleton

### Phase 2: Core Agents (Months 4–6)
- Storyboard Agent with asset library
- Cinematographer Agent
- Reel Editor Agent with timeline
- Cross-agent context passing via project graph

### Phase 3: Platform (Months 7–9)
- Brand Kit system
- Collaboration and permissions
- Export pipeline
- Billing integration

### Phase 4: Scale (Months 10–12)
- Performance optimization
- Advanced agent capabilities
- Analytics and insights
- Enterprise features

---

## Tech Stack (from PRD)

The PRD recommends:
- **Frontend:** React/Next.js with Tailwind CSS (the prototypes already use Tailwind)
- **Backend:** Node.js or Python FastAPI
- **Database:** PostgreSQL with vector extensions for semantic search
- **AI Orchestration:** Multi-agent framework with a 6-layer prompt assembly engine
- **Infrastructure:** Cloud-native, GPU-enabled inference endpoints

See PRD Section 5 for full details.

---

## Design Notes

The HTML prototypes are self-contained — each file includes inline Tailwind CSS and is viewable by opening it directly in a browser. They represent the target UI fidelity, not throwaway wireframes.

The two themes exist to demonstrate visual flexibility:
- **Cinematic Dark** — Premium, media-focused aesthetic (recommended as primary)
- **Ivory Light** — Clean, minimal, professional

The PNG screenshots are from an earlier version and still show the original "Crushed Studios" branding. The HTML files are the source of truth.

---

## Questions?

Open an issue or reach out to [rishi@thetopscout.com](mailto:rishi@thetopscout.com).
