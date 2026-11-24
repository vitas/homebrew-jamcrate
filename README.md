# JamCrate — Homebrew tap

[![Install](https://img.shields.io/badge/brew%20install%20--cask-vitas%2Fjamcrate%2Fjamcrate-black)](https://github.com/vitas/homebrew-jamcrate)

Backing-track player for musicians: solo markers, loop points, tempo and pitch
control, CoreMIDI footswitch support. Native macOS app, Apple silicon and Intel.
Free, no account.

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

Requires macOS 14 Sonoma or later. The app is signed and notarized by Apple, so it
opens with a plain double-click — no "Open Anyway" step.

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
valid and passes `brew audit --cask --online`. The official repository has
requirements this project only partly meets:

| Requirement | Status |
|---|---|
| Passes Gatekeeper (notarized) | done |
| Repository at least 30 days old | done |
| 225 stars, or 90 forks, or 90 watchers (self-submission) | not yet |

Until then, this tap is the supported install path. The cask is generated from
the release artifact by `tools/make-cask.sh` in the main project — the `sha256`
is always computed from the published DMG, never typed by hand.
