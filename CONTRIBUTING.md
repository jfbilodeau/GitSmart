# Contributing to GitSmart

Thank you for your interest in contributing to GitSmart! This document outlines a simple, standard process for reporting issues, proposing changes, and submitting pull requests so we can keep this demo project useful and easy to maintain.

## Code of Conduct

Please follow common sense and kindness when interacting in issues and pull requests. If you want a formal Code of Conduct, add `CODE_OF_CONDUCT.md` to the repository; otherwise use the Contributor Covenant as a reference.

## How can I contribute?

You can contribute in several ways:

- Open an issue to report bugs or request a feature.
- Open a pull request to fix bugs, improve docs, or add features.
- Improve tests or add new tests.
- Improve documentation (README, docs, examples).

## Reporting bugs

- Search existing issues to see if the bug has already been reported.
- When opening a new issue, include:
  - A descriptive title.
  - Steps to reproduce the problem.
  - Expected behavior and actual behavior.
  - Environment details (OS, .NET SDK version, any relevant logs or stack traces).

## Suggesting enhancements

- For feature requests, include a clear description of the desired behavior and why it's useful.
- Provide examples or sketches if helpful.

## Pull request process

1. Fork the repository and create a branch for your change: `git checkout -b feature/my-change`.
2. If you're changing code, run and add tests when appropriate.
3. Keep commits small and focused; write clear commit messages.
4. Push your branch to your fork and open a PR to `main` with a descriptive title and description.
5. The maintainer(s) will review and may request changes. Address feedback, squash or clean up commits if requested, and update the PR.

## Code style

- Prefer idiomatic C# and follow the common .NET naming conventions.
- Keep the code simple and well-documented.
- If there are formatting preferences, add an `.editorconfig` or explain them here.

## Tests

- Add unit or integration tests for any functional change where feasible.
- Run tests locally before opening a PR: `dotnet test`.

## Local development

- Requirements: .NET 9 SDK.
- To build the project locally:

```powershell
dotnet restore
dotnet build
```

- To run the app locally:

```powershell
dotnet run --project .
```

## Security issues

If you discover a security vulnerability, please do not open a public issue. Instead, contact the repository owner directly or use your organization's responsible disclosure process.

---

Thanks again for helping improve GitSmart. Contributions are welcome — big or small.
