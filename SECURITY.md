# Security Policy

## Report privately
Do not post exploit details, credentials, personal data, or proof-of-concept payloads in public issues or pull requests. Open the repository Security tab and use private vulnerability reporting if available. If unavailable, contact the Owner through an established private channel and first confirm a secure reporting route. Do not send vulnerability details until that route is confirmed.

Include the affected repository/path/commit, realistic impact, minimal safe reproduction steps, and a suggested mitigation. Coordinated disclosure is preferred. Response times and remediation timelines are not guaranteed.

## Secret exposure
Never copy credentials into issues, PRs, chats, logs, or documentation. If exposed, notify the Owner privately and rotate or revoke the credential at its provider immediately. Removing a secret from Git history does not invalidate it.

## Scope
This policy grants no permission to access private data, bypass authentication, disrupt services, perform social engineering, conduct denial-of-service tests, or assess third-party systems. Only test systems you own or are explicitly authorized to assess.

## Platform boundary
This document describes reporting expectations; it does not prove that GitHub private vulnerability reporting, secret scanning, push protection, Dependabot alerts, branch protection, or any other account-level setting is enabled.
