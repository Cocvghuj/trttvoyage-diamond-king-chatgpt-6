# Security Baseline and Threat Model

**Project:** DR-TRTT-OPS-001 · **Repository:** Diamond King Command Center

## Purpose
This is a security design baseline for a public project hub and its GitHub automation. It is not a certification and does not prove that platform settings are enabled.

## Assets
- Source, documentation, issue and pull-request history.
- Workflows, tokens, artifacts and deployment credentials.
- Owner/contributor accounts, permissions and recovery paths.
- Private project information, personal data and unpublished content.
- Default-branch integrity and release artifacts.

## Threats and controls

| Threat | Required control |
|---|---|
| Credential exposure | Never commit secrets; rotate exposed credentials immediately |
| Workflow privilege abuse | Least-privilege permissions; do not expose secrets to untrusted PR code |
| Dependency compromise | Dependabot; review dependency provenance and permissions |
| Prompt/content injection | Treat external content as untrusted data; validate inputs; never execute arbitrary supplied commands |
| Unauthorized changes | Feature branches, PR review, required checks and rulesets where available |
| Privacy leakage | Data minimization, redaction and private reporting |
| Supply-chain tampering | Review actions, artifacts and release inputs |

## Required controls
1. Set least-privilege permissions in every workflow.
2. Separate untrusted PR validation from privileged publishing.
3. Review third-party actions; pin high-assurance production actions to full immutable commit SHAs.
4. Validate user-controlled input and avoid unsafe shell interpolation.
5. Keep credentials and personal/private data out of public files, issues and logs.
6. Review static-analysis and dependency alerts.
7. Use protected environments and explicit approvals for production.
8. Keep auditable change, test, limitation and recovery records.

## GitHub settings status
The rulesets API returned an empty list for both central repositories at inspection. Branch-protection read returned HTTP 403, so protection status is NOT VERIFIED. The following are also NOT VERIFIED: required checks, force-push restrictions, Dependabot alerts, secret scanning, push protection, private vulnerability reporting, Actions policy and account-level 2FA/recovery.

Verify in repository Settings → Rules / Branches, Settings → Advanced Security, and Settings → Actions. Availability depends on plan, visibility and organization policy. Policy files do not activate these settings.

## Incident response
1. Triage affected files, workflow, branch and exposure window.
2. Revoke/rotate exposed credentials at the provider.
3. Isolate a vulnerable workflow when safe and authorized.
4. Preserve evidence without copying secrets or personal data.
5. Patch through a focused PR, run checks, and read back after merge.
6. Record impact, remediation, remaining risk and lessons.

## Release checklist
- [ ] No secrets or private data in diff, logs or artifacts.
- [ ] Workflow permissions are least privilege.
- [ ] Actions and dependencies are reviewed.
- [ ] Relevant tests/security analysis passed or limitations are explicit.
- [ ] Platform security settings are verified, not assumed.
- [ ] Production actions have separate Owner approval.
- [ ] Recovery steps are documented.
