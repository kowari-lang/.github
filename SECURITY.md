# Security Policy

## Supported versions

Kowari is **v0 (pre-alpha)** and has no supported releases yet. There is
nothing to report against.

## Reporting a vulnerability

Once v1.0 ships, security reports will be handled via GitHub's private
vulnerability reporting at
<https://github.com/kowari-lang/kowari/security/advisories/new>.

Do **not** open a public issue for a suspected vulnerability.

## Scope

Kowari's threat model focuses on:

- Correctness of the compiler's safety invariants (affine check, reference rules, `unsafe` boundaries) — a compiler that accepts a program violating the invariants in `SPEC.md` §4.5 is a security bug.
- The WebAssembly host (`kowari-wasm-host`) — sandbox escape, memory corruption in marshalling.
- The FFI layer (`extern "C"`) — anything that lets safe Kowari code trigger UB through a foreign call.

Reports about the design itself (e.g. "the affine check should be
stronger") belong in a discussion, not a security report.