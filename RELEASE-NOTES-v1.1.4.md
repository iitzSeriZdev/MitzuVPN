# MitzuVPN 1.1.4

Latency and the connected state are honest now: a server that only looks reachable no longer shows a green ping, and Windows checks that real traffic passes after connecting instead of showing a silent green screen. The server panel is updated to the same version (1.1.4); its features are unchanged.

## Downloads

| File | For |
|---|---|
| `MitzuVPN-1.1.4-universal.apk` | **Android** 7.0 or newer, any phone |
| `MitzuVPN-1.1.4-arm64-v8a.apk` | Android, modern 64-bit phones (smaller download) |
| `MitzuVPN-1.1.4-armeabi-v7a.apk` | Android, older 32-bit phones |
| `MitzuVPN-Setup-1.1.4.exe` | **Windows** 10 or 11, 64-bit |
| `MitzuVPN-1.0.0-chromium.zip` | **Browser extension** (unchanged) |
| `mitzu-panel-linux-amd64` + `install-mitzu-panel.sh` | **Server panel**, Linux 64-bit (now 1.1.4) |
| `SHA256SUMS.txt` | Checksums |

## Fixed

- **Real ping for app-core servers.** VLESS / VMess / Trojan / Shadowsocks and Cisco servers now need a completed TCP handshake to show a latency: a machine that answers with "port closed" no longer shows a green millisecond value — the location shows "no answer" until its core is actually up. UDP protocols (WireGuard, IKEv2, L2TP…) keep the old behavior, since their TCP port is closed by design.
- **"Connected" is verified on Windows.** Right after the tunnel comes up the app now proves that real data gets out (a tiny HTTP request and a DNS round trip through the tunnel). If the server is connected in name only and nothing passes, the app says so instead of showing a silent green screen — and it keeps re-checking, so the moment traffic starts flowing the screen returns to Connected by itself.
- This also means automatic connect is no longer fooled: it only ranks locations that really answer.
