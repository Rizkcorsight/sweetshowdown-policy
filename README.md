Sweet Showdown — Privacy Policy
================================

Last updated: 2026-05-22

## Plain-language summary

Sweet Showdown collects nothing. Everything you make stays on your device.
We don't have servers, accounts, or user logins. We don't
talk to advertisers or analytics services. There is no in-app purchase.
The app never makes a network call — there's no internet code in the
binary at all.

## What's stored on your device

- **Game progress** (XP, completed Season chapters, daily streak,
  unlocked judges and trophies, sound/music/haptics preferences) —
  saved in local app-private storage on your device.
- **Saved dishes** — when you finish a round and the dish is added to
  your Gallery, a PNG image plus a recipe summary are saved to the
  app's private storage. They never leave your device unless YOU
  choose to share them via the system share sheet (Photos, AirDrop,
  Messages, Files, Mail, etc.).
- **In-progress rounds** — if you're pulled away mid-round, we save a
  small snapshot so you can resume on next launch. Stale snapshots
  (3+ days old) are auto-deleted.
- **Photo Library / media save (only when you choose it)** — if you
  save or share a finished dish, the operating system handles that
  destination. We never read existing photos.

## What's NOT collected

- No name. No email. No phone number. No location. No birthdate.
- No camera, microphone, or contacts access.
- No advertising identifiers.
- No analytics events.
- No crash reports sent to us. Apple or Google may receive store-level
  diagnostics under your device and account settings; that is handled
  by the operating system, not by Sweet Showdown.
- No third-party analytics, advertising, social, or tracking tools.

## Network usage

Sweet Showdown is fully offline by design. **The app makes zero
network calls of any kind** — no `URLSession`, no peer-to-peer
discovery, no Bonjour, no MultipeerConnectivity, no remote config.
The local party/head-to-head mode is pass-the-device only: players
alternate turns on the same device. (An earlier "Nearby"
peer-discovery prototype that briefly broadcast a display name over
local WiFi has been removed entirely from the v1 build.)

## Sound, motion, and Live Activities

- **Sound** — sound effects, music, and read-aloud voices are generated
  or played on-device. No microphone is used, and no audio data ever
  leaves the device.
- **Motion** — when motion is available, tiny device tilts can subtly
  affect how sprinkles roll. Motion data is read in-process and
  discarded immediately; nothing is logged, stored, or transmitted.
- **Live Activities** — the in-progress round timer can show on your
  Lock Screen / Dynamic Island via WidgetKit. The Live Activity reads
  round state in-process; no network or shared container.
- **Speech** — judge/read-aloud voices use the platform's on-device
  speech system. Speech generation never leaves the device.

## Platform privacy declarations

Sweet Showdown's platform privacy declarations cover the following
local-only system capabilities:

- `UserDefaults` — to save your progress and settings (CA92.1)
- `FileTimestamp` — to age-check saved snapshots (C617.1)
- `DiskSpace` — to verify there's room before saving a dish (E174.1)
- `SystemBootTime` — to compute relative timestamps (35F9.1)

The store privacy declarations also state **"Data Not Collected"**,
which matches the absence of app networking and data collection.

## Children and Family Sharing

Sweet Showdown is designed for younger children and families. We follow
the privacy expectations for children and family apps:

- No third-party analytics, advertising, social, or tracking tools.
- No external links exposed to the child without a parental gate.
- No identifying information collected from the child — no usernames,
  no profile pictures, no chat.
- No In-App Purchases. The app is paid up-front; once you own it you
  have everything.
- No push notifications.
- No multiplayer contact with strangers — Versus is one-device
  alternating turns only.

## Sharing a dish

If you tap the "Share" button on a finished-round sticker, poster,
cookbook, or Gallery item, the operating system opens its standard
share sheet so you can choose where it goes. The share sheet itself is
provided by the operating system — Sweet Showdown does not see what
destination you choose or whether you actually send it. Once you do send something, that destination's
privacy policy applies.

## Changes to this policy

If we ever change the policy, the "Last updated" date at the top will
change, and we'll mention material changes in store release notes.

## Contact

Email: Rizkcorsight@Rizkcorsight.com

<!-- policy-translations-start -->
## Localized Privacy Policies

The root URL remains the canonical English policy. Localized convenience translations are available at:

- Español: `https://rizkcorsight.github.io/sweetshowdown-policy/es/`
- Français: `https://rizkcorsight.github.io/sweetshowdown-policy/fr/`
- Deutsch: `https://rizkcorsight.github.io/sweetshowdown-policy/de/`
- Italiano: `https://rizkcorsight.github.io/sweetshowdown-policy/it/`
- 日本語: `https://rizkcorsight.github.io/sweetshowdown-policy/ja/`
- 한국어: `https://rizkcorsight.github.io/sweetshowdown-policy/ko/`
- Português (Brasil): `https://rizkcorsight.github.io/sweetshowdown-policy/pt-BR/`
- 简体中文: `https://rizkcorsight.github.io/sweetshowdown-policy/zh-Hans/`
- 繁體中文: `https://rizkcorsight.github.io/sweetshowdown-policy/zh-Hant/`
- العربية: `https://rizkcorsight.github.io/sweetshowdown-policy/ar/`
- עברית: `https://rizkcorsight.github.io/sweetshowdown-policy/he/`
- Nederlands: `https://rizkcorsight.github.io/sweetshowdown-policy/nl/`
- Русский: `https://rizkcorsight.github.io/sweetshowdown-policy/ru/`
<!-- policy-translations-end -->
