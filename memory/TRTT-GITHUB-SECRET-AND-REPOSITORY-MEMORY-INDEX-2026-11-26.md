# TRTT Voyage — GitHub Repository, Secret-Reference & Memory Index
**Record ID:** TRTT-GITHUB-MEMORY-INDEX-001  
**Audit date:** 2026-11-26  
**Status:** Initial evidence-backed inventory  
**Primary memory repository:** `Cocvghuj/trttvoyage-diamond-king-chatgpt-6`  
**Related automation repository inspected:** `Cocvghuj/Cocvghuj-trtt-news-bot`

## 1. Why this record exists
This index explains which named records and files are saved, why they exist, and how they fit together. It is intended to reduce repeated explanations and help future AI-assisted work use the correct rules, files, branches, and service references.

This is a public-safe index. It contains secret *names and purposes only*, never secret values, tokens, private keys, passwords, OAuth credentials, or personal account data.

## 2. Core operating records in this repository

| Saved name / Record ID | Repository path | Why it exists / how it is used |
|---|---|---|
| `TRTT-3TRIGGER-FINAL-001` | `docs/TRTT-FINAL-OPERATING-RULES-THREE-TRIGGERS-2026-11-26.md` | Defines the three owner-facing stages: Trigger 1 work authorisation/build-and-save; Trigger 2 the specifically approved GitHub deployment; Trigger 3 approved Blog publication. It says not to invent extra triggers and requires evidence-based reporting. |
| `TRTT-MERGE-BY-OWNER-001` | `docs/TRTT-MERGE-APPROVAL-RULES-2026-11-26.md` | Every agent-authored repository change goes through a feature branch and PR. The owner alone makes the final merge decision. No agent merge, auto-merge, or direct Main commit. |
| `TRTT-AUTOMATION-VISION-001` | `docs/TRTT-VOYAGE-AUTOMATION-VISION-2026-11-26.md` | Keeps the real goal clear: build durable free tools and reusable automation that reduce repeated phone/manual work; do not turn the owner into a daily manual publisher. |
| Project Charter | `docs/PROJECT-CHARTER.md` | Defines the repository as a public-safe handbook, its values, scope, prohibited sensitive data, and approval boundaries. |
| Evidence-first workflow | `docs/WORKFLOW.md` | Standard sequence: inspect → plan → build → diff review → validate → save → read back → report. |
| Repository map | `docs/REPOSITORY-MAP.md` | Explains which repository areas are public handbook, private vault, or product source. |
| Daily workflow-builder memory | `memory/TRTT-DAILY-MEMORY-2026-11-26.md` | Records the TRTT Magic Workflow Builder work, source checks, limitations, and pending deployment/publication stages. |
| Daily packing-planner memory | `memory/TRTT-DAILY-MEMORY-2026-11-26-PACKING-PLANNER.md` | Records the free packing tool, files, design, privacy approach, and tests not yet performed. |

## 3. Saved tools and content — what each is for

| Name / path | Purpose | Current limitation / status |
|---|---|---|
| `trttmagic.html` | Browser-only TRTT Magic Workflow Builder: edit workflow steps, check required stages, preview/copy/export JSON. | Planning/export utility only; it does not connect to GitHub, Blogger, Make.com, or run automations. |
| `Diamond King/trttmagic.html` | Requested Diamond King folder copy of the workflow-builder HTML. | Source copy; not a separate automation service. |
| `tools/trtt-trip-packing-planner.html` | Free trip packing checklist with trip/weather options, progress, text export, and print. | Browser-only; no remote API or account integration. |
| `blog/drafts/TRTT-MAGIC-WORKFLOW-BUILDER-2026-11-26.html` | Blogger-ready article draft about the workflow builder. | Draft only; not published. |
| `blog/drafts/TRTT-SMART-TRIP-PACKING-PLANNER-2026-11-26.html` | Blogger-ready article draft about the packing planner. | Draft only; not published. |

## 4. Secret names referenced by the inspected automation workflows

The following names were found in workflow source files in **`Cocvghuj/Cocvghuj-trtt-news-bot`**, not in this memory repository. This is an inventory of source-code references, not proof that a matching GitHub Actions Secret currently exists or is populated.

