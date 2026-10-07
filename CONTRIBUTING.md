# Contributing

Thanks for your interest in improving the decomposition-note bundle.

## Before you start

- For anything beyond a small fix, open an issue first so the change can be
  discussed before you invest time in it.
- Security problems go through `SECURITY.md`, not public issues.

## Requirements

- Python 3.11 or newer (the CLI uses standard-library `tomllib`)
- Bash

## Making a change

1. Fork the repository and branch from `main`. Branch names are snake_case
   with one of these prefixes: `fix/`, `feature/`, `chore/`, `docs/`
   (for example `fix/lease_expiry_check`).
2. Keep each pull request to one concern. Refactoring goes in a separate
   commit from behavior changes.
3. Run the validator and make sure it passes:

   ```bash
   ./validate-bundle.sh
   ```

4. If you change bundled files, update `MANIFEST.sha256` and, where relevant,
   `VERSION` and `README.md`.
5. Open a pull request against `main` describing what changed and why.

## Commit messages

Use a conventional prefix matching the branch type, for example
`fix: reject expired lease at JOIN` or `docs: clarify install steps`.

## License

By contributing, you agree that your contributions are licensed under the
Apache License 2.0, as described in `LICENSE`.
