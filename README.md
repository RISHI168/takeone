# TakeOne

**The world's first role-based AI creative studio** — where specialized AI agents collaborate to produce professional short-form video content through an intelligent project graph system.

TakeOne treats post-production as an operating system, not a collection of point tools. Four specialized agents (Scriptwriter, Storyboard Artist, Cinematographer, Reel Editor) coordinate through a shared project graph with cross-scene continuity tracking and 230+ configurable parameters.

---

## What This Repo Contains

This is the **product design & specification layer** for TakeOne — everything a team needs to pick up the project and start building.

```
takeone/
├── docs/
│   ├── PRD.md                        # Full Product Requirements Document (~190KB)
│   └── tech-architecture.pdf         # System architecture diagrams
│
├── design/
│   ├── cinematic-dark/               # 19 screens — dark cinematic theme
│   └── ivory-light/                  # 19 screens — light ivory theme
│
├── CONTRIBUTING.md
└── README.md
```

### `/docs`

The PRD covers 12 sections: problem statement & market sizing, three user personas, full feature specs for each agent, technical architecture (6-layer prompt assembly engine, project graph schema, credit system), UX workflows, risk mitigation, go-to-market strategy, pricing tiers (Free / Starter $9 / Pro $39 / Studio $99 / Enterprise), success metrics, and a phased roadmap.

The tech architecture PDF contains system diagrams for the agent orchestration layer, data flow, and infrastructure topology.

### `/design`

38 interactive HTML prototypes covering every core screen across two visual themes. Each screen has a `.html` file (live Tailwind CSS prototype you can open in any browser) and a `.png` screenshot.

**Screen inventory:**

| # | Screen | Description |
|---|--------|-------------|
| 01 | Homepage | Landing page with value proposition and CTA |
| 02 | Dashboard | Project overview, recent work, quick actions |
| 03 | New Project | Project creation wizard with brand kit integration |
| 04 | Scriptwriter Agent | AI script generation with tone, structure, and hook controls |
| 05 | Storyboard Agent | Visual scene planning — AI generation, manual uploads, visual intelligence |
| 06 | Reel Editor Agent | Timeline editing, media selection, transitions |
| 07 | Brand Kit | Logo, colors, fonts, voice guidelines management |
| 08 | Cinematographer Agent | Camera language, shot composition, visual style controls |
| 09 | Project Export | Render settings, format selection, delivery |
| 10 | Collaboration | Team access, permissions, project sharing |
| 11 | Credits & Billing | Usage tracking, plan management, payment |
| 12 | Profile | Account settings and preferences |
| 13 | Support Center | Help docs, ticket submission |
| 14 | Security Settings | Password, 2FA, session management |
| 15 | Pricing | Plan comparison and subscription management |

---

## The Thesis

Content creators produce 10–30 short-form videos per week to stay visible. A single 30-second professional reel takes 4–6 hours across 5–7 different tools. Existing AI tools generate assets but don't orchestrate workflows — they're primitives, not professionals.

TakeOne closes this gap with **agent specialization** (each agent has deep domain knowledge in its craft) and **cross-agent orchestration** (the project graph maintains context from script through final export). The result: professional-quality content in under 15 minutes.

**Target:** $500K ARR Year 1, 25,000 active creators.

---

## How to Pick Up This Project

See [CONTRIBUTING.md](CONTRIBUTING.md) for a detailed guide on how to start building from this spec.

**Quick orientation:**

1. Read `docs/PRD.md` — Sections 1–3 for context, Section 5 for architecture, Section 4 for feature specs
2. Open any `design/*.html` file in a browser to explore the UI
3. Review `docs/tech-architecture.pdf` for system diagrams
4. Check the open decisions in PRD Section 12

---

## Known Gaps

- **No backend code yet** — this repo is the design/spec layer. The PRD Section 5 (Technical Architecture) defines the stack and schema.
- **Binary files with legacy branding** — `tech-architecture.pdf` and all `.png` screenshots still show "Crushed Studios" (the original working title). The HTML prototypes and PRD markdown are fully rebranded to TakeOne.
- **No CI/CD, tests, or infra config** — these are defined in the PRD roadmap (Phase 1–3) but not yet implemented.

---

## License

MIT

---

## Author

**Rishi Bhattacharjee**
- [The TopScout](https://thetopscout.com)
- [Tech Fondue](https://techfondue.substack.com)
- [LinkedIn](https://linkedin.com/in/rishibhattacharjee)