| Exact name | Why the workflow uses it | Referenced by |
|---|---|---|
| `BLOGGER_CLIENT_ID` | OAuth client identifier used to authenticate Blogger API access. | `trtt-master-control.yml`, `trtt-news-draft.yml`, `trtt-787950-bot.yml`, `flightscoutpro-single-draft.yml` |
| `BLOGGER_CLIENT_SECRET` | OAuth client credential paired with the client ID. Treat as highly sensitive. | Same Blogger workflows above |
| `BLOGGER_REFRESH_TOKEN` | Allows the workflow to obtain a short-lived access token for Blogger API operations. Treat as highly sensitive. | Same Blogger workflows above |
| `BLOGGER_BLOG_ID` | Identifies the target Blogger blog used by the TRTT news/draft workflow. | `trtt-master-control.yml`, `trtt-news-draft.yml`, `trtt-787950-bot.yml` |
| `FLIGHTSCOUTPRO_BLOG_ID` | Identifies the separate FlightScoutPro Blogger destination. | `trtt-news-draft.yml`, `flightscoutpro-single-draft.yml` |
| `GITLAB_TOKEN` | Authenticates the GitLab backup/pipeline step in the 24/7 workflow. | `trtt-24-7-pipeline.yml` |

### Related values that are not user-created Secret names in the inspected references
- `github.token` is GitHub's workflow-provided token expression; the workflow maps it to an environment variable called `GH_TOKEN`. Do not mistake `GH_TOKEN` for proof of a separately configured repository Secret.
- `TRTT_TARGET_DATE` is a workflow input/environment setting, not a credential.
- `BLOGGER_BLOG_ID`, `FLIGHTSCOUTPRO_BLOG_ID`, and OAuth credentials must be configured for the intended workflow to work, but their actual configured status was not accessible in this audit.

## 5. How the system is intended to work

1. **Owner sends one of the three established triggers.** Use the exact scope in `TRTT-3TRIGGER-FINAL-001`; do not ask for extra triggers for routine substeps.
2. **Agent inspects first.** Check repository, branch, existing files, workflow state, and previous records.
3. **Build on a feature branch.** Keep existing history; add new dated files or additive changes.
4. **Use only the required service credentials by name.** Workflows read GitHub Actions Secrets at runtime. Never paste secret values into chat, source files, Markdown, commits, screenshots, or logs.
5. **Validate honestly.** Distinguish source inspection from a real workflow run, browser test, Blogger API result, deployment, or backup.
6. **Save to GitHub and read back.** A successful commit is not proof of deployment or publication.
7. **Open a PR for every repository change.** Include changed files, tests, risks, and read-back evidence.
8. **Owner reviews and merges.** The agent must never merge the PR.
9. **GitLab is the backup/mirror.** Check actual mirror or pipeline status separately; do not report backup success merely because a token reference exists.
10. **Blog content remains draft until the authorised publication stage.**

## 6. Security and access audit findings

- This memory repository is public and its Project Charter says it is for public-safe guidance, not credentials or private operational records.
- The related news-bot repository is also public. The workflow source files expose the *names* of credential references, but no credential values were copied into this index.
- GitHub's sensitive Secrets API is not available through the connected read interface. Therefore the actual repository/org Secret inventory, configured/not-configured state, and secret timestamps are **NOT VERIFIED**.
- The memory repository's `main` branch API reported `protected: false`; the repository rulesets endpoint returned an empty list. This means the owner-merge rule is documented but is **not technically enforced by branch protection/rulesets** at the time of this audit.
- Reading branch-protection details returned an integration permission error; the branch object's protection status and empty rulesets result are the evidence available here.
- The memory repository has no `.github/workflows/` directory on `main`; the Blogger and GitLab secret references inspected belong to the separate news-bot repository.
- GitLab backup parity for this new memory record: **NOT TESTED**.

## 7. Audit scope and limits

Inspected:
- Main branch root, `docs/`, `memory/`, `tools/`, `templates/`, and relevant Blogger draft paths in the memory repository.
- The core operating documents and daily memory records listed above.
- The workflow directory in `Cocvghuj/Cocvghuj-trtt-news-bot`, including the Blogger master/news/787950/FlightScoutPro workflows and GitLab 24/7 pipeline workflow.

Not verified:
- Actual values or existence of GitHub Actions Secrets.
- Every workflow in every GitHub repository accessible to the account.
- Organization-level secrets, environment-level secrets, or secrets in other repositories not inspected.
- Whether the GitLab token is valid, whether mirroring is enabled now, or whether a current backup completed.
- Runtime execution of Blogger publishing or GitLab backup as part of this audit.

**Security rule:** Secret values must never be requested for chat, displayed, committed, or stored in this public repository. Use exact secret names only.

**TRTT Voyage — ONE TEAM. ONE VISION. ONE JOURNEY.**
