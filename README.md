# JamCrate — Homebrew tap

[![Install](https://img.shields.io/badge/brew%20install%20--cask-vitas%2Fjamcrate%2Fjamcrate-black)](https://github.com/vitas/homebrew-jamcrate)

Backing-track player for musicians: solo markers, loop points, tempo and pitch
control, CoreMIDI footswitch support. Native macOS app, Apple silicon and Intel.

Site: <https://jamcrate.app> · Try it in the browser, no install:
<https://play.jamcrate.app>

## Install

```sh
brew tap vitas/jamcrate
brew install --cask jamcrate
```

Or in one line, without tapping first:

```sh
brew install --cask vitas/jamcrate/jamcrate
```

Requires macOS 14 Sonoma or later.

## ⚠️ First launch

**This beta is ad-hoc signed, not notarized yet**, so macOS will block it the
first time you open it. That is expected, and `brew install` prints the same
notice. To get past it once:

- **macOS 15 Sequoia and later:** try to open the app, then go to
  **System Settings → Privacy & Security**, scroll down and click **Open Anyway**.
- **macOS 14 Sonoma:** right-click `JamCrate.app` in Applications and choose
  **Open**, then confirm.

You only do this once. Notarized builds — once the Apple Developer enrollment
completes — will open with a plain double-click, and this notice will disappear
from the cask.

## Upgrade

```sh
brew upgrade --cask jamcrate
```

## Uninstall

```sh
brew uninstall --cask jamcrate
```

Your sets, markers and settings are not touched by uninstalling.

## About this tap

This is a personal tap, which means the cask lives here rather than in
[homebrew/cask](https://github.com/Homebrew/homebrew-cask). The cask itself is
valid and passes `brew audit --cask --online`; the official repository has two
additional requirements this project does not meet yet:

| Requirement | Status |
|---|---|
| Passes Gatekeeper (notarized) | pending Apple Developer enrollment |
| Repository at least 30 days old | not yet |
| 225 stars, or 90 forks, or 90 watchers (self-submission) | not yet |

Until then, this tap is the supported install path. The cask is generated from
the release artifact by `tools/make-cask.sh` in the main project — the `sha256`
is always computed from the published DMG, never typed by hand.
