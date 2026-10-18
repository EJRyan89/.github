# Shared community health files

This public repository supplies GitHub community health defaults for repositories owned by `EJRyan89`.
It is also the canonical source for copies kept in individual repositories.

## Files

| File | Purpose |
| --- | --- |
| `.github/pull_request_template.md` | Prompts contributors to explain changes, implications, and validation. |
| `.github/ISSUE_TEMPLATE/bug.md` | Collects reproduction steps, expected behavior, actual behavior, and environment. |
| `.github/ISSUE_TEMPLATE/enhancement.md` | Collects the problem, proposed behavior, and acceptance criteria. |
| `.github/ISSUE_TEMPLATE/documentation.md` | Identifies documentation gaps and the desired correction. |
| `.github/ISSUE_TEMPLATE/question.md` | Collects usage questions, relevant documentation, and troubleshooting results. |
| `.github/ISSUE_TEMPLATE/config.yml` | Disables blank issues and links to the shared security policy in the issue chooser. |
| `.github/FUNDING.yml` | Links the repository's Sponsor button to the maintainer's Ko-fi page. |
| `SECURITY.md` | Directs private vulnerability reports to the affected repository's Security tab. |
| `CODE_OF_CONDUCT.md` | Sets participation expectations and directs enforcement reports to the maintainer. |
| `labels.yml` | Defines the canonical shared labels and their descriptions and colors. |

Nothing applies `labels.yml` automatically. The shared label names, descriptions, and colors match GitHub's
default labels for new repositories. Existing labels need no synchronization unless their definitions differ.
Repositories restore missing labels explicitly and add their own labels on top. A template can apply its
matching label only when that label exists in the repository that receives the issue.

## How defaults apply

GitHub uses these files in its web UI when a repository owned by this account lacks its own copy.

If a repository has anything in `.github/ISSUE_TEMPLATE/`, including only `config.yml`, GitHub uses that
repository's issue template configuration and does not use the default issue templates.

`pull_request_template.md`, `SECURITY.md`, `CODE_OF_CONDUCT.md`, `CONTRIBUTING.md`, `SUPPORT.md`, and
`FUNDING.yml` each fall back independently. GitHub reads a default `FUNDING.yml` only from this repository's
`.github` folder. A local copy of a file overrides only that file type. This repository supplies
the files listed above; it does not supply a contributing guide or support policy.

See [GitHub's default community health file documentation](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file).

## Copies for agent sessions

Defaults never appear in a clone. Agent sessions need real copies in the repositories where they work.
Keep those copies in each repository. This canonical source provides the shared starting point;
local copies can diverge to include guidance specific to each repository. Updates are reviewed and copied
manually; nothing synchronizes them automatically.

## Repository settings

Enable Sponsorships under Settings, General, Features in each repository that should show the Sponsor
button. `FUNDING.yml` does not enable the setting, and a repository with it disabled shows no button.

See [GitHub's sponsor button documentation](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/displaying-a-sponsor-button-in-your-repository).

Enable private vulnerability reporting in each public repository that uses the security policy.
The policy file does not enable the setting. GitHub does not offer this reporting feature for private
repositories. A private repository, or a public repository with the feature disabled, needs a private
contact channel from its maintainer. Without one, the shared policy provides no private reporting route.

See [GitHub's private vulnerability reporting configuration](https://docs.github.com/en/code-security/how-tos/report-and-fix-vulnerabilities/configure-vulnerability-reporting/configure-for-a-repository).

The shared code of conduct names the repository maintainer as the enforcement contact; private reports to
the maintainer depend on a channel they publish. For abuse on GitHub, the code of conduct also provides a
fallback to GitHub Support. GitHub handles those reports under its own policies.
