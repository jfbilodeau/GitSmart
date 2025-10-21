# Security Policy

Thank you for taking the time to responsibly disclose security issues in GitSmart. This project is a demo application; the guidance below describes how to report potential vulnerabilities and what to expect.

## Supported Versions

This repository is a demo and does not have an official supported version lifecycle. If you rely on this code for anything sensitive, please treat it as experimental and do not deploy it without appropriate security reviews.

## Reporting a Vulnerability

Please do NOT open a public issue for security vulnerabilities. Instead, report them privately to the repository owner. Recommended options:

- Send an email to the repository owner (if available) with the subject `Security issue in GitSmart` and include details, reproduction steps, and any PoC code.
- If you have the OWNER's GitHub username, you can send them a direct message on GitHub or use GitHub's security advisories if you have permissions to do so.

If you don't have a private contact, and the vulnerability is time-sensitive, you may contact the project maintainer(s) through your normal channels and mark the communication confidential.

## What to include in your report

- A clear description of the issue and impact.
- Detailed steps to reproduce, including code snippets or PoC if possible.
- The environment where it occurs (OS, .NET SDK/runtime version, configuration).
- Any suggested mitigations or patches, if applicable.

## Response process

1. A maintainer should acknowledge receipt within 3 business days.
2. The maintainer will ask follow-up questions if more information is needed.
3. The maintainer and reporter will agree on a disclosure timeline (private fix and coordinated disclosure is preferred).

## Handling security advisories

When a fix is ready, the maintainer will:

- Create a pull request with the fix and tests if feasible.
- Coordinate a disclosure timeline with the reporter.
- Publish a security advisory if the fix is a vulnerability in the public repo and affects users.

## Notes

- This project is a small demo and may not follow all industry-grade security practices. Use caution before using it in production.
- Do not send secrets or private keys in a public issue or PR.
