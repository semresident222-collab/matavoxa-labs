# MetaVoxa Labs

**labs.metavoxa.com** — Research infrastructure for invisible populations.

> MetaVoxa Labs designs research-grade data frameworks for neurodivergent global health populations. Populations every existing diagnostic instrument was built without. This repo holds the public-facing site for that infrastructure.

---

## What This Is

MetaVoxa Labs is not a product. It is not a consultancy. It is research infrastructure — the frameworks, cohort models, measurement systems, and policy translation mechanisms that make previously unmeasurable phenomena measurable.

The site is an archive interface: five layers of work, each holding active entries and reserved slots for future work. The reserved slots are principled commitments — work that does not yet have the evidence to justify going live.

---

## The Five Layers

| # | Layer | Prefix | What it holds |
|---|-------|--------|---------------|
| 01 | **Observations** | OBS | Early signals, systemic blind spots, real-world patterns conventional systems overlook |
| 02 | **Frameworks** | DF | Research-grade data frameworks and measurement models |
| 03 | **Cohorts** | COH | Population design models built around who existing research excluded |
| 04 | **Evidence** | EV | Publications, preprints, qualitative archives, academic collaborations |
| 05 | **Translation** | TR | Policy translation, regulatory analysis, mechanisms that carry evidence to where it changes things |

Layer 06 — **Lab Logs** — exists in the interface as a locked drawer. It will open when ready.

---

## Architecture

### Entry States

Every entry in the archive carries one of these states:

| State | Meaning |
|-------|---------|
| **Active** | Live, being worked on |
| **Active Research** | Formal research protocol running |
| **Active Preparation** | Actively preparing for a specific event or submission |
| **Research Phase** | In formal research/patent phase |
| **Validation** | Framework under validation testing |
| **Development** | In active development |
| **Evidence Mapping** | Mapping existing evidence base |
| **Protocol Stage** | Research protocol written, awaiting ethics/IRB |
| **In Progress** | Ongoing collection or production |
| **Submitted** | Submitted and awaiting response |
| **Published** | Formally published |
| **Forming** | Question or framework still forming |
| **Reserved** | Future work — present but not yet evidenced |

### Reserved Entries

Reserved entries are not wishful thinking. They are disciplined scope-holding. A cohort is Reserved because the evidence base for including it does not yet exist. A framework is Reserved because the first spark has not yet produced enough to justify a live entry. This mirrors the Kill Criteria and First Spark discipline in the MetaVoxa Strategic Questions Registry.

Reserved entries become Active only when there is a documented trigger — a Lived Reality observation, a research question entered in the Registry, or a protocol approved.

---

## Content Source of Truth

All content in this site is derived from the **MetaVoxa Knowledge Core** — specifically:

- **Strategic Questions Registry** (Lived Reality Triggers → Observations layer)
- **Innovation Registry** (patents, frameworks → Frameworks layer)
- **Research Library** (publications, preprints → Evidence layer)
- **Ecosystem Map** (five-layer architecture)
- **Founder Profile** (current active projects and constraints)

**The Fortress Principle applies here:** if the content on this site and the Knowledge Core ever disagree, the Knowledge Core wins. This site is an output. The Core is the source.

Update site content only after updating the relevant Knowledge Core document first.

---

## What Is Not Here

**GlacéGrip and SMWB** are not in this repo and do not appear on this site. They are consumer IP that partially funds MetaVoxa's research infrastructure. They live on `marthakoroma.com` under the Founder/About section, where they can be given the full context they deserve. Mixing a steering-wheel cooling device into a page about GDPR-compliant cohort design for neurodivergent health data would undercut the research-infrastructure positioning the moment a visitor scrolled past the hero.

---

## Tech

- **Framework:** React (JSX, functional components, hooks)
- **Styling:** Inline styles — no CSS framework, no external stylesheet
- **Fonts:** Source Serif 4 (display), IBM Plex Sans (body), JetBrains Mono (index labels/metadata) via Google Fonts
- **Interactions:** Drawer open/close via `max-height` transition; card hover via local `useState`; modal via fixed overlay
- **Light/Dark toggle:** CSS token swap on page context; the filing cabinet always stays dark wood (physical object, not a UI element)
- **No photo assets required** — the archive aesthetic is achieved entirely through typography, spacing, and CSS

---

## Design Language

The signature element is the **physical dark-wood filing cabinet with brass pulls and cream index cards** — the archive metaphor made literal. Everything else on the page is quiet around it.

Key decisions, and why:

- **Cabinet always dark** — it is a physical object. Its color does not change with the page's light/dark mode, the same way a real wooden cabinet in a room doesn't change color when you turn the lights on.
- **Cards always cream paper** — index cards are physical objects too. They are always paper-colored regardless of the surrounding interface.
- **Reserved entries visually distinct (dashed border, dimmed)** — future work is visible but clearly not-yet-real. This is a design decision and a credibility decision at once.
- **Lab Logs locked (Drawer 06)** — present but inaccessible. Signals that there is more, without claiming it is ready.
- **Two-column layout inside each drawer** — Current entries (left, clickable) and Reserved future work (right, read-only). The visual separation between what exists and what is coming is structural, not just labelled.

---

## Ecosystem Position

```
metavoxa.com  (landing — neutral front door)
   ├── atrium.metavoxa.com   — the sovereign digital estate
   ├── labs.metavoxa.com     — THIS REPO — research infrastructure
   ├── press.metavoxa.com    — essays, vocabulary, thought leadership
   ├── research.metavoxa.com — publications, preprints, academic record
   └── marthakoroma.com      — founder threshold (external)
```

Labs is one room. It does not explain the others. `metavoxa.com` is the front door.

---

## Known Gaps / Deferred

- **Mobile layout:** the two-column drawer interior needs responsive handling for narrow screens — currently best viewed on desktop. Planned: stack columns vertically on mobile, preserve the card and cabinet aesthetic.
- **Lab Logs (Drawer 06):** locked and inactive. Opens when Martha decides it is ready. No timeline.
- **Entry IDs:** Reserved entries currently share the placeholder `00X` — these will be numbered sequentially when entries become Active.
- **Cohorts layer:** currently holds one Active entry (Neurodivergent Women). Black Women, Migrant Populations, and Global Health Cohorts are Reserved pending documented first sparks in the Strategic Questions Registry.

---

## Deployment

- Domain: `labs.metavoxa.com` → this repo (CNAME record at DNS provider)
- Root `metavoxa.com` routes to the separate landing page repo
- [Add your actual host/build details here — GitHub Pages, Vercel, Netlify, etc.]

---

*Maintained by Martha Wuya Koroma. Part of the MetaVoxa Knowledge Core ecosystem.*  
*Last updated: June 2026*
