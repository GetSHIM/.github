# Contributing

These are the organization defaults. A repository with its own
`CONTRIBUTING.md` overrides this file — read that one first.

## Before you open a pull request

- Keep the change small and self-contained. One reason per pull request.
- Run whatever the repository's CI runs, locally, before you push.
- Update the docs and tests that your change makes wrong.
- Use synthetic values everywhere. Never commit a real prompt, secret, key,
  customer name, or personal record — not in code, not in a test fixture, not
  in an issue, not in a screenshot.

## What we look for in review

Evidence. A benchmark number, a failing test that now passes, a link to the
spec you are following. "This should be faster" is not a claim we can merge.

## Behaviour that needs a design first

Network calls, telemetry, persistent state, self-updaters, and new client
adapters change the trust boundary of the software. Open an issue and get
agreement before writing that code, so nobody wastes an afternoon.

## Security

Do not report vulnerabilities in a pull request or a public issue. See
[SECURITY.md](SECURITY.md).
