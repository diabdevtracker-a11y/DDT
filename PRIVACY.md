# Privacy Policy — DiabetesDevicesTracker

**Effective date: April 2026**

DiabetesDevicesTracker ("the app") is a personal logging tool for
tracking infusion set changes and CGM sensor insertions. This policy
explains, in full, what the app does and does not do with your data.

The short version: **the app collects nothing, sends nothing anywhere,
and has no way to identify you.** Everything below explains exactly how.

---

## 1. Overview

DiabetesDevicesTracker is designed with privacy as a first principle. It
collects no personal information and operates with **no network
connectivity of any kind** — it does not contact any server, ours or
anyone else's, for any reason. There is no account, sign-in, or user
identifier of any kind anywhere in the app.

## 2. What data the app stores, and where

The only data the app stores is what you enter yourself: the date and
time you changed an infusion set or CGM sensor, and (optionally) a
sensor's serial number.

- This data is stored **only on your device**, using Apple's standard
  on-device storage (`UserDefaults`, shared through an App Group so the
  Home Screen/Lock Screen widget can display it too — see [§6](#6-home-screen--lock-screen-widget)).
- It is **not** synced to iCloud, backed up to any external service, or
  transmitted anywhere.
- It is **not** linked to your name, email address, Apple ID, device
  identifier, or any other form of identity — the app has no way to
  know who you are, because it never asks.

## 3. Data sharing

We share no data with any third party, because we never receive any data
in the first place — it never leaves your device. Specifically:

- The app makes **no network requests** of any kind.
- No analytics SDKs are included.
- No advertising SDKs are included.
- No crash-reporting or telemetry SDKs are included.
- No third-party libraries with their own data collection are included.

If you export your log as a CSV file (a feature you have to trigger
yourself, from Settings), that file is handed to iOS's standard share
sheet — you choose where it goes (Files, AirDrop, Mail, etc.). We have no
visibility into, or involvement in, that choice.

## 4. Camera

The app can use your device's camera to scan a CGM sensor's printed
serial number, so you don't have to type it manually. Camera access is
requested only when you tap the scan button — it is never active in the
background.

- Camera frames are processed **entirely on-device** using Apple's Vision
  framework (on-device text recognition).
- No image, frame, or video is ever saved, stored, or transmitted
  anywhere, by us or anyone else.
- The recognized serial number text is the only thing that reaches the
  app, and only after you confirm it.

## 5. Notifications

The app can send you local reminders (e.g., "your infusion set has been
in use for 3 days"). These are **local notifications**, scheduled and
delivered entirely on your device by iOS itself — they do not involve
Apple Push Notification servers, our servers, or any network connection.
No notification content or scheduling data is ever sent anywhere.

## 6. Home Screen / Lock Screen widget

If you add the app's widget to your Home Screen or Lock Screen, it reads
the same on-device data described in [§2](#2-what-data-the-app-stores-and-where) through an iOS App Group — a
mechanism Apple provides specifically so an app and its widget can share
local storage on the same device. This does not involve any network
transmission, and the same "nothing leaves your device" guarantee
applies to the widget as it does to the app itself.

## 7. Data deletion

You are always in control of your data:

- **Delete individual entries** from the Log tab at any time.
- **Delete everything at once** from Settings → Delete all records.
- **Uninstalling the app** removes all of its data permanently and
  immediately — there is nothing left behind on any server, because
  nothing was ever sent to one.

## 8. Children's privacy

This app is a tool for parents, caregivers, or the person managing their
own diabetes care — it is used *by* an adult to log device changes,
optionally *about* a child in their care. It does not knowingly collect
data from children as users of the app, does not require any account or
registration from anyone, and — as throughout this policy — does not
transmit any information about anyone, adult or child, off the device
it's installed on.

## 9. Your rights

Because DiabetesDevicesTracker collects no personal data and stores
everything exclusively on your own device, there is no server-side data
for us to access, export, correct, or delete on your behalf — you already
have complete, direct control over all of it through the app itself (see
[§7](#7-data-deletion)). This means requests under frameworks like the GDPR or CCPA are, in
practice, already fully satisfied by design: there is nothing held by us
to request.

## 10. Changes to this policy

If this policy changes, the "Effective date" at the top will be updated,
and the in-app copy (Settings → Privacy Policy) will be updated to match.
Material changes will be reflected in the app's release notes.

## 11. Contact

Questions about this policy or the app's privacy practices are welcome:

**Email:** DiabDevTracker@gmail.com

---

*This document is also shown in full within the app (Settings → Privacy
Policy) and is kept consistent with it — this GitHub version exists so
the policy can be linked publicly (e.g., from an App Store listing)
without requiring anyone to have the app installed.*
