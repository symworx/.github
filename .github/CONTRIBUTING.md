# Contributing to SymWorx

Thanks for your interest in contributing. These are org-wide defaults.
Use a repository’s own `CONTRIBUTING.md` when it has one.

Software in this org includes the [analysis monorepo](https://github.com/symworx/symworx)
plus sibling tools ([symkit](https://github.com/symworx/symkit),
[symelib](https://github.com/symworx/symelib),
[symsight](https://github.com/symworx/symsight),
[symcourse](https://github.com/symworx/symcourse),
[symjump](https://github.com/symworx/symjump)).
The monorepo’s first public release is in beta. 

## Ways to contribute

- Report bugs and request features with the issue templates
- Improve documentation and examples
- Submit pull requests for fixes and small, well-scoped features
- Review open PRs and discuss design in issues

## Before you start

1. Search existing issues and PRs to avoid duplicates.
2. For larger changes, open an issue first so maintainers can align on design.
3. Follow the [Code of Conduct](CODE_OF_CONDUCT.md).

## Development workflow

1. Fork the repository you are changing (or use a branch if you have write access).
2. Base work on that repo’s default branch — **`develop`** for the tools listed above (not `main`).
3. Create a focused branch: `fix/short-description` or `feat/short-description`.
4. Prefer small, reviewable commits with clear messages.
5. Run that repository’s tests and linters before opening a PR (see its `README.md` / `DEVELOPMENT.md`).
6. Open a pull request against **`develop`** (or `main` only if that repo’s default is `main`).

## Pull requests

- Describe **what** changed and **why**.
- Link related issues (`Fixes #123` when applicable).
- Keep the diff focused; avoid unrelated reformatting.
- Update docs or examples when behavior changes.
- Expect review feedback; maintainers may request changes before merge.

## Issues

Use the provided templates when available:

- **Bug report** — steps to reproduce, expected vs actual behavior, environment
- **Feature request** — problem statement, proposed approach, alternatives

Security vulnerabilities must **not** be filed as public issues. See
[SECURITY.md](SECURITY.md).

## Code style

- Match that repository’s style and tooling (e.g. `rustfmt`, workspace lints).
- Prefer clear names and explicit error handling over cleverness.
- Do not commit secrets, large binaries, or generated artifacts unless the
  project already tracks them intentionally.

## License

Public SymWorx repositories use the Apache License 2.0. By submitting a
contribution, you agree that it may be distributed under that license
(or the license stated in the target repository).
