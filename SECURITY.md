# Security

Security issues should be handled carefully and should not be disclosed publicly before they have been reviewed.

## Secrets and credentials

Never commit secrets or credentials to a repository.

This includes:

* API keys and access tokens
* passwords
* private keys and certificates
* cloud credentials
* service-account credentials
* `.env` files containing secrets
* database credentials
* other authentication material

Use the appropriate secret-management mechanism for development, CI, and deployment instead.

If a secret is accidentally committed, treat it as compromised even if the commit is subsequently removed. Revoke or rotate the credential immediately and notify the appropriate repository or organization owner.

Do not rely solely on deleting the secret from Git history.

## Reporting security issues

Do not open a public GitHub issue for a suspected security vulnerability or exposed credential.

Instead, report the issue privately to an organization owner or the appropriate repository maintainer.

Include, where possible:

* a description of the issue;
* the affected repository or component;
* steps to reproduce or verify it;
* the potential impact;
* any known mitigation.

## Dependencies

New third-party dependencies should come from trusted sources and have licenses compatible with their intended use.

Avoid adding unnecessary dependencies.

Security updates to dependencies should be reviewed and applied promptly when they affect company software.

## Access

Repository and organization access should be limited to what is necessary for a person's work.

Do not share GitHub accounts, credentials, personal access tokens, SSH private keys, or other authentication material.

Access should be removed when it is no longer required.

## Security-sensitive changes

Changes involving authentication, authorization, secrets, infrastructure, deployment, or other security-sensitive functionality should receive careful review before being merged.
