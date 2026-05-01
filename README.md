Sweet Showdown — Privacy Policy
================================

Last updated: 2026-05-01

## Plain-language summary

Sweet Showdown collects nothing. Everything you make stays on your iPad
or iPhone. We don't have servers, accounts, or user logins. We don't
talk to advertisers or analytics services. There is no in-app purchase.
The app never makes a network call — there's no internet code in the
binary at all.

## What's stored on your device

- **Game progress** (XP, completed Season chapters, daily streak,
  unlocked judges and trophies, sound/music/haptics preferences) —
  saved in your device's `UserDefaults`.
- **Saved dishes** — when you finish a round and the dish is added to
  your Gallery, a PNG image plus a recipe summary are saved to the
  app's Documents folder. They never leave your device unless YOU
  choose to share them via the iOS Share Sheet (Photos, AirDrop,
  Messages, etc.).
- **In-progress rounds** — if you're pulled away mid-round, we save a
  small snapshot so you can resume on next launch. Stale snapshots
  (3+ days old) are auto-deleted.
- **Photo Library (only on save-to-Photos)** — if you tap "Save to
  Photos" on a finished dish, iOS prompts you for permission and the
  PNG is added to your Photo Library. We never read existing photos.

## What's NOT collected

- No name. No email. No phone number. No location. No birthdate.
  (Earlier builds had a "player name" field — it's been removed in v1.)
- No camera, microphone, or contacts access.
- No advertising identifiers (IDFA, IDFV).
- No analytics events.
- No crash reports sent to us. (iOS may send anonymized crash data to
  Apple if your device's Diagnostics setting opts in — that's between
  you and Apple.)
- No third-party SDKs at all — every framework imported is a
  first-party Apple framework (SwiftUI, RealityKit, AVFoundation,
  CoreMotion, WidgetKit).

## Network usage

Sweet Showdown is fully offline by design. **The app makes zero
network calls of any kind** — no `URLSession`, no peer-to-peer
discovery, no Bonjour, no MultipeerConnectivity, no remote config.
The Versus head-to-head mode is pass-the-iPad only: two players
alternate turns on the same device. (An earlier "Nearby"
peer-discovery prototype that briefly broadcast a display name over
local WiFi has been removed entirely from the v1 build.)

## Sound, motion, and Live Activities

- **Sound** — every sound effect and the background music are
  *generated procedurally on-device* via `AVAudioEngine`; no audio
  files ship with the app. The audio session uses `.playback` with
  `.mixWithOthers`, so if you have Spotify or Apple Music playing,
  Sweet Showdown's music plays at the same time without ducking your
  other audio. The app also listens for system audio interruptions
  (phone calls, alarms) and resumes its own audio when iOS clears the
  interruption — no audio data ever leaves the device.
- **Motion** — when you place toppings, tiny iPad tilts subtly affect
  how sprinkles roll using `CMMotionManager`. Motion data is read
  in-process and discarded immediately; nothing is logged, stored, or
  transmitted. This is why the app declares
  `NSMotionUsageDescription` in `Info.plist`.
- **Live Activities** — the in-progress round timer can show on your
  Lock Screen / Dynamic Island via WidgetKit. The Live Activity reads
  round state in-process; no network or shared container.
- **Speech** — judge voices use Apple's on-device
  `AVSpeechSynthesizer`. Speech generation never leaves the device.

## Required-reason API declarations

Per Apple's Privacy Manifest (`PrivacyInfo.xcprivacy` in the bundle),
Sweet Showdown declares the following required-reason APIs:

- `UserDefaults` — to save your progress and settings (CA92.1)
- `FileTimestamp` — to age-check saved snapshots (C617.1)
- `DiskSpace` — to verify there's room before saving a dish (E174.1)
- `SystemBootTime` — to compute relative timestamps (35F9.1)

The Privacy Manifest also explicitly declares **"Data Not Collected"**,
which is enforced by the absence of any networking code in the binary.

## Children and Family Sharing

Sweet Showdown ships in the App Store Kids Category with the
**Ages 5 and Under** age band. We follow Apple's guidelines for apps
targeting children:

- No third-party analytics, advertising, or social SDKs.
- No external links exposed to the child without a parental gate.
- No identifying information collected from the child — no usernames,
  no profile pictures, no chat.
- No In-App Purchases. The app is paid up-front; once you own it you
  have everything.
- No push notifications.
- No multiplayer contact with strangers — Versus is one-device
  alternating turns only.

## Sharing a dish

If you tap the "Share" button on a finished-round sticker or in the
Gallery, iOS opens its standard Share Sheet so you can send the PNG
via Messages, Mail, AirDrop, Notes, Photos, or any third-party share
extension you have installed. The Share Sheet itself is iOS — Sweet
Showdown does not see what destination you choose or whether you
actually send it. Once you do send something, that destination's
privacy policy applies.

## Changes to this policy

If we ever change the policy, the "Last updated" date at the top will
change, and we'll mention the change in the App Store release notes.

## Contact

Email: support@sweetshowdown.app
