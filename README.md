# .github

This repository is the provisioning profile for the Duncanite organization on GitHub.

It contains:

- `profile/README.md`: the organization profile page shown on https://github.com/duncanite
- `.github/ISSUE_TEMPLATE/`: shared issue templates (bug, feature request, question) and their config
- `.github/PULL_REQUEST_TEMPLATE.md`: the default pull request body
- community health files applied org-wide:
  - `CODE_OF_CONDUCT.md`: acceptable behavior
  - `CONTRIBUTING.md`: tooling, rules, etc
  - `GOVERNANCE.md`: how the org is governed
  - `SECURITY.md`: vulnerability reporting process
  - `SUPPORT.md`: defining support
- `.lint-github.yaml`: the organization's declarations for `limen github check -org duncanite`

These defaults apply to every repository in the organization that does not provide its own.
GitHub only resolves them from a **public** `.github` repository, and only from the root,
`.github/` or `docs/`.

## Working on it

This repository is [`limen`](https://github.com/farcloser/limen)-enrolled, so the interface is
the usual one:

```
just lint
just security
just fix
```

### If you ever list a private repository

`profile/README.md` currently lists only public repositories, so there is no root
`.lint-links.toml`. If a private one is ever added, mark it 🔒 in the profile *and* exclude it
in a new root `.lint-links.toml`: lychee runs unauthenticated, so the link would otherwise 404
and fail the run.
