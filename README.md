Sweet Showdown — Privacy Policy
================================

Last updated: 2026-04-29

## Plain-language summary

Sweet Showdown collects nothing. Everything you make stays on your iPad
or iPhone. We don't have servers, accounts, or user logins. We don't
talk to advertisers or analytics services. There is no in-app purchase.

## What's stored on your device

- **Game progress** (XP, completed Season chapters, daily streak,
  unlocked judges and trophies) — saved in your device's UserDefaults.
- **Saved dishes** — when you finish a round and the dish is added to
  your Gallery, an image and a recipe summary are saved to your app's
  Documents folder. They never leave your device unless YOU choose to
  share them via the iOS Share Sheet (Photos, AirDrop, Messages, etc.).
- **In-progress rounds** — if you're pulled away mid-round, we save a
  small snapshot so you can resume on next launch. Stale snapshots
  (3+ days old) are auto-deleted.

## What's NOT collected

- No name. No email. No phone number. No location. No birthdate.
- No camera, microphone, or contacts access.
- No advertising identifiers (IDFA, IDFV).
- No analytics events.
- No crash reports sent to us. (iOS may send anonymized crash data to
  Apple if your device's Diagnostics setting opts in — that's between
  you and Apple.)

## Network usage

Sweet Showdown is fully offline by design. The only network activity is
Apple's local-only "Nearby" peer-to-peer Wi-Fi/Bluetooth discovery, used
for the head-to-head Versus mode. **In v1, this feature is disabled.**
No data ever leaves your local network in any release.

## Required-reason API declarations

Per Apple's Privacy Manifest, Sweet Showdown declares the following
required-reason APIs:

- `UserDefaults` — to save your progress and settings (CA92.1)
- `FileTimestamp` — to age-check saved snapshots (C617.1)
- `DiskSpace` — to verify there's room before saving a dish (E174.1)
- `SystemBootTime` — to compute relative timestamps (35F9.1)

## Children and Family Sharing

Sweet Showdown is in the Kids Category. We follow Apple's guidelines for
apps targeting children, including:
- No third-party analytics or advertising SDKs.
- No external links exposed to the child without a parental gate.
- No identifying information collected from the child.

## Changes to this policy

If we ever change the policy, the "Last updated" date at the top will
change, and we'll mention the change in the App Store release notes.

## Contact

Email: support@sweetshowdown.app
