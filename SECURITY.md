# Security Policy

## Security Model

This repository is a public, publication-only knowledge base.

It is intentionally isolated from the maintainer's private
Obsidian vault, private research material, credentials, and
local authoring environment.

All external contributions are treated as untrusted input until
they have been reviewed and explicitly accepted.

## Reporting a Security Issue

Do not disclose sensitive security issues in public Issues,
Discussions, Pull Requests, or commit messages.

Potential security issues include:

- exposed credentials or authentication tokens
- accidentally published private or confidential information
- malicious or suspicious contributed files
- attempts to introduce executable content
- unauthorized modifications to repository governance files
- suspicious links or embedded content
- repository configuration weaknesses
- suspected account or repository compromise

If you discover a security issue, report it privately to the
repository maintainer.

## Secrets and Credentials

This repository must never contain:

- passwords
- API keys
- access tokens
- session credentials
- private keys
- certificates
- `.env` files
- authentication material

If a secret is accidentally published, it must be considered
compromised and revoked or rotated immediately.

Deleting the secret in a later commit is not considered sufficient,
because it may remain accessible through Git history, forks, clones,
or caches.

## Prohibited Content

Normal contributions must not introduce:

- executable code
- scripts
- Obsidian plugins
- Obsidian configuration
- GitHub Actions workflows
- environment files
- credentials
- private datasets
- confidential research material

See `CONTRIBUTING.md` for the complete contribution policy.

## Trust Boundary

The public repository must contain only information that is safe
for unrestricted public disclosure.

The public repository has no trusted synchronization path into the
maintainer's private authoring environment.

Content from external contributors is not automatically imported
into any private system.

## Supported Version

Only the current `main` branch is considered the authoritative
public version of this knowledge base.
