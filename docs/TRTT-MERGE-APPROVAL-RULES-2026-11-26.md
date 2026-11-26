# TRTT Voyage — Mandatory Owner-Merge Policy
**Rule ID:** TRTT-MERGE-BY-OWNER-001  
**Effective date:** 2026-11-26  
**Status:** ACTIVE

## 1. Core rule
Every repository change prepared by the DIAMOND KING agent must be submitted to the repository owner for review through a GitHub Pull Request (PR), called a Merge Request in some platforms. The owner makes the final merge decision.

## 2. No direct merge
- Never merge a PR into `main`, the default branch, or another protected/integration branch on the owner's behalf.
- Never bypass review, branch protection, required checks, or approval rules.
- Never use auto-merge or enable an automatic merge queue for agent-created work.
- A PR being green, mergeable, or approved does not authorize the agent to merge it. Only the owner performs the merge.

## 3. Every-work PR requirement
For every task that changes tracked repository content—including code, website/theme files, blog drafts, documentation, workflows, configuration, tests, and memory/decision logs—the agent must:
1. Inspect the target repository, current branch, and relevant existing files before editing.
2. Preserve history and existing content. Append or add by default; do not delete or overwrite unless the owner explicitly authorizes that exact change.
3. Make changes on a dedicated feature/work branch, never directly on `main`.
4. Verify the changed files by reading them back from GitHub and report tests as PASS, FAIL, or NOT TESTED.
5. Open a PR from the work branch to the intended integration branch (normally `main`, unless the owner specified another target).
6. Send the owner the direct PR link, source and target branches, concise change summary, verification evidence, and any known risks.
7. Stop and leave the PR open for the owner. Do not merge it.

If a PR already exists for the same source and target branches, update that PR with the new commits and send the existing PR link rather than opening duplicates.

## 4. No-change and blocked cases
- If no repository content changes, no PR is required; explain that no files were changed.
- If repository access, permissions, branch state, or conflicts prevent a PR, report the exact blocker. Do not claim a PR was created.
- Do not create a PR against a different repository merely to work around missing access. Identify the repository mismatch and ask the owner to connect the intended repository.
- Never expose secret values. Use secret names only.

## 5. Owner's merge checklist
Before merging, the owner should review the PR diff, confirm there are no unintended deletions or secret leaks, inspect relevant tests/checks, and verify the target branch. Merge only when satisfied.

## 6. Explicit boundary
The agent is responsible for preparing, verifying, and submitting the PR. The repository owner is responsible for the final merge. This rule applies to all future TRTT Voyage repository work unless the owner explicitly changes it.

**TRTT Voyage — ONE TEAM. ONE VISION. ONE JOURNEY.**
