# Contributing to Kowari

**Kowari is in v0 (pre-alpha).** The design is being finalized and the
compiler is under construction. We are not yet accepting external code
contributions, because the API surface is changing week-to-week and
reviewing PRs against a moving target is unkind to contributors.

## When contributions open

External contributions will open at **Milestone 2** (see `PLANNING.md`
in the monorepo). The first opportunities will be:

- Adding golden tests for diagnostic codes that lack them.
- Extending the standard library once its API is stable.
- Editor integrations and tooling (v2).

## How to follow along

- Read [`SPEC.md`](https://github.com/kowari-lang/kowari/blob/main/SPEC.md)
  and [`PLANNING.md`](https://github.com/kowari-lang/kowari/blob/main/PLANNING.md).
- Watch the monorepo for releases.
- Open a **discussion** (not an issue) if you have a design question.

## Design proposals

Language-design changes are made by editing `SPEC.md` in the monorepo,
with a rationale and the corresponding test changes. Do not open a PR
that changes `SPEC.md` without first opening an issue to discuss it —
the spec is the contract, and changes to it ripple through everything.

## Code of conduct

All participation in Kowari spaces (issues, discussions, PRs, chat) is
governed by the [Code of Conduct](./CODE_OF_CONDUCT.md).

## Security

Do not open a public issue for security problems. See [SECURITY.md](./SECURITY.md).