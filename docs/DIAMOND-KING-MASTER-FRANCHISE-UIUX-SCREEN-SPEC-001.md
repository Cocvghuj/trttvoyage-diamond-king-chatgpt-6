# Diamond King Master Franchise — UI/UX Screen Specification 001

**Project:** DR-TRTT-OPS-001  
**Product:** Diamond King Master Franchise  
**Brand:** TRTT Voyage  
**Stage:** UI/UX concept prototype  
**Date:** 2026-11-27  
**Prototype:** [Command Center standalone HTML](../prototypes/diamond-king-command-center/index.html)

## 1. Design goal

Translate the approved product universe into a tangible first interface. The Command Center should make the product's structure understandable at a glance and guide the Owner from learning to original ideas, projects, and future franchise operations.

This is a front-end concept prototype. It is not a live SaaS application and has no authentication, backend, persistent data, billing, AI connection, or external integrations.

## 2. Primary information architecture

- Command Center
- Learning Universe
- Idea Universe
- SaaS Universe
- Franchise Universe (future capability)
- My Projects
- My Knowledge
- My Progress
- Settings

Global shell:
- Workspace selector (visual placeholder)
- Universal search (local interaction preview)
- Notifications (visual placeholder)
- Profile control (visual placeholder)
- Main navigation and content canvas

## 3. Command Center screen

### Header
- Workspace selector: identifies the active workspace.
- Search: entry point for future cross-universe search.
- Notifications and profile: reserved for authenticated product functions.

### Hero / universe map
- Headline: “Your Universe, Your Ideas, Your Journey”.
- Product promise: “Learn · Imagine · Build · Share”.
- Four visible destination orbs around the central Command Center: Learning, Idea, SaaS, and Franchise.
- Primary CTA: Explore the Universe.
- Secondary CTA: View Guide.

### Overview cards
1. Continue Learning — one learning path, milestone progress, resume action.
2. Your Idea Atlas — visual network motif and illustrative idea/theme counters.
3. Active SaaS Projects — project preview and illustrative delivery stages.

### Supporting panels
- Recent Activity — sample events only.
- Quick Create — learning note, idea card, project, knowledge map, team space, decision.
- Brand statement — TRTT Voyage motto.

**Data honesty:** all progress, counts, project states, and activity shown in the prototype are illustrative sample values, not live user data.

## 4. Core user flows

### Flow A — Resume learning
Command Center → Continue Learning → Learning Universe → select path → open lesson → capture note → record milestone.

### Flow B — Capture and develop an idea
Command Center → Quick Create / Idea Universe → Idea Card → add problem and hypothesis → attach evidence → connect related ideas → define experiment → record outcome.

### Flow C — Create a SaaS project
Idea Detail → Promote to Project → define audience and scope → create milestones → open SaaS Universe → add UX, technical, testing, and security deliverables.

### Flow D — Explore franchise workspace
Command Center → Franchise Universe → review future workspace template → owner configures brand and roles → invite team after tenant isolation and permission controls are implemented.

## 5. Interaction model in the prototype

Implemented front-end demonstration interactions:
- Sidebar navigation updates the hero heading and selected navigation state.
- CTA and quick-create controls show a temporary status message.
- Workspace and notification controls show clear “preview only” feedback.
- Search accepts text and shows a local preview response.

Not implemented:
- Route changes, saved records, real search, user accounts, invitations, server actions, AI responses, file upload, analytics, or franchise administration.
- Interactions intentionally do not claim to save or create real records.

## 6. Visual system

Core palette:
- Royal Midnight #11152D — primary canvas
- Pink #E98BAF — selected navigation and learning emphasis
- Piyaji #B77991 — secondary emphasis
- Kathali #D6A542 — primary action and milestones
- White #FFFFFF — primary text and surfaces
- Accent Cyan #67E8F9 — technical/SaaS emphasis
- Accent Diamond Gold #FFD700 — restrained premium highlight

Visual direction:
- Dark, premium, cosmic workspace with restrained orbit/diamond motifs.
- Clear card hierarchy and readable content over decorative effects.
- Desktop sidebar and compact mobile navigation.
- Single-column mobile layout; multi-column dashboard at wider widths.
- Reduced-motion preference supported.
- Semantic landmarks, labelled controls, keyboard-operable buttons, and visible focus treatments.

## 7. Responsive behavior

- Wide desktop: fixed-width navigation rail, sticky top bar, three-column overview and supporting panels.
- Tablet: compact navigation and two-column cards.
- Mobile: horizontal compact navigation, stacked cards, simplified hero/orbit presentation, and full-width content.
- Reduced motion: smooth scrolling and transitions are reduced when requested by the operating system.

## 8. Accessibility and QA checklist

Source-level review:
- [x] HTML5 document declaration and language attribute.
- [x] Viewport metadata.
- [x] Semantic navigation, main, header, section, article, and footer landmarks.
- [x] Accessible names for search, notifications, and profile controls.
- [x] Keyboard-operable buttons and search input.
- [x] Navigation selected state communicated with aria-current.
- [x] Live status feedback uses aria-live.
- [x] Reduced-motion media query.
- [x] Responsive breakpoints for tablet and mobile.

Not tested:
- [ ] Browser rendering and screenshot comparison.
- [ ] Real Android/iOS device touch testing.
- [ ] Cross-browser testing.
- [ ] Automated accessibility audit and manual screen-reader testing.
- [ ] Performance/Lighthouse.
- [ ] Production hosting or deployment.

## 9. Next design deliverables

1. Learning Universe screen and lesson/skill-map states.
2. Idea Atlas canvas and Idea Detail screen.
3. SaaS Project Studio and project lifecycle views.
4. Franchise workspace setup and permission matrix.
5. Shared design tokens and component library.
6. Click-through flow connecting the screens.

## 10. Acceptance criteria

- The prototype loads as a standalone HTML file without external assets.
- The five product spaces are visible and understandable.
- Navigation and quick actions provide truthful local feedback.
- Illustrative data is labelled as sample/demo content.
- Layout adapts to mobile, tablet, and desktop breakpoints in source.
- No feature is described as live when it is only a visual placeholder.

**Status:** Source prototype and specification created; visual rendering/device QA NOT TESTED.


## Implementation addendum — 2026-11-28

The Command Center navigation now links directly to the Learning Universe and Idea Universe screens. The primary learning and idea actions open those working screens rather than displaying a fake navigation result. Dynamic navigation headings are constructed with DOM text nodes rather than HTML string insertion.

The Learning Universe and Idea Universe now provide useful single-browser workflows:
- Idea capture: save up to 100 records in localStorage, view, delete, and export JSON.
- Learning plans: save up to 100 tasks, optionally attach HTTPS source URLs, mark/reopen completion, delete, calculate self-recorded progress by pathway, and export JSON.
- Both screens use safe text-node rendering, visible keyboard focus, and clear local-only storage disclosures.
- These are local browser prototypes, not a server database, cloud sync, user account, secure vault, or production SaaS. Clearing browser data may erase records; export backups. Do not store secrets or sensitive personal data.
- Source syntax and mock-DOM workflow tests were run for save/delete and save/complete/progress. Real browser, cross-device, screen-reader, export-download, and production QA remain NOT TESTED.
