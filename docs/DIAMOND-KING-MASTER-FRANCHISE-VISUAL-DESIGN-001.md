# Diamond King Master Franchise — Visual Product Design Specification

**Project:** DR-TRTT-OPS-001  
**Product concept:** Diamond King Master Franchise  
**Brand:** TRTT Voyage — From Vision to Global Brand! Explore Beyond. Discover Everything.  
**Motto:** ONE TEAM. ONE VISION. ONE JOURNEY.  
**Status:** Initial visual/product direction — concept, not a production implementation  
**Date:** 2026-11-27

## 1. Product North Star

Build a visual, interactive digital universe where a person can learn, capture original ideas, turn ideas into projects, collaborate with AI, and—where appropriate—share or operate a branded workspace.

The product must not become a wall of articles. Knowledge should be explorable through maps, timelines, canvases, project spaces, galleries, progress views, and connected records.

**Experience promise:** Learn → Imagine → Build → Share.

**Ownership principle:** The human founder owns their ideas, workspace, data, and decisions. AI supports research, organization, explanation, prototyping, and review; it does not claim human ownership or make protected decisions.

## 2. Product Universe / Information Architecture

The central **Diamond King Command Center** connects five primary spaces:

1. **Command Center** — overview, notifications, recent activity, decisions, workspace switcher, and system health.
2. **Learning Universe** — learning paths, lessons, skill map, notes, milestones, source library, and learning timeline.
3. **Idea Universe** — idea vault, visual canvas, linked concepts, experiments, opportunity board, and decision journal.
4. **SaaS Universe** — projects, product briefs, UX flows, design system, code workspace, data architecture, testing, security reviews, and release evidence.
5. **Franchise Universe** — future multi-workspace administration, brand customization, member roles, templates, partner operations, and aggregate analytics.

Supporting spaces: **Knowledge Map**, **Prototype Gallery**, **Community**, **Reports**, **Settings & Privacy**, and **Help / Learning Guide**.

Do not mix unrelated personal/family experiments or separate TRTT products into the core homepage. They may be linked as separately permissioned workspaces when deliberately added.

## 3. Primary Navigation and Screen Inventory

### Global shell
- Left navigation rail on desktop; compact drawer/bottom navigation on mobile.
- Top bar: workspace switcher, universal search, create action, notifications, profile and help.
- Main canvas: context-aware content with breadcrumbs and clear page titles.
- Persistent quick-create: Note, Idea, Learning Item, Project, Decision, Experiment.
- Command palette: keyboard-accessible navigation and actions.

### Core screens
- **Home / Command Center:** welcome, continue learning, recent ideas, active projects, next actions, activity timeline.
- **Learning Map:** visual nodes grouped by path/topic; progress, prerequisites, source references, and personal notes.
- **Learning Studio:** lesson/content view with notes, questions, practice tasks, and completion evidence.
- **Idea Atlas:** zoomable canvas, cards, links, tags, clusters, status, and origin/history.
- **Idea Detail:** problem, hypothesis, audience, evidence, risks, next experiment, linked learning and projects.
- **Project Studio:** overview, milestones, tasks, files, team, decisions, design and release evidence.
- **Visual Workshop:** wireframes, screen inventory, design tokens, prototype links, and review comments.
- **Knowledge Graph:** searchable relationships across lessons, ideas, projects, decisions, and sources.
- **Franchise Studio (future):** tenant/workspace creation, brand settings, template catalogue, member invitations, role management, and usage reporting.
- **Account & Privacy:** data export, deletion request workflow, consent, integrations, access log, and security settings.

## 4. Key User Flows

### A. Learn and retain
Open Learning Universe → choose a path → study a lesson → capture a note/question → connect it to a skill or idea → record practice → review progress.

### B. Turn an idea into a project
Create an idea → describe the problem and intended user → attach evidence → map related ideas → choose an experiment → record outcome → promote to project → create milestones and deliverables.

### C. Build a SaaS product
Create product brief → define user roles and jobs → map user flow → create wireframes → approve design specification → plan schema and APIs → implement → test → threat-model → release review.

### D. AI collaboration
User explicitly selects workspace context and asks for help → AI proposes a draft/analysis → sources and uncertainty are visible → user edits/accepts/rejects → decision is recorded with author and timestamp. No silent publishing, merging, billing, permission escalation, or production deployment.

### E. Franchise workspace (future)
Owner creates a workspace from an approved template → sets brand identity → invites members with least-privilege roles → configures allowed modules → reviews usage and audit events. Each workspace must have tenant isolation.

## 5. Visual Identity

### Palette
Use the established TRTT palette:
- Pink: #E98BAF
- Piyaji: #B77991
- Kathali / Gold: #D6A542
- Royal Midnight: #11152D
- White: #FFFFFF

Cyan #67E8F9 and Diamond Gold #FFD700 may be used sparingly as accents, not as replacements for the core palette.

### Visual language
- Premium editorial + futuristic workspace; spacious, structured, and readable.
- Royal Midnight backgrounds for command/overview contexts; white surfaces for focused reading and editing.
- Pink for learning and human-centered actions; Piyaji for secondary emphasis; Kathali for milestones and important highlights.
- Diamond/orbit motifs are reserved for navigation, universe maps, and meaningful transitions—not every card.
- Use real interface hierarchy, clear labels, restrained glow, consistent spacing, and strong contrast. Avoid clutter and decorative effects that obscure content.

