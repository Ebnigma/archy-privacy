# Privacy Policy
**Archy** - The Archer's best friend

Last updated: 12 August 2026

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

**Not available in the current release.** Live shared rounds are switched off
while the feature is being reworked, so this build never contacts a relay and
never opens a round to other devices. The description below applies to
releases in which the feature is enabled again; it is kept here so the policy
does not have to change under you when it returns.

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

### Wear OS sync and handing a round to another device

Archy communicates with your own paired Wear OS watch to transfer or mirror a
scoring session. It can also hand a finished round to another phone over your
local Wi-Fi or hotspot: the sending device opens a short-lived connection on
the local network, the receiving device scans a QR code carrying the address
and an encryption key, and the round moves directly between the two devices.
Both are direct connections between the devices involved — nothing is routed
through a server of ours, and the transferred round is encrypted with a key
that exists only inside that QR code.

Direct Bluetooth / Wi-Fi Direct connections to a nearby device (Nearby
Connections) belong to the live-round feature that is switched off in the
current release. **This release requests no Bluetooth or nearby-device
permissions at all.**

### Sending a round as a file
You can move a finished session to another device by sending it as a
`.archysession` file through your device's share sheet (Quick Share, mail,
saving to files). This involves no server of ours: the file goes exactly
where you send it. Archy can also open such a file it receives from another
app; the contents are imported locally after you confirm the preview.

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

- **Internet / Network state** — to open the local-network connection used when
  you hand a round to another device (section 3), and for the Google Play
  Services component that decodes QR codes. This release contacts no server of
  ours.
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
- **Local network** (when you hand a round to another device) — to transfer the
  round over Wi-Fi or a hotspot. This access is not used for discovery or
  tracking outside that transfer you started.

This release does **not** request Bluetooth or nearby-device permissions. They
belong to the live group rounds described in section 3 and will return only in
a release that switches that feature back on; if that happens, this policy and
the permission list here are updated in the same release.

## 6. Children's privacy

Archy is a general-audience scoring tool and does not knowingly collect any
personal information from anyone, including children.

## 7. Third parties

Archy does not include advertising or analytics SDKs and does not share your
data with third parties. Standard platform components (e.g. Google Play
Services for Wear OS communication and for decoding QR codes) are used only to
enable the features described above and operate under their own providers'
terms.

## 8. Changes to this policy

If this policy changes, we will update the "Last updated" date above and post
the revised policy at the same URL. Continued use of the app after changes
constitutes acceptance of the updated policy.

## 9. Contact

If you have questions about this privacy policy, you can reach the developer through the GitHub repository:
https://github.com/Ebnigma/archy-privacy

or e-Mail
ebnigma.apps@gmail.com
