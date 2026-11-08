# MitzuVPN 1.0.2

The free network now connects on networks that block every WARP route, and the apps load faster and more reliably.

## Downloads

| File | For |
|---|---|
| `MitzuVPN-1.0.2-universal.apk` | **Android** 7.0 or newer, any phone |
| `MitzuVPN-1.0.2-arm64-v8a.apk` | Android, modern 64-bit phones (smaller download) |
| `MitzuVPN-1.0.2-armeabi-v7a.apk` | Android, older 32-bit phones |
| `MitzuVPN-Setup-1.0.2.exe` | **Windows** 10 or 11, 64-bit |
| `MitzuVPN-1.0.0-chromium.zip` | **Browser extension** (unchanged) |
| `SHA256SUMS.txt` | Checksums |

## Free network

- **New relay route.** When the filter blocks the WARP routes (and even the free sign-up), Smart mode now moves on to a relay network that gets through. It needs nothing from your server and uses none of its bandwidth.
- **Connected in seconds.** Smart mode starts the WARP route and the relay at the same moment and keeps whichever carries traffic first; the other stops at once. On a filtered connection in Iran this took about 4 seconds the first time and about 2 seconds after that. Routes that cannot work are dropped as soon as that is clear.
- Disconnecting always stops every part of the free connection.
- Operators can turn the relay route off under **App settings → Free network**.

## Apps

- **Sign out** happens at once, even on a slow network.
- **Faster loading:** the apps keep their connection to the server open between requests, try both server addresses side by side when one is slow, and retry a failed load once by themselves.
- Pages that could not load now say so and offer **Try again** (support tickets, inbox, devices, plans, exit countries), instead of an endless spinner or an empty list.
- Inbox and support tickets are loaded in the background, so they open at once.
