# Privacy Policy
**Archy** - The Archer's best friend

Last updated: 11 July 2026

# Overview

Archy ("the app") is an offline-first archery scoring application developed by
EbnigmaApps ("we", "us"). This policy explains what data the app handles and how.

The short version: **Archy has no user accounts, contains no advertising, and
uses no analytics or tracking. Your scoring data lives on your device. We do
not collect or sell it. An optional cloud relay receives only encrypted round
traffic and the network information needed to carry it, as described below.**

## 1. Data stored on your device

Everything you create in Archy is stored **locally on your device** and is not
sent to us. This includes:

- Sessions, ends, and individual arrow scores
- Shooter names, bows, courses, variants, and target labels you enter
- Custom scoring systems you create
- Statistics derived from your scoring history
- App settings and preferences
- If you turn on activity tracking for a round: your step count, walking
  distance, elevation gain, and GPS route for that round (see section 3a)

This data stays on your device unless **you** choose to export or share it (see
sections 3 and 4). Uninstalling the app removes this data from your device.

## 2. Data Collection

Archy does not create an account for you, require you to log in, or contain
analytics, crash-reporting, advertising, or tracking software. We do not
receive readable scoring content and do not build user profiles. If you choose
an internet relay, that server necessarily receives your IP address and
encrypted traffic while it routes the round; details are below.

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

Cloud relay availability depends on the build you installed. A distributor can
configure a built-in relay at build time; otherwise cloud rounds stay disabled
until you enter a self-hosted relay URL in Settings. Settings always shows which
case applies. If an official Archy build includes a built-in relay, it is
operated by EbnigmaApps. Because it is zero-knowledge, we cannot see your
scoring content. The relay and its hosting provider necessarily receive your IP
address to route the connection; it is not used to build a profile or combined
with scoring content. You can always self-host, use LAN/Nearby instead, or avoid
network rounds entirely.

### Nearby device-to-device connection and Wear OS sync
Archy can connect directly to a nearby device (via Bluetooth / Wi-Fi) or to a
paired Wear OS watch to transfer or mirror a scoring session. This is a direct
connection between your own devices/participants; the data is not routed to us.

### Offline QR transfer
You can move a finished session to another device by displaying and scanning
QR codes. This involves no network at all.

## 3a. Optional activity tracking (off by default)

You can choose to record your walk during a round — steps, distance,
elevation gain, and the GPS route. This is **off by default** and enabled per
round; while recording, Android shows a persistent notification.

- All recorded location and motion data is **stored only on your device** and
  is never transmitted to us or anyone else.
- Live group rounds and the QR codes you share with other archers **never
  contain your route or steps** — only your own full backups and the transfer
  between your own watch and phone carry them.
- The shareable result image shows at most the aggregate numbers (steps,
  distance, elevation) that are visible in its preview, never the route.
- Deleting a session deletes its recorded activity; uninstalling the app
  removes everything.

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
- **Location** (only if you turn on activity tracking for a round) — to record
  your walking route and elevation during that round. Recording runs as a
  visible foreground service so it keeps working with the screen off; Archy
  does not request background location. The route is stored only on your
  device (see section 3a).
- **Physical activity** (only if you turn on activity tracking) — to count
  your steps during the round via the device's step sensor. Stored only on
  your device.
- **Camera** (when you use it) — to scan QR codes for joining a round or
  importing a session, or to take a shooter photo. QR camera images are used
  only for on-device scanning and are not stored or transmitted; a shooter
  photo is copied only into Archy's private on-device storage.
- **Photo library** (when you use it) — to choose a shooter photo. Archy copies
  only the image you select into its private on-device storage.
- **Local network** (when you start a LAN round) — to host or join a live group
  round over Wi-Fi or a hotspot. This access is not used for discovery or
  tracking outside that user-initiated round.

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
