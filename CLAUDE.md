# CLAUDE.md — surfn-mint-y-pink

## Project overview

Standalone repo for the **Surfn-Mint-Y-Pink** icon theme, a colour variant of the base
`erikdubois/surfn` icon set. Folder-colour icons sourced from `linuxmint/mint-y-icons`.
See [README.md](./README.md).

## Current state

Ships one theme: `usr/share/icons/Surfn-Mint-Y-Pink/`. Packaged as `surfn-mint-y-pink-icons-git`
(recipe in `~/KIRO-PKG-BUILD-ICONS/surfn-mint-y-pink/`), `depends=('surfn-icons-git')` — the base Surfn theme.

## Patterns & decisions

- Theme dir PascalCase; repo/package lowercase. `icon-theme.cache` gitignored (rebuilt by
  the pacman hook on install). Only the sparse `places/` folder-colour icons are shipped;
  everything else inherits Surfn. Bash scripts follow the canonical Kiro template.
