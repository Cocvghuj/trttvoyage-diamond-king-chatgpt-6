# Learning Universe & Idea Universe — Screen Specification 001

Project: DR-TRTT-OPS-001  
Repository: TRTT-VOYAGE/trttvoyage-diamond-king-chatgpt-6  
Implementation branch: feature/offline-learning-idea-workflows-20261128  
Date: 2026-11-27

## Purpose
Extend the Diamond King Command Center with two dedicated spaces under the product principle Learn → Imagine → Build → Share.

## Screens
- `prototypes/diamond-king-universe/learning.html`: learning pathways, lesson/library preview, learning evidence principles.
- `prototypes/diamond-king-universe/ideas.html`: idea atlas, lifecycle, idea intake form, browser-local records and validated JSON import/export.

## Shared design
Royal Midnight #11152D, Pink #E98BAF, Piyaji #B77991, Kathali #D6A542, White #FFFFFF; Cyan #67E8F9 accent. Responsive 12-column desktop grid collapsing to one column on narrow screens. Semantic landmarks, labelled controls, visible focus behavior from native controls, aria-live status, and reduced-motion support.

## Interaction boundary
The Idea Universe stores up to 100 idea records in browser localStorage on the current device, supports deletion, and imports/exports JSON backups with validation and duplicate-ID handling. The Learning Universe stores up to 100 learning plans in browser localStorage, supports self-recorded completion, deletion, pathway progress calculation, and JSON export. Records are not uploaded, cloud-synced, or attached to an account. Clearing browser data may erase them; users should export backups. Completion is self-recorded and not externally verified. Learning pathway names are illustrative starter categories; progress bars are calculated from the user's self-recorded completed plans on this device.

## Data and security
No authentication, server database, user profile, cloud sync, AI integration, billing, franchise tenant isolation, or external connector is present. Local browser storage is not a secure vault and must not be used for secrets or sensitive personal data. No secrets or personal contact details included.

## Acceptance checks
- HTML5 document structure, language, viewport and theme metadata.
- Navigation links between Command Center, Learning, and Ideas.
- Responsive layout and reduced-motion CSS.
- Form labels and live status feedback.
- Browser-local save/delete flows, input length limits, safe text-node rendering, local storage error handling, and validated JSON import/export.
- Local-only privacy disclosure; no server or cloud-sync claims.
- Clear sample-data and local-only storage, backup restore, and sample-data disclosures.
- No deletion, redirects, auto-publication, or production actions.

## QA status
Source-level inspection only. Functional localStorage flows, browser rendering, Android/iOS device QA, cross-browser QA, screen-reader audit, Lighthouse, and production deployment are NOT TESTED.


## Re-audit hardening addendum — 2026-11-28

- Idea and Learning localStorage readers now validate non-empty IDs and content, enforce the existing field limits, and normalize stored timestamps without inventing a date. Missing or invalid timestamps are represented as unavailable rather than rendered as “Invalid Date”.
- Learning source URLs are parsed with the URL API and retained only when the parsed protocol is HTTPS; malformed or non-HTTPS stored values are cleared from the in-memory normalized record.
- JSON import accepts an empty timestamp only to preserve a legacy record whose date is unavailable; any non-empty timestamp must parse successfully. Existing valid timestamps are normalized to ISO format.
- No existing storage key or backup format version changed. Browser/device QA and real import/export picker testing remain NOT TESTED.
