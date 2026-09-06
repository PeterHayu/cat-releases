# cat-desktop — downloads

A desktop pet: a real cat — **bb** (short-haired tuxedo) or **niuniu** (blue-point longhair
Munchkin) — floats on top of your windows, transparent and frameless, and turns her head to
follow your mouse.

This repository holds **only the installers**. The source lives in a private repo.

## Install

Grab the newest build from [Releases](https://github.com/PeterHayu/cat-releases/releases/latest).

- **Windows** — `cat-desktop_<version>_x64-setup.exe`. The build is not Authenticode-signed, so
  SmartScreen warns on first run: *More info → Run anyway*.
- **macOS** — `cat-desktop_<version>_aarch64.dmg` (Apple silicon). Unsigned, so the first launch
  needs right-click → *Open*.

## Updating

From **v0.2.4** onward the cat updates herself: right-click her → **Check for Updates**. The menu
item's own label reports progress, and she relaunches into the new version.

Builds up to and including **v0.2.3** cannot do this — they look for updates in a private location
and always report "Update failed". Replace one of those by installing from Releases once; after
that it is automatic.

The `latest.json` attached to each release is the manifest the app polls. Every installer ships
with a `.sig` next to it, and the app refuses any update whose signature does not verify.
