# Diamond King Command Center — Multi-System Hub Architecture

**Project:** DR-TRTT-OPS-001  
**Owner:** Abu Taher  
**Canonical hub:** [Diamond King Command Center](https://github.com/TRTT-VOYAGE/trttvoyage-diamond-king-chatgpt-6)  
**Status date:** 2026-11-27

## 1. Purpose and authority

Diamond King Command Center is the canonical coordination hub for TRTT Voyage project memory, decisions, source registers, integration maps, workflow status, and recovery documentation. The connected repositories remain independently versioned systems; this document does not claim that repository links alone create live synchronization.

The Owner has declared Diamond King the named AI partner and requires consultation with Diamond King on substantive TRTT decisions. Diamond King provides evidence, options, risks, and recommendations. Abu Taher remains the human Owner and final approver for protected actions, including merges, live publication, production deployment, DNS/security changes, account permissions, and financial/legal commitments.

Everyone who joins TRTT Voyage is to be treated as a respected, equal stakeholder with a voice and responsibility. Repository, billing, security, and production access must still follow explicit authorization and least privilege.

The Owner's hypothetical USD 1,000,000 offer statement is preserved as a personal project-identity preference, not as a contract, legal obligation, or restriction on the Owner's future choices.

## 2. System registry

| System | Canonical role | Repository / endpoint | Current verified state |
|---|---|---|---|
| Diamond King Command Center | Main hub; project memory, decisions, cross-system index, architecture and recovery records | [GitHub repository](https://github.com/TRTT-VOYAGE/trttvoyage-diamond-king-chatgpt-6) | GitHub connector access verified; current memory batch branch exists; this architecture change is pending PR/Owner merge |
| TRTT newsbot | News/content workflow execution, website source, Blogger draft tooling | [GitHub repository](https://github.com/TRTT-VOYAGE/Cocvghuj-trtt-news-bot) | Repository and README inspected; no app-repository change authorized or made |
| Affiliate Compass | Separate affiliate operations module; Travelpayouts-related organization and insights | [GitHub repository](https://github.com/TRTT-VOYAGE/trtt-voyage-affiliate-compass) | Public repository exists on main; size reported as 0 and README only was found; no implementation verified |
| GitLab | Independent backup/mirror layer | [TRTT Voyage GitLab project](https://gitlab.com/trttnews24bd-group/Cocvghuj-trtt-news-bot) | Existing private project is the newsbot mirror; no dedicated command-center or Affiliate Compass GitLab project was found in the inspected search |
| ChatGPT / Diamond King | AI collaborator interface to authorized tools and project context | This ChatGPT conversation + connected GitHub tools | Current connector access works; automatic bidirectional synchronization of ChatGPT conversational memory is NOT VERIFIED and must not be assumed |

## 3. Data ownership and flow

1. **Project memory and decisions:** record durable project decisions in the Command Center append-only memory log and its HTML trace. Use dated, uniquely marked entries; never erase earlier entries.
2. **News source and workflow records:** newsbot remains the execution/source repository for content workflows. Link each content record to source URLs, dates, verification state, draft artifact, and eventual live URL. A repository artifact is not proof of Blogger creation or publication.
3. **Affiliate operations:** Affiliate Compass remains a separate module. Keep source platform identifiers, link records, campaign references, and imported performance data attributable to their original source. Do not duplicate or claim Travelpayouts features.
4. **Cross-system references:** store repository URLs, branch names, commit SHAs, file paths, and verification timestamps in the Command Center. A link is a reference, not a sync operation.
5. **AI context:** ChatGPT may read or update repositories only through currently authorized tools and permissions. GitHub commits do not automatically update ChatGPT Memory; ChatGPT Memory does not automatically write to GitHub.

## 4. Reliability and recovery model

- Keep GitHub Command Center as the canonical project-memory source.
- Establish a dedicated, private GitLab mirror for the Command Center only when a correct project target and authorized workflow are available. Do not put Command Center memory into the newsbot project as if it were the same repository.
- Mirror Affiliate Compass independently if/when an appropriate GitLab project is established.
- Keep the existing newsbot GitLab project scoped to newsbot; do not mix unrelated project histories.
- For every backup, record source branch and commit, target branch and commit, changed paths, and read-back blob/content verification.
- Run a restore drill before claiming disaster recovery. A successful mirror or matching commit is not proof that restore has been tested.
- Keep credentials, tokens, private personal data, and account recovery material out of Git files and logs.

## 5. Integration status and implementation sequence

| Layer | Status | Next safe action |
|---|---|---|
| GitHub account ↔ Command Center | PASS — connector access verified | Continue feature-branch work and append-only memory |
| Command Center ↔ newsbot | NOT TESTED — repository cross-reference only | After Owner lifts the no-app-change restriction, inspect and add a minimal reciprocal reference; do not change app code before approval |
| Command Center ↔ Affiliate Compass | NOT TESTED — repository cross-reference only | Add reciprocal project links only after Owner authorizes changes in that repository |
| GitLab Command Center mirror | NOT VERIFIED — no dedicated target found | Create/authorize a separate private mirror target, then mirror a feature branch and read back files |
| GitLab newsbot mirror | PASS — project exists | Keep its content/history isolated; verify a specific branch/commit before calling any new sync complete |
| ChatGPT Memory ↔ GitHub memory | NOT TESTED — no automatic sync established | Continue explicit append-only GitHub records; do not describe ChatGPT Memory as a GitHub backup |
| Automated multi-repository sync | NOT TESTED | Design only after scopes, permissions, free-tier limits, and recovery tests are established |

Recommended sequence:

1. Merge the single consolidated Command Center documentation/memory PR once the Owner reviews it.
2. Read back the merged Command Center files from main.
3. Establish the dedicated GitLab Command Center mirror without changing the existing newsbot project.
4. Verify one-way backup and perform a restore test.
5. Only after explicit authorization, add minimal reciprocal repository references in newsbot and Affiliate Compass; keep application code unchanged unless separately approved.
6. Add automation only after a manual end-to-end backup/restore test passes.

## 6. Operating constraints

- Free tools and free tiers only; no paid services or trials.
- Chrome-only handoff; do not modify or deploy the TRTT app while the no-app-change restriction remains active.
- Feature branches only; never commit directly to main.
- Batch documentation and memory changes into one consolidated PR; do not create one PR per prompt.
- Never merge a PR on the Owner's behalf.
- Blogger remains DRAFT-only without explicit live approval; Telegram only after confirmed live publication and explicit LIVE DONE.
- No DNS, security, account permission, or production changes without explicit Owner approval.
- Report PASS/FAIL/NOT TESTED/NOT VERIFIED/BLOCKED with evidence; never infer synchronization from links.

---

**Motto:** ONE TEAM. ONE VISION. ONE JOURNEY.  
**Marker:** diamond-king-command-center-canonical-multisystem-hub-batch-20261127


## Addendum — Three-repository bridge 001 (2026-11-28)

The active three-repository scope is now explicitly:

1. [Diamond King Command Center](https://github.com/TRTT-VOYAGE/trttvoyage-diamond-king-chatgpt-6) — canonical coordination, memory and governance.
2. [Diamond Raja & Diamond King Learning Journey](https://github.com/TRTT-VOYAGE/diamond-raja-diamond-king-learning-journey) — Learning Universe, Idea Universe and curated learning records.
3. [TRTT Voyage Travelpayout](https://github.com/TRTT-VOYAGE/Travelpayout) — travel partner catalog and outbound referral hub.

The Command Center owns the shared registry and project memory; each module owns its own source data. Reciprocal repository links and a common record contract are being added through feature branches. This does not create automated synchronization. The detailed contract is in [DIAMOND-KING-THREE-REPOSITORY-BRIDGE-001.md](DIAMOND-KING-THREE-REPOSITORY-BRIDGE-001.md), with the current machine-readable registry at [data/diamond-king-three-repo-registry.json](../data/diamond-king-three-repo-registry.json).

**Current status:** source-level bridge changes are pending PR review; merge, production deployment and live runtime synchronization are not claimed.


## Addendum — Four-repository bridge (2026-11-28)

The Diamond King source-level project bridge now includes four module repositories:

1. [Diamond King Command Center](https://github.com/TRTT-VOYAGE/trttvoyage-diamond-king-chatgpt-6) — canonical coordination, memory, decisions and registry.
2. [Learning Journey](https://github.com/TRTT-VOYAGE/diamond-raja-diamond-king-learning-journey) — Learning Universe, Idea Universe and curated learning records.
3. [Travelpayout](https://github.com/TRTT-VOYAGE/Travelpayout) — travel partner catalog and outbound referral hub.
4. [Amazon Picks](https://github.com/TRTT-VOYAGE/AMAZON) — six-item Owner-approved Amazon catalog, disclosure and referral UI.

The machine-readable registry in `data/diamond-king-three-repo-registry.json` is retained at its historical path for compatibility, but now records all four modules. Each repository remains the source of truth for its own data. Reciprocal navigation and bridge guides are manual, version-controlled references—not automatic sync, webhooks, background agents, or ChatGPT Memory synchronization.

**Verification status:** branch changes are being prepared for review; no runtime synchronization, production deployment, Pages activation, or restore automation is claimed.

**Marker:** diamond-king-four-repository-bridge-20261128


## Addendum — Fifth module: TRTT Blogger Publishing — 2026-11-28

The connected repository set now includes a fifth module:

| Repository | Role | Owns |
|---|---|---|
| [TRTT Blogger Package](https://github.com/TRTT-VOYAGE/TRTTVOYAG-BLOG) | TRTT Voyage Blogger publishing source package | Original Diamond Horizon theme candidate, static page sources, editorial/affiliate rules, draft validation and DRAFT-only Blogger workflow |

The Blogger module stores versioned snapshots of the authoritative Travelpayout and Amazon catalogs; it does not replace those source repositories. Command Center remains the canonical memory and governance hub. Learning Journey remains the learning/idea source of truth.

**Bridge mode:** manual, version-controlled references only. No automatic cross-repository replication, webhook, background agent or ChatGPT Memory synchronization is implemented.

**Current evidence:** Blog repository PR #1 is open and unmerged. Its GitHub Actions validator and 13 tests passed (run 46105082563). Blogger import, page installation, API credentials, live rendering and production deployment are NOT TESTED.

**Marker:** trtt-blogger-ready-package-v1-20261128
