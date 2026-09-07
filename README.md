# Di-kairos/homebrew-tap

Homebrew tap for [Paranoid Tools](https://github.com/Di-kairos/paranoid-tools) — five small
macOS command-line tools for handling local secrets.

## Install

```bash
brew install Di-kairos/tap/securetrash
```

That is shorthand for:

```bash
brew tap Di-kairos/tap
brew install securetrash
```

Any of the five names works in place of `securetrash`.

## Formulae

- **securetrash** — honest secure file deletion for macOS (FileVault + crypto-shred vaults).
- **vaultwatch** — guard an open securetrash vault (Spotlight/Time Machine/cloud, TTL).
- **panic** — one-step hide-and-lock kill-switch.
- **ghostdraft** — ephemeral scratch draft kept in a RAM disk, not in on-disk temp.
- **seedsplit** — split a secret into Shamir shares (pure Bash, GF(256)).

## Verifying what you install

Homebrew installs from a source tarball of a signed release tag. The releases themselves carry an
Ed25519 signature over their checksum manifest; the repository's `verify-releases.sh` checks every
published release against the pinned key. The tarball route is convenient, not a substitute for
that check — the signed installers are documented in each tool's README.
