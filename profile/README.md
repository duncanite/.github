# Duncanite

Common house projects: photo albums, mini event websites, home automation tooling, and the
small utilities that keep the Duncanites rolling.

One household's home lab, published. Everything here is built the same way as the
[farcloser](https://github.com/farcloser) tooling it runs on: pinned, linted and released by
the rules written down in the
[engineering book](https://github.com/farcloser/limen/blob/main/book/index.md).

## Container images

- [**cupsicle**](https://github.com/duncanite/cupsicle) — a container image for
  [CUPS](https://www.cups.org/), geared towards exposing legacy USB printers: read-only,
  no capabilities, a non-root process.
- [**jazzsamba**](https://github.com/duncanite/jazzsamba) — a container image for
  [Samba](https://www.samba.org/), geared towards Time Machine backups.

## Infrastructure

- **infra** — the infrastructure behind the house projects, as code; a private
  repository.
- [**.github**](https://github.com/duncanite/.github) — this repository: the organization
  profile and the community health files every other repository inherits.

## Contributing & support

Projects here are provided as-is, best-effort, without warranty.

- [Contributing guide](https://github.com/duncanite/.github/blob/main/.github/CONTRIBUTING.md)
- [Security policy](https://github.com/duncanite/.github/blob/main/.github/SECURITY.md)
- Bugs and ideas go to the issue tracker of the repository they concern.

The sibling organizations [farcloser](https://github.com/farcloser) and
[forkcloser](https://github.com/forkcloser) hold the tooling and the forks these are built with.
