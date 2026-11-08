# MitzuVPN 1.0.1

A fix-up release for the apps, and the new **MitzuVPN website** built into the server panel.

## Downloads

| File | For | Size |
|---|---|---|
| `MitzuVPN-1.0.1-universal.apk` | **Android** 7.0 or newer, any phone (take this one if unsure) | 48 MB |
| `MitzuVPN-1.0.1-arm64-v8a.apk` | Android, modern 64-bit phones (smaller download) | 24 MB |
| `MitzuVPN-1.0.1-armeabi-v7a.apk` | Android, older 32-bit phones | 23 MB |
| `MitzuVPN-1.0.1-x86_64.apk` | Android emulators and x86 Chromebooks | 24 MB |
| `MitzuVPN-Setup-1.0.1.exe` | **Windows** 10 or 11, 64-bit | 72 MB |
| `MitzuVPN-1.0.0-chromium.zip` | **Browser extension** for Chrome, Edge, Opera, Brave and Vivaldi (premium accounts; unchanged since 1.0.0) | 1.3 MB |
| `mitzu-panel-linux-amd64` + `install-mitzu-panel.sh` | **Server panel** for operators: 64-bit Linux with systemd | 311 MB |
| `SHA256SUMS.txt` | Checksums of every file above | |

Installing over 1.0.0 keeps your sign-in and settings. The Android app is signed with the same key as before.

## Fixed

- **Android:** the app closed when you tapped **Disconnect** while it was still connecting (most often on the free network). It now stops cleanly.
- **Android and Windows:** an unexpected error no longer closes the app silently; you get a message and the app keeps running.
- **Windows:** disconnecting in the middle of a connection attempt no longer shows that attempt's error afterwards.

## Improved

- **Custom DNS** now has two fields: a primary address and an optional secondary one. Both are checked, and a wrong address is pointed out before you connect.

## New: the MitzuVPN website

The server panel now carries a complete website, in the apps' design and in all 10 languages:

- Every feature of the apps, a free-versus-premium comparison, FAQ and terms of use.
- Downloads for **Android**, **Windows** and the **Chrome extension**, taken from the builds the operator publishes in the panel.
- **Prices and buying online** with the same payment methods as the apps: card to card with a receipt upload, or cryptocurrency with an address QR code. The page follows the payment and shows when the plan is active.
- A visitor's **account page**: plan, expiry, data used and the **subscription link for iPhone**.

For operators: the site answers at `https://<your-domain>:8443/`. **MitzuVPN App → App settings → Website → Open the website on port 443** also serves it at `https://<your-domain>` through the VLESS Reality inbound, while VPN users keep connecting on the same port. iPhone users should refresh their subscription once after that switch. Details are in the server guide (`Server-Guide-EN.md`, "Website").

## Upgrading a server

Copy the new `mitzu-panel-linux-amd64` and `install-mitzu-panel.sh` to the server and run `sudo bash install-mitzu-panel.sh`; it detects the existing panel, backs it up and updates it in place. Your users, plans and inbounds stay as they are.

## Checksums

Check a download against `SHA256SUMS.txt`: on Linux `sha256sum -c SHA256SUMS.txt`, on Windows `Get-FileHash <file> -Algorithm SHA256`.
