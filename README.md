# Shared community health files

This public repository supplies GitHub community health defaults for repositories owned by `ejryan89`.
It is also the canonical source for copies kept in individual repositories.

## Files

| File | Purpose |
| --- | --- |
| `.github/pull_request_template.md` | Prompts contributors to explain changes, implications, and validation. |
| `.github/ISSUE_TEMPLATE/bug.md` | Collects reproduction steps, expected behavior, actual behavior, and environment. |
| `.github/ISSUE_TEMPLATE/enhancement.md` | Collects the problem, proposed behavior, and acceptance criteria. |
| `.github/ISSUE_TEMPLATE/documentation.md` | Identifies documentation gaps and the desired correction. |
| `.github/ISSUE_TEMPLATE/question.md` | Collects usage questions and what the reporter tries. |
| `.github/ISSUE_TEMPLATE/config.yml` | Disables blank issues and records security reporting guidance in a comment. |
| `SECURITY.md` | Directs private vulnerability reports to the affected repository's Security tab. |
| `CODE_OF_CONDUCT.md` | Sets participation expectations and directs enforcement reports to the maintainer. |
| `labels.yml` | Defines the canonical shared labels and their descriptions and colors. |

Nothing applies `labels.yml` automatically. Repositories create or synchronize the shared labels explicitly
and add their own labels on top. Issue templates use the matching labels, so those labels need to exist
in the repository that receives the issue.

## How defaults apply

GitHub uses these files in its web UI when a repository owned by this account lacks its own copy.

If a repository has anything in `.github/ISSUE_TEMPLATE/`, including only `config.yml`, GitHub uses that
repository's issue template configuration and does not use the default issue templates.

`pull_request_template.md`, `SECURITY.md`, `CODE_OF_CONDUCT.md`, `CONTRIBUTING.md`, and `SUPPORT.md`
each fall back independently. A local copy of a file overrides only that file type. This repository supplies
the files listed above; it does not supply a contributing guide or support policy.

See [GitHub's default community health file documentation](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file).

## Copies for agent sessions

Defaults never appear in a clone. Agent sessions need real copies in the repositories where they work.
Keep those copies in each repository and review updates from this canonical source. Preserve repository
specific guidance where it is needed; these defaults provide a fallback and a shared starting point.

## Repository settings

Enable private vulnerability reporting in each public repository that uses the security policy.
The policy file does not enable the setting. Private repositories need a private contact channel through
their maintainer when GitHub's reporting option is unavailable.

See [GitHub's private vulnerability reporting configuration](https://docs.github.com/en/code-security/how-tos/report-and-fix-vulnerabilities/configure-vulnerability-reporting/configure-for-a-repository).

Maintainers provide a usable private reporting channel for Code of Conduct reports. The shared code names
the maintainer as the enforcement contact; it does not publish a contact address.
