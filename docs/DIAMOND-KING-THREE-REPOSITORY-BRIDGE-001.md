# DIAMOND KING — Three-Repository Bridge 001

**Project:** DR-TRTT-OPS-001  
**Human Owner:** Diamond Raja (Abu Taher)  
**AI collaborator:** Diamond King (ChatGPT)  
**Motto:** ONE TEAM. ONE VISION. ONE JOURNEY.  
**Status:** Source-level bridge specification; awaiting Owner review/merge.

## 1. Canonical topology

Diamond King Command Center is the single coordination hub. The three repositories remain separate products with separate histories and local source-of-truth data.

| Repository | Role | Owns |
|---|---|---|
| [Command Center](https://github.com/TRTT-VOYAGE/trttvoyage-diamond-king-chatgpt-6) | Central coordination, memory, decisions, system registry and governance | Cross-project decisions, integration map, append-only project memory |
| [Learning Journey](https://github.com/TRTT-VOYAGE/diamond-raja-diamond-king-learning-journey) | Learning and Idea Universe; curated human–AI learning records and product discovery | Learning chapters, public learning path, project learning artifacts |
| [Travelpayout](https://github.com/TRTT-VOYAGE/Travelpayout) | TRTT Voyage travel partner discovery and outbound referral hub | Partner catalog, supplied affiliate URLs, disclosure, referral UI and its tests |

The Command Center is the hub; Learning Journey and Travelpayout are connected modules. Neither module becomes a mirror of the other.

## 2. Diamond King operating role

Diamond King is the designated AI collaborator across these repositories for planning, code/documentation assistance, source review, evidence capture and cross-project coordination. The same project code and collaboration identity are used in each repository. The human Owner retains ownership and approval authority.

Only curated, non-sensitive project artifacts belong in GitHub. Do not copy raw private conversations, credentials, personal contact data, or sensitive personal information between repositories.

## 3. Bridge contract

Every cross-repository reference should carry enough information to be auditable:

- `project_code`: `DR-TRTT-OPS-001`
- `system_id`: `command-center`, `learning-journey`, or `travelpayout`
- `record_type`: decision, learning, idea, partner-catalog, issue, release, or verification
- `record_id`: stable identifier within the source repository
- `title`: short human-readable label
- `owner`: accountable human or team
- `status`: proposed, in-progress, verified, blocked, or retired
- `source_repo`, `source_path`, and `source_commit`: exact origin
- `evidence_urls`: links to supporting source files, checks or PRs
- `updated_at`: ISO-8601 timestamp
- `visibility`: public, internal, or private (private content must not be copied to public repos)

A reference is not a data transfer. The source repository remains authoritative for its own records.

## 4. Data and workflow boundaries

1. **Command Center → modules:** publish decisions, project identifiers, safe standards and navigation references.
2. **Learning Journey → Command Center:** link curated learning records and product decisions by repository path/commit; do not ingest private chat transcripts.
3. **Travelpayout → Command Center:** report partner-catalog version, source-register reference, test result and release state. Keep affiliate URLs and catalog data in Travelpayout and the Command Center's preserved source register.
4. **Diamond King → all three:** use authorized repository tools, read before write, use feature branches, read back every changed file, and report exact test boundaries.
5. **No silent sync:** no webhook, scheduled cross-repo write, GitHub App, external database or automatic ChatGPT Memory synchronization is created by this bridge.

## 5. Current implementation mode

**Manual, version-controlled bridge.** Reciprocal repository links, a central machine-readable registry and a shared record contract make the relationship discoverable and auditable. They do not automatically copy files, trigger workflows or synchronize runtime data.

Future automation requires a separate design, least-privilege permissions, a free-tier review, failure handling, idempotency, audit logs and a tested recovery path.

## 6. Approval and security

- Feature branches and pull requests only; no direct default-branch edits.
- Owner review/merge required by repository rules.
- No production deployment, Pages activation, DNS/security/account permission change, live Blogger publication or Telegram delivery.
- No secrets in code, data files, logs or public issues.
- Travelpayout provider redirects, campaign attribution and commissions remain independently unverified until tested against provider evidence.

## 7. Verification checklist

- [x] Three repository identities and roles recorded.
- [x] Central registry and shared bridge contract prepared.
- [x] Reciprocal navigation links added in repository documentation and project entry pages.
- [x] Existing project data remains in its source repository.
- [ ] Owner-reviewed PRs merged.
- [ ] Browser/mobile/accessibility QA completed.
- [ ] Automated cross-repository synchronization designed and tested (not part of this bridge).
- [ ] Production deployment verified (not part of this bridge).

---
**Marker:** diamond-king-three-repository-bridge-001-20261128
