# Privacy Policy
**Archy** - The Archer's best friend

Last updated: 8 July 2026

# Overview

Archy ("the app") is an offline-first archery scoring application developed by
EbnigmaApps ("we", "us"). This policy explains what data the app handles and how.

The short version: **Archy has no user accounts, contains no advertising, and
uses no analytics or tracking. Your scoring data lives on your device. We do
not collect, sell, or transmit your personal data to us or to any third
party.**

## 1. Data stored on your device

Everything you create in Archy is stored **locally on your device** and is not
sent to us. This includes:

- Sessions, ends, and individual arrow scores
- Shooter names, bows, courses, variants, and target labels you enter
- Custom scoring systems you create
- Statistics derived from your scoring history
- App settings and preferences

This data stays on your device unless **you** choose to export or share it (see
sections 3 and 4). Uninstalling the app removes this data from your device.

## 2. Data Collection

**None.** Archy does not create an account for you, does not require you to log
in, and does not contain any analytics, crash-reporting, advertising, or
tracking software. We have no servers that receive your personal scoring data,
and we do not build user profiles.

## 3. Optional networking features (you initiate all of them)

Archy works completely offline. Some optional features involve a network or a
direct device-to-device connection, and are only active when **you** start
them:

### Live group rounds (LAN or cloud relay)
You can score a round together with other archers. You may host over your
local network / hotspot (fully offline, no internet), or connect through a
cloud relay server. In both cases:

- All shared data (scores, names) is **end-to-end encrypted on your device**
  before it leaves it. The encryption key is exchanged directly between
  participants via a QR code or join code and never reaches the relay.
- A relay server only forwards **encrypted** data between participants and
  **cannot read your scores, names, or anything else**. It has no user
  accounts and asks for no personal information.
- **Ephemeral by design:** a round's data lives only in the relay's memory for
  the duration of the round and is evicted after a period of inactivity.
  Nothing is written to disk and nothing is persisted after the round ends.

**The default cloud relay is operated by us (EbnigmaApps)** for convenience.
Because it is a zero-knowledge relay, we cannot see your scoring data. As with
any internet server, when your device connects to the relay the relay (and its
hosting provider) necessarily receives your device's IP address in order to
route the connection; this is used only to forward the encrypted traffic and is
not used to identify you or combined with your scoring data. If you prefer, you
can run your own relay and point the app at it in Settings, or avoid the cloud
relay entirely by hosting live rounds over your local network.

### Nearby device-to-device connection and Wear OS sync
Archy can connect directly to a nearby device (via Bluetooth / Wi-Fi) or to a
paired Wear OS watch to transfer or mirror a scoring session. This is a direct
connection between your own devices/participants; the data is not routed to us.

### Offline QR transfer
You can move a finished session to another device by displaying and scanning
QR codes. This involves no network at all.

## 4. Data export and sharing

At your request, Archy can export your data — for example as a ZIP backup of
JSON files or as a CSV file. When you export or share this data (via Android's
share sheet, saving to a file, etc.), it goes wherever **you** choose to send
it. We are not involved in and have no access to those exports.

## 5. Permissions

Archy requests certain Android permissions only to support the optional
features above:

- **Internet / Network state** — for optional live rounds via a relay.
- **Bluetooth, Wi-Fi, and Nearby Wi-Fi devices** — for direct device-to-device
  live rounds and transfers via Nearby Connections. Archy declares these scan
  permissions as **"never used for location"** and does **not** access your
  physical location.
- **Wake lock** — to keep the screen usable while scoring or in Wear OS ambient
  mode.
- **Camera** (when you use it) — to scan QR codes for joining a round or
  importing a session. Camera images are used only for on-device QR scanning
  and are not stored or transmitted.

## 6. Children's privacy

Archy is a general-audience scoring tool and does not knowingly collect any
personal information from anyone, including children.

## 7. Third parties

Archy does not include advertising or analytics SDKs and does not share your
data with third parties. Standard platform components (e.g. Google Play
Services for Nearby Connections and Wear OS communication) are used only to
enable the optional connectivity features described above and operate under
their own providers' terms.

## 8. Changes to this policy

If this policy changes, we will update the "Last updated" date above and post
the revised policy at the same URL. Continued use of the app after changes
constitutes acceptance of the updated policy.

## 9. Contact

If you have questions about this privacy policy, you can reach the developer through the GitHub repository:
https://github.com/Ebnigma/archy-privacy

or e-Mail
ebnigma.apps@gmail.com