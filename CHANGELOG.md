# Changelog

## 0.2.0 — 2026-09-16

First public release of this austrasien fork of
[HeitorM50/omapkdex](https://github.com/HeitorM50/omapkdex).

### Added

- Count **Cursor** usage (Cursor IDE and `cursor-agent` CLI on the same
  account) from `~/.local/state/omarchy/agents/usage/cursor.json`.
- That file is the `schemaVersion: 1` record written by
  [omarchy-cursor-usage](https://github.com/austrasien/omarchy-cursor-usage),
  not by Omarchy's first-party collectors.

Claude Code, Codex and Fireworks are unchanged. Existing lifetime totals
still only set the ruler on first sight of an agent, so a Cursor history
does not graduate the first creature instantly.

### Install

```bash
omarchy plugin add https://github.com/austrasien/omarchy-omapkdex.git --enable
```

Already on upstream?

```bash
cd ~/.config/omarchy/plugins/io.github.heitorm50.omapkdex
git remote set-url origin https://github.com/austrasien/omarchy-omapkdex.git
git pull
omarchy restart shell
```
