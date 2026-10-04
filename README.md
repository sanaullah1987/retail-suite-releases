# Retail Suite — Releases

Public download & auto-update feed for **Retail Suite** — an offline-first
Point-of-Sale, Inventory & Accounting app for retailers.

> This repository holds only the built installers and update metadata.
> There is **no source code** here — releases are published automatically by CI
> whenever a new version is tagged.

## Download & install (Windows)

1. Open the **[latest release](../../releases/latest)**.
2. Download **`Retail-Suite-Setup-<version>.exe`**.
3. Run it. The app isn't code-signed yet, so Windows SmartScreen may warn on the
   first launch — click **More info → Run anyway**.

That's the only manual step. After this first install, the app keeps itself up to
date on its own.

## Automatic updates

On launch the app checks this repo and downloads any newer version in the
background using `latest.yml` — but it **never interrupts a sale**. An update only
installs when the till is idle or on the next restart. Offline shops keep trading
and simply update the next time they're online.

## What each release contains

| File | Purpose |
| --- | --- |
| `Retail-Suite-Setup-<version>.exe` | The Windows installer — use this for the first install |
| `latest.yml` | Update manifest the app reads to detect new versions |
| `Retail-Suite-Setup-<version>.exe.blockmap` | Enables small differential update downloads |

## Support

For help or to report a problem, contact your Retail Suite provider.

---

© Retail Suite. All rights reserved.
