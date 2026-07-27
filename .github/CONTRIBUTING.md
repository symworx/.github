# Contributing to SymWorx

Thanks for your interest in contributing. These guidelines apply to
[symworx/symworx](https://github.com/symworx/symworx) unless that repository
provides its own `CONTRIBUTING.md`.

> **Note:** The first public release is pending. The monorepo may still be
> private; contribution paths open fully when the repository is public.

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

1. Fork [symworx/symworx](https://github.com/symworx/symworx) (or use a branch if you have write access).
2. Base work on the default branch **`develop`** (not `main`).
3. Create a focused branch: `fix/short-description` or `feat/short-description`.
4. Prefer small, reviewable commits with clear messages.
5. Run the monorepo tests and linters before opening a PR (see its `README.md` / `DEVELOPMENT.md`).
6. Open a pull request against **`develop`**.

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

- Match the monorepo style and tooling (e.g. `rustfmt`, workspace lints).
- Prefer clear names and explicit error handling over cleverness.
- Do not commit secrets, large binaries, or generated artifacts unless the
  project already tracks them intentionally.

## License

Contributions are accepted under the Apache License 2.0 as used by the monorepo.
By submitting a contribution, you agree that it may be distributed under that
license.
