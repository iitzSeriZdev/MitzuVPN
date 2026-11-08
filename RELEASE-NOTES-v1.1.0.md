# MitzuVPN 1.1.0

Servers from your other 3X-UI panels in the app, a VLESS / VMess / Trojan / Shadowsocks core inside the apps, free configs for free users, and fixes for the server list and the traffic counters.

## Downloads

| File | For |
|---|---|
| `MitzuVPN-1.1.0-universal.apk` | **Android** 7.0 or newer, any phone |
| `MitzuVPN-1.1.0-arm64-v8a.apk` | Android, modern 64-bit phones (smaller download) |
| `MitzuVPN-1.1.0-armeabi-v7a.apk` | Android, older 32-bit phones |
| `MitzuVPN-Setup-1.1.0.exe` | **Windows** 10 or 11, 64-bit |
| `MitzuVPN-1.0.0-chromium.zip` | **Browser extension** (unchanged) |
| `SHA256SUMS.txt` | Checksums |

## New

- **VLESS, VMess, Trojan and Shadowsocks in the app.** Android and Windows now carry their own core for these protocols (REALITY, TLS, WebSocket, gRPC, XHTTP, HTTPUpgrade and more). The panel's own VLESS/VMess/Trojan/Shadowsocks inbounds appear as locations too, next to WireGuard, OpenVPN and the others. Before a connection is reported as up, the app checks that the server really carries traffic.
- **External panels (3X-UI).** Add another server's 3X-UI panel (version 3 with an API key, or older versions with a username and password), tick the inbounds your users should get and give each one a name and flag of your own. Your paid users get them as locations in the app and in their subscription link; their usage there counts toward their traffic here, and their access follows their subscription. Resellers can add their own panels for their own customers.
- **Free configs.** A new page for config links and subscriptions that free users get in the app, next to the free network (optionally paid users too).
- **New inbounds go to every user** by themselves (a switch in App settings): an inbound you add reaches all your users at once, and an inbound you give a reseller reaches all of that reseller's customers.

## Fixed

- **Upload and download speeds** stayed at zero after connecting on Android, and on Windows with the free network in proxy mode. They now show the real traffic.
- **Refreshing the server list** shows a spinner and confirms when the list is up to date, and can no longer get stuck.
