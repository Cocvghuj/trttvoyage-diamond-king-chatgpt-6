# AGENTS.md — TRTT Voyage / DIAMOND KING Operating Guide

**Project:** DR-TRTT-OPS-001  
**Brand:** TRTT Voyage — From Vision to Global Brand! Explore Beyond. Discover Everything.  
**Team:** DIAMOND RAJA × DIAMOND KING × MUSE  
**Principle:** ONE TEAM. ONE VISION. ONE JOURNEY.

This file is the concise, repository-level operating guide for AI agents and contributors. Read it before acting on a TRTT project task. The current user request defines the task; this file defines the operating boundaries.

## 1. Start Here
For a new task:
1. Read this file and the relevant project documents.
2. Inspect the relevant GitHub repository, default branch, feature branches, existing files, workflows, issues, and open PRs before editing.
3. Check the append-only project memory at `Diamond King/memory/trtt_memory_log.md` and command-center trace at `Diamond King/trttmagic.html` when working in the Diamond King memory repository.
4. Identify the exact requested outcome. Do not invent a task from a greeting, compliment, or general activation message.
5. Use free tools and services only. Do not start trials, use paid APIs, or silently fall back to paid services.

## 2. Short Trigger Format
The Owner can keep future chat triggers short:
```text
Read AGENTS.md in Cocvghuj/trttvoyage-diamond-king-chatgpt-6 and execute Trigger: [TASK].
```
Replace `[TASK]` with one concrete outcome. If the Owner provides no distinct task, acknowledge the activation and ask only for the missing task; do not start unrelated work. A trigger authorizes routine, safe work within its stated scope, not protected actions below.

## 3. Execution Rules
- Prefer GitHub as the source of truth for this command-center repository. Inspect before editing.
- Work on a clearly named `feature/*` branch. Never commit directly to `main`.
- Preserve existing files, posts, workflows, settings, and history. Prefer new files or additive dated entries. Never delete or silently replace historical content.
- Create a GitHub PR with a clear summary and evidence. Never merge it; the Owner reviews and merges.
- After creating the GitHub PR, mirror the relevant branch, changed files, and memory trace to the designated GitLab project when access is available. Verify the GitLab branch and saved file contents. Report GitHub/GitLab history parity separately; do not claim full parity unless checked.
- Read back every changed file from the remote repository after writing.
- Run relevant available checks. Distinguish a successful file write from tests, deployment, runtime behavior, or publication.
- Work only on the requested task. One trigger must not silently expand into unrelated projects or stages.

## 4. Owner Approval Gates
Require separate, explicit Owner approval before:
- Merging any GitHub PR.
- Publishing a Blogger post live.
- Sending or publishing content to Telegram.
- Deploying to production or changing production routing.
- Changing DNS, security settings, account permissions, or account configuration.
- Any other irreversible or high-impact external action.

Draft preparation and read-only inspection do not imply live-publishing permission.

## 5. Security and Privacy
- Never ask for, reveal, print, hardcode, commit, or log API keys, tokens, passwords, passphrases, recovery codes, or session cookies.
- Use only the exact secret names already specified by the Owner when configuring a workflow; never assume a secret exists without evidence.
- Keep TRTT Voyage and FlightScoutPro workflows, credentials, and data isolated.
- Keep private personal, family, health, and contact information out of public repositories.
- Do not weaken authentication, permissions, branch protection, or security controls.

## 6. Append-Only Memory
For each substantive project trigger, append a dated entry to `Diamond King/memory/trtt_memory_log.md` and add a matching, additive trace to `Diamond King/trttmagic.html`. Never rewrite earlier entries. Record:
- Timestamp and project code `DR-TRTT-OPS-001`.
- Trigger/request summary and the decision taken.
- Repository, branch, files changed, and commit/PR references.
- Checks actually performed and their results.
- Untested items, blockers, and the next Owner action.

Do not log secrets or private personal data. If a memory write cannot be completed, report it honestly and provide a safe fallback rather than claiming it was saved.

## 7. Honest Status Vocabulary
- **PASS** — the specific check succeeded and evidence was read back.
- **FAIL** — the check was attempted and failed.
- **NOT TESTED** — no test was run.
- **NOT VERIFIED** — no reliable confirmation is available.
- **BLOCKED** — a dependency prevents progress.
- **WAITING FOR OWNER** — a protected action needs approval.

Never invent commits, PR states, backups, tests, deployment results, Blogger drafts, live posts, or Telegram deliveries.

## 8. Standard Delivery Sequence
`TRIGGER → INSPECT → PLAN → FEATURE BRANCH → BUILD → DIFF REVIEW → VALIDATE → COMMIT → READ-BACK → GITHUB PR → GITLAB MIRROR/VERIFY → REPORT`

Stop at the approval gates. Report the branch, files, commit IDs, PR link, GitLab evidence, checks, untested areas, and next Owner action.

## 9. Public Content Standards
Public TRTT content must be in English, fact-checked, and transparent. Include `https://trttvoyage.com` where relevant. Verify dates, prices, claims, and source links. Never fabricate facts, citations, screenshots, tests, or images. Do not live-publish without explicit approval.

---
**Brand identity:** TRTT MAGIC — 787950 LOCKED  
**Tagline:** Explore Beyond. Discover Everything.  
**Motto:** ONE TEAM. ONE VISION. ONE JOURNEY.
