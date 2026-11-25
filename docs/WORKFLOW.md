# Evidence-First Delivery Workflow

## Standard sequence
1. **TRIGGER** — identify the requested outcome and its permitted scope.
2. **INSPECT** — read the current branch, relevant files, and existing history.
3. **PLAN** — list intended additive files or changes and acceptance criteria.
4. **BUILD** — work on a feature branch; preserve existing content.
5. **DIFF REVIEW** — inspect the result for scope drift, broken links, unsafe behavior, and accidental replacement.
6. **VALIDATE** — run only checks that are available; record exact commands and results.
7. **SAVE** — commit to the feature branch and capture the commit identifier.
8. **READ-BACK** — fetch the saved files and confirm the stored content.
9. **REPORT** — state what changed, what passed, what was not tested, and the next approval gate.

## Protected actions
Do not merge to Main, publish live Blogger content, deploy to production, alter DNS, change account permissions, or modify security settings without explicit owner approval.

## File preservation
- Create a new file when a path does not exist.
- Before editing an existing file, fetch it and inspect its current contents.
- Do not delete files, branches, logs, or historical versions.
- Do not replace an existing document merely to make it cleaner; append a dated addendum or create a new version instead.

## Evidence record
Every completed task should record:
- Request / trigger
- Repository and branch
- Files added or changed
- Commit SHA
- Validation performed
- Read-back result
- Remaining risks and untested areas

## Honest completion
A commit confirms that GitHub accepted a repository write. It does not prove code compiles, tests pass, a site is deployed, or a Blogger post is live. Report each claim separately.
