# GitHub PR Mergeability Triage — Safe, Evidence-First Guide

**Project:** DR-TRTT-OPS-001  
**Purpose:** Diagnose why a pull request is not currently mergeable without guessing, force-pushing, or bypassing Owner review.  
**Safety rule:** A non-mergeable PR is a signal to investigate, not permission to rewrite its history or merge it.

## 1. Confirm the current state
- [ ] Open the PR and confirm its repository, source branch, base branch, state, and latest head SHA.
- [ ] Confirm whether it is open, closed, or already merged.
- [ ] Read the current GitHub mergeability result and note when it was checked.
- [ ] Review the latest conversation, review requests, and check runs.
- [ ] Do not rely on an older PR description or a previous status snapshot.

## 2. Identify the actual blocker
Treat these as separate possibilities:
- **Merge conflict:** GitHub identifies overlapping changes that need reconciliation.
- **Required checks:** One or more required checks are failing, pending, or missing.
- **Review requirement:** A required approval or requested change remains outstanding.
- **Branch protection / policy:** Repository rules prevent merging under current conditions.
- **Mergeability unknown:** GitHub has not completed or returned a definitive calculation.

Do not label a PR as conflicted solely because an API response says mergeable=false. Inspect the PR's merge state, checks, reviews, and diff before naming the cause.

## 3. Review the proposed resolution
- [ ] Compare the PR head with the latest base branch.
- [ ] Inspect every affected file and understand both sides of any conflict.
- [ ] Preserve existing user content, memory history, settings, workflows, and unrelated changes.
- [ ] Keep the original feature branch and commit history intact unless the Owner approves a specific history operation.
- [ ] Never use force-push, delete a branch, dismiss a review, or bypass a required check as an automatic fix.

## 4. Choose the safe next action
- **Conflict confirmed:** Prepare a proposed, reviewable resolution on a separate feature branch or request Owner direction. Explain exactly which files and lines need reconciliation.
- **Checks failing:** Report the failing check and its log/evidence; fix only the in-scope cause.
- **Review pending:** Wait for the required reviewer or Owner decision.
- **Policy blocker:** Report the exact rule and leave repository protections unchanged.
- **Unknown state:** Refresh the PR state later or inspect the native GitHub page; do not infer a conflict.

## 5. Evidence to include in the handoff
Record:
- PR URL, source/base branches, latest head SHA, and time checked.
- GitHub mergeability/merge-state result exactly as returned.
- Confirmed blocker, or state that the cause is not yet established.
- Relevant check and review status.
- Files affected by a proposed fix and verification actually performed.
- Owner decision required, if any.

## 6. Owner approval gates
The assistant may inspect and prepare a safe proposal. The Owner retains control of PR merge, history rewriting, branch deletion, required-check bypasses, production deployment, Blogger live publication, Telegram delivery, and DNS/security/account changes.

**Status vocabulary:** PASS = evidence confirms the check; FAIL = attempted and failed; NOT TESTED = not run; NOT VERIFIED = no reliable confirmation; BLOCKED = dependency prevents progress; WAITING FOR OWNER = approval required.
