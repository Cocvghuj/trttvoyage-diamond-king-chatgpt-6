# Learning Universe & Idea Universe — Screen Specification 001

Project: DR-TRTT-OPS-001  
Repository: TRTT-VOYAGE/trttvoyage-diamond-king-chatgpt-6  
Prototype branch: feature/learning-idea-universe-rebased-20261128  
Date: 2026-11-27

## Purpose
Extend the Diamond King Command Center with two dedicated spaces under the product principle Learn → Imagine → Build → Share.

## Screens
- `prototypes/diamond-king-universe/learning.html`: learning pathways, lesson/library preview, learning evidence principles.
- `prototypes/diamond-king-universe/ideas.html`: idea atlas, lifecycle, idea intake form, local-only preview.

## Shared design
Royal Midnight #11152D, Pink #E98BAF, Piyaji #B77991, Kathali #D6A542, White #FFFFFF; Cyan #67E8F9 accent. Responsive 12-column desktop grid collapsing to one column on narrow screens. Semantic landmarks, labelled controls, visible focus behavior from native controls, aria-live status, and reduced-motion support.

## Interaction boundary
All interactions are local prototype behavior. The idea intake form only renders a preview in the current page; it does not persist, transmit, or create a backend record. Learning pathways and progress bars are illustrative and intentionally show no completed progress.

## Data and security
No authentication, database, user profile, cloud sync, AI integration, billing, franchise tenant isolation, or external connector is present. No secrets or personal contact details included.

## Acceptance checks
- HTML5 document structure, language, viewport and theme metadata.
- Navigation links between Command Center, Learning, and Ideas.
- Responsive layout and reduced-motion CSS.
- Form labels and live status feedback.
- Clear sample-data and local-preview disclosures.
- No deletion, redirects, auto-publication, or production actions.

## QA status
Source-level inspection only. Browser rendering, Android/iOS device QA, cross-browser QA, screen-reader audit, Lighthouse, and production deployment are NOT TESTED.
