# Security Policy

## Supported versions

Only the latest released bundle version (see `VERSION`) receives security fixes.

## Scope

This bundle installs Codex project configuration, hooks, rules, and Python
scripts that run inside the repositories that adopt it. Reports are in scope
when they concern, for example:

- a hook or guard that can be bypassed, or that fails open;
- `install.sh` writing outside the target repository or overwriting files it
  should not;
- runtime, audit, or evidence records leaking secrets or local material;
- integrity checks (JOIN verdicts, leases, `VOID + KEEP` rejection) that can be
  forged or skipped.

Behavior of the Codex runtime or model backends themselves is out of scope;
report those to their vendors.

## Reporting a vulnerability

Do not open a public issue. Report privately through either channel:

- GitHub: Security tab of this repository, "Report a vulnerability";
- email: eduard@agntflow.io

Include the bundle version, a description of the impact, and steps or a
minimal repository to reproduce it.

You can expect an acknowledgement within 5 business days. We will keep you
informed while a fix is prepared and credit you in the release notes unless
you ask us not to.
