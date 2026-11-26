# Owner PR Review Checklist — Evidence-First Mobile Review

**Project:** DR-TRTT-OPS-001  
**Purpose:** A short, repeatable review path for GitHub pull requests, especially on a phone.  
**Rule:** An open PR is a proposal, not a release. The Owner decides whether to merge.

## 1. Confirm the proposal
- [ ] Repository and PR title match the intended project.
- [ ] Base branch is the expected target (normally `main`).
- [ ] Head branch is a dedicated `feature/*` branch.
- [ ] PR is open and has not already been merged or closed.
- [ ] The summary explains the user problem and the intended outcome.

## 2. Inspect the change
- [ ] Open **Files changed** and scan every changed path.
- [ ] Each changed file is relevant to the stated task.
- [ ] No unexpected deletion, replacement, generated dump, or unrelated refactor appears.
- [ ] Existing posts, settings, workflows, memory history, and user content are preserved.
- [ ] New public content is in English and includes verified links where relevant.

## 3. Check safety and privacy
- [ ] No API keys, tokens, passwords, passphrases, cookies, or private contact details appear.
- [ ] No unapproved production, DNS, security, permission, or account changes are included.
- [ ] Blogger content remains a draft unless live publication was separately approved.
- [ ] Telegram delivery is not implied unless the live post and API delivery are confirmed.
- [ ] TRTT Voyage and FlightScoutPro data and workflows remain isolated.

## 4. Evaluate verification evidence
- [ ] The PR states the exact checks that were run.
- [ ] Test results are distinguished from static inspection and file read-back.
- [ ] Untested runtime, browser, device, external-service, and publication behavior is clearly labelled.
- [ ] Changed files were read back from the remote feature branch.
- [ ] Any known failure or blocker is visible, not hidden by a PASS summary.

## 5. Make the Owner decision
Choose one outcome:
- **Merge** only when the diff is in scope, safe, and sufficiently verified.
- **Request changes** when a specific correction is needed.
- **Hold** when evidence, dependencies, or approval are incomplete.

Do not merge merely because a PR is open, a preview exists, or a check passed. A successful merge still does not prove production deployment or Blogger publication.

## 6. Phone review sequence
1. Open the PR link.
2. Read the title and summary.
3. Open **Files changed** and inspect the full file list and diff.
4. Check the verification and known-limitations sections.
5. Review conversation comments and check status.
6. Make the Owner decision in GitHub.

## 7. After an Owner merge
- [ ] Confirm GitHub reports the PR as merged.
- [ ] Record the merge commit and verify the target branch.
- [ ] Run only the separately authorized post-merge checks.
- [ ] Mirror the approved branch/files to GitLab where required and verify the mirror.
- [ ] Keep Blogger live publishing, Telegram distribution, and production changes behind their own approval gates.

---
**Status vocabulary:** PASS = verified; FAIL = attempted and failed; NOT TESTED = not run; NOT VERIFIED = no reliable confirmation; BLOCKED = dependency prevents progress; WAITING FOR OWNER = approval required.
