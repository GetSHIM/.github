# Security policy

These are the organization defaults. A repository with its own `SECURITY.md`
overrides this file.

## Reporting a vulnerability

Report through a private GitHub Security Advisory on the affected repository:
open its **Security** tab and choose **Report a vulnerability**. If that is not
available to you, write to <security@getshim.tech>.

Do not open a public issue and do not include exploit details in one.

Please include:

- the affected repository and version
- the environment (OS, runtime version, client and version)
- reproduction steps
- what an attacker gets out of it
- relevant logs, with secrets and personal data removed

Please do not send real secrets or real personal data. Synthetic values
reproduce almost everything, and we would rather not hold your data while we
work on a fix.

## What happens next

We acknowledge the report, assess it, and coordinate disclosure through the
advisory. If we decide something is out of scope, we say so and explain why
rather than letting the thread go quiet.

## Supported versions

Only the latest released version of a package receives security fixes unless
its repository states otherwise.

## Scope

Our published tools are best-effort guards, not enforcement boundaries, and
they say so in their own documentation. A report is in scope when it shows a
behaviour worse than the documented one: prompt data leaving a path we
documented as local, unsafe hook output, persistence beyond a documented
temporary file, an unexpected network call, installer ownership failures, or a
fail-open path we did not document.
