# Security policy

## Supported versions

Consult the repository's releases and documentation for supported versions. Check whether the issue affects
the latest supported version before reporting it.

## Reporting a vulnerability

Use the affected repository's **Security** tab → **Report a vulnerability** to report a suspected vulnerability
privately. Do not open a public issue.

GitHub's private vulnerability reporting is available only for public repositories where the maintainer
enables it. If that option is unavailable, contact the repository maintainer privately through a channel
they make available. This shared policy does not specify an alternative private contact method. If the
repository provides no private channel, there is no documented private reporting route. Do not disclose
vulnerability details publicly.

Include enough information to reproduce and assess the issue:

- the affected release or commit;
- relevant operating-system and tool versions;
- minimal reproduction steps;
- expected and observed behavior;
- potential impact and required preconditions; and
- any suggested mitigation.

Avoid credentials, tokens, personal configuration, private repository contents, and other sensitive data.
Use sanitized fixtures whenever possible.

The maintainer assesses the report, coordinates fixes and disclosure, and credits reporters who want
attribution. No response or remediation deadline is guaranteed.

## Security-sensitive areas

Report privately anything involving unauthorized access, command injection, unsafe file access, data loss,
trust-boundary failures, or disclosure of secrets through logs, generated files, archives, or diagnostics.

Non-sensitive defects and feature requests go through normal GitHub issues.