### Typography and components
- Use a legible system sans-serif for product UI; reserve a restrained display face for brand headlines.
- Define tokens for type scale, spacing, radii, shadows, borders, and focus states.
- Standard components: buttons, inputs, cards, tabs, breadcrumbs, status chips, dialogs, side panels, empty states, charts, timeline items, graph nodes, and responsive navigation.
- Every interactive control needs hover, focus-visible, active, disabled, loading, success, and error states where relevant.

### Responsive behavior
- Mobile-first; preserve the primary task on narrow screens.
- Desktop: persistent navigation rail and multi-column workspace.
- Tablet: collapsible rail and two-column layouts where useful.
- Mobile: single-column content, drawer/bottom navigation, full-screen editor/canvas modes, large touch targets, and no horizontal page overflow.

### Accessibility baseline
- Semantic HTML and heading order.
- Keyboard navigation and visible focus.
- Text and controls meet WCAG contrast expectations.
- Every icon-only control has an accessible name.
- Respect reduced-motion preferences.
- Do not use colour alone to communicate status.
- Graph/canvas views must have a list or structured alternative.

## 6. Product Writing and Content Standards

All product-facing documentation, interface copy, onboarding, help content, and public materials are written in clear English. Use plain language, explain unfamiliar terms, show examples, and label conceptual or unverified features honestly.

Required documentation set as the product matures:
- Product vision and PRD
- Personas, jobs-to-be-done, and user stories
- Information architecture and user flows
- Wireframes and design specification
- Brand guide and component library
- Technical architecture and API contracts
- Database schema and data dictionary
- Test strategy, test cases, and release checklist
- Threat model, privacy notice, permissions matrix, and incident process
- Pricing research, SaaS business model, and launch plan
- Franchise operating model and partner handbook

## 7. Data and Architecture Concepts

Initial domain entities (planning only):
- User, Workspace, Membership, Role, Permission
- LearningPath, Lesson, Skill, LearningRecord, Note
- Idea, ConceptLink, Experiment, Evidence, Decision
- Project, Milestone, Task, Artifact, Review
- Source, Attachment, Comment, ActivityEvent, AuditEvent
- BrandTheme, WorkspaceTemplate, Plan, Entitlement, UsageRecord

Design requirements:
- Workspace-scoped records and explicit ownership.
- Tenant isolation before any multi-tenant launch.
- Server-side authorization on every protected operation.
- Version history for important user-authored records.
- Export and deletion workflows.
- Backups and tested recovery before production use.
- No claim of automatic private ChatGPT conversation synchronization. Only user-selected and authorized content may be imported through a supported integration.

No database engine, hosting provider, billing provider, or production architecture is selected by this visual specification.

## 8. Security, Privacy, and Governance

- Default to private workspaces and least-privilege roles.
- Separate Owner, Workspace Admin, Editor, Contributor, Viewer, and AI Assistant capabilities.
- AI access must be scoped to the current workspace and explicitly shared context.
- Record consequential actions in an audit trail.
- Require explicit confirmation for external publication, destructive actions, permission changes, payments, and production releases.
- Protect secrets in managed secret stores; never put credentials in source code or logs.
- Define retention, export, deletion, consent, and incident-response policies before public launch.
- Perform threat modelling and security testing before enabling multi-tenant or franchise operations.

## 9. Business Model — Hypotheses, Not Validated Pricing

Potential future tiers:
- **Personal:** individual learning and idea workspace.
- **Creator:** expanded projects, visual tools, and export.
- **Team:** collaboration, shared libraries, and team administration.
- **Franchise / Partner:** branded workspaces, templates, tenant administration, and partner support.

Do not publish prices or promise franchise rights until competitor research, cost modelling, legal review, support capacity, and willingness-to-pay research are completed. Avoid presenting a conceptual tier as an available product.

## 10. Delivery Roadmap

1. **Foundation:** approve product vision, information architecture, roles, and design tokens.
2. **Visual prototype:** clickable Command Center, Learning Universe, Idea Universe, and Project Studio.
3. **MVP:** authentication, private workspace, learning records, idea vault, project records, search, and export.
4. **AI assistance:** scoped retrieval, draft generation, source display, and human approval.
5. **Collaboration:** invitations, roles, comments, and audit events.
6. **Franchise readiness:** tenant isolation, workspace templates, branding, entitlements, operational tooling, and legal review.
7. **Launch:** accessibility, security, reliability, support, pricing validation, and controlled rollout.

Each phase requires its own acceptance criteria and evidence. A concept image or static prototype is not proof of a functioning SaaS.

## 11. Acceptance Criteria for the First Visual Prototype

- A user can understand the five core spaces without reading a long explanation.
- Command Center links to Learning, Ideas, SaaS Projects, and the future Franchise area.
- At least one representative screen exists for each core space.
- The learning map and idea canvas have accessible structured alternatives.
- Mobile and desktop layouts are specified.
- Design tokens use the approved palette and consistent components.
- Empty, loading, error, and populated states are represented.
- No nonfunctional control is presented as working.
- No live integration, account system, payment, AI sync, or deployment is claimed unless implemented and tested.

## 12. Current Evidence and Limitations

- A first visual concept image was generated in the conversation on 2026-11-27 to establish the broad visual direction.
- This document is a product/visual specification only.
- No production code, database, authentication, tenant isolation, billing, external integration, browser-rendered prototype, or deployment was created or tested by this document.
- The image is a concept reference, not a final logo, approved brand asset, or pixel-perfect UI specification.

**Project link:** https://trttvoyage.com  
**Motto:** ONE TEAM. ONE VISION. ONE JOURNEY.
