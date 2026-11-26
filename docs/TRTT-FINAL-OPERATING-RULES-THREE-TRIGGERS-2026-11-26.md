# TRTT FINAL OPERATING RULES — THREE TRIGGERS ONLY
**Record ID:** TRTT-3TRIGGER-FINAL-001  
**Date:** 2026-11-26  
**Repository:** `Cocvghuj/trttvoyage-diamond-king-chatgpt-6`  
**Branch:** `feature/diamond-king-command-center-v1`  
**Status:** ACTIVE OPERATING RULE

## 1. Supreme rule: exactly three owner triggers
The TRTT delivery workflow has exactly these three owner-facing triggers. The assistant must not invent intermediate, fourth, fifth, or replacement triggers for the same delivery.

### TRIGGER 1 — WORK AUTHORISATION
Exact trigger:
`[TRIGGER 1 — কাজের অনুমতি]`

When the owner sends this trigger with the task or when the task is already unambiguously specified in the active conversation, the assistant is authorised to complete the safe, in-scope build-and-save stage without asking for another trigger between its substeps.

The assistant must:
1. Inspect the existing repository, branch, relevant files, and history before editing.
2. Preserve existing content and records. Use additive changes; never delete history.
3. Build the requested work on the designated feature branch.
4. Perform a diff and security review.
5. Run available relevant tests and report exact results. Never invent test results.
6. Fix issues found within the authorised scope and re-check them.
7. Save the completed work to GitHub on the feature branch.
8. Read the saved files back from GitHub and verify the content.
9. Report the commit, file links, evidence, limitations, and any genuinely blocked checks.

At the end of Trigger 1, stop before deployment and present only the established Trigger 2.

### TRIGGER 2 — GITHUB DEPLOY
Exact trigger:
`[TRIGGER 2 — GITHUB DEPLOY]`

This trigger authorises the specifically prepared and reviewed GitHub deployment/release action for the deliverable. Before acting, confirm the target, workflow, and deployment scope from repository evidence. Run the intended deployment only if the target and action are clear, available, and safe. Then verify the reported deployment result and provide evidence.

This trigger does not authorise unrelated DNS changes, security or account-permission changes, destructive operations, or changes to unrelated production systems. If a required target, workflow, credential, or check is unavailable, report BLOCKED or NOT TESTED honestly; do not simulate a deployment.

At the end of Trigger 2, stop before publishing to the Blog and present only the established Trigger 3.

### TRIGGER 3 — BLOG POST
Exact trigger:
`[TRIGGER 3 — BLOG POST]`

This trigger authorises publication of the approved, fact-checked content to the specified TRTT Blog. Verify the final content, destination, and publication result. Provide the real live URL only after confirming that the post is publicly accessible.

A saved draft is not a published post. If no supported Blogger publishing action or access is available, report BLOCKED and provide the prepared content/draft status without claiming publication.

## 2. No extra trigger rule
- These are the only three owner-facing triggers for this workflow.
- Do not ask the owner to separately trigger inspection, planning, coding, diff review, security review, fixes, tests, GitHub save, or read-back. Those are Trigger 1 substeps.
- Do not create a new trigger because the assistant changed its mind, changed the task label, or reached an internal milestone.
- Do not repeat questions when the answer is already present in the current conversation or verified project records.
- At each stage boundary, show the next exact trigger from this document—never a newly invented phrase.
- If the work is blocked, explain the specific blocker and the smallest necessary owner action. Do not disguise a blocker as a new workflow trigger.

## 3. Approval boundaries and preservation
- Trigger 1 authorises feature-branch work and GitHub save only; it does not authorise merge, production deployment, or Blog publication.
- Trigger 2 authorises the explicitly identified GitHub deployment only; it does not authorise Blog publication.
- Trigger 3 authorises the approved Blog publication only.
- Never merge to the default/Main branch unless the owner separately and explicitly authorises that merge.
- Never change DNS, account permissions, secrets, security settings, or unrelated production infrastructure under these three triggers.
- Never delete files, commits, branches, logs, memories, or historical records. Prefer new dated files or additive amendments.
- Never modify any separately designated immutable/locked file.
- Never claim that a workflow ran, a test passed, a deployment succeeded, or a post went live without direct evidence.

## 4. Reporting standard
Every stage report must use truthful status labels: `PASS`, `FAIL`, `NOT TESTED`, `BLOCKED`, or `WAITING FOR APPROVAL`.

Include:
- Trigger and authorised scope
- Repository and branch
- Files changed or added
- Commit SHA and GitHub links
- Diff/security review findings
- Tests actually run and exact outcomes
- GitHub read-back verification
- Deployment or Blog publication evidence, only when applicable
- Remaining risks and untested items

Never invent ratings, scores, URLs, prices, test outcomes, or successful external actions.

## 5. Low-interaction operating promise
The owner may provide one task instruction with Trigger 1. The assistant should use the available project context and tools to complete all safe Trigger 1 substeps in one continuous work session, minimising phone interaction and avoiding repetitive permission requests.

The assistant cannot independently send a future message or start work when no user turn or authorised automation is active. It must not imply that it can work in the background without an enabled automation. When the owner returns with one of the three triggers, continue from the verified repository state and this rule file without asking the owner to restate the workflow.

## 6. Canonical trigger card
1. `[TRIGGER 1 — কাজের অনুমতি]` — Inspect → Build → Diff/Security Review → Fix → Test → GitHub Save → Read-back.
2. `[TRIGGER 2 — GITHUB DEPLOY]` — Execute and verify the prepared GitHub deployment.
3. `[TRIGGER 3 — BLOG POST]` — Publish the approved post and verify its live URL.

**No fourth trigger. No invented intermediate trigger. Preserve history. Report only verified facts.**

---
**TRTT Voyage — From Vision to Global Brand.**  
**Explore Beyond. Discover Everything.**  
**DIAMOND RAJA 🤝 DIAMOND KING 🤝 MUSE**  
**ONE TEAM. ONE VISION. ONE JOURNEY.**
