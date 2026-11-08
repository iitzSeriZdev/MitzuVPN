# MitzuVPN 1.0.0

The first release of MitzuVPN: a fast, private VPN for **Android** and **Windows**, a **browser extension** for Chrome-based browsers, and the **server panel** that runs it all.

Use the free network with no setup, or sign in with a premium account for servers in many countries over modern protocols built for hard-to-reach networks.

## Downloads

| File | For | Size |
|---|---|---|
| `MitzuVPN-1.0.0-universal.apk` | **Android** 7.0 or newer, any phone (take this one if unsure) | 48 MB |
| `MitzuVPN-1.0.0-arm64-v8a.apk` | Android, modern 64-bit phones (smaller download) | 24 MB |
| `MitzuVPN-1.0.0-armeabi-v7a.apk` | Android, older 32-bit phones | 23 MB |
| `MitzuVPN-1.0.0-x86_64.apk` | Android emulators and x86 Chromebooks | 24 MB |
| `MitzuVPN-Setup-1.0.0.exe` | **Windows** 10 or 11, 64-bit | 72 MB |
| `MitzuVPN-1.0.0-chromium.zip` | **Browser extension** for Chrome, Edge, Opera, Brave and Vivaldi (premium accounts) | 1.3 MB |
| `mitzu-panel-linux-amd64` + `install-mitzu-panel.sh` | **Server panel** for operators: 64-bit Linux with systemd | 310 MB |
| `SHA256SUMS.txt` | Checksums of every file above | |

## What's inside

### Apps (Android and Windows)

- 🌍 **Free network for everyone**: connect for free with no setup; *Smart* mode finds the method that works on your internet and remembers it.
- ⭐ **Premium servers**: WireGuard, AmneziaWG, OpenVPN, Cisco, L2TP and IKEv2, plus a **gaming mode** on Windows; **Auto (fastest)**, a **Trade** section with fixed-IP servers, and a choice of **exit country**.
- 🔀 **Split tunneling** for sites, IP addresses and apps (Android) or programs (Windows).
- 🇮🇷 **Iranian sites without VPN**: Iranian sites and services open directly, so banks and payment pages keep working.
- 🛡️ **Protection**: block ads, trackers, malware and phishing, or choose **Family** to also block adult sites.
- 🧯 **Kill switch** on Windows, **local network access**, IPv6 leak protection, and **try the next server** when one doesn't answer.
- 💳 **Buy inside the app** by bank card or cryptocurrency; the plan activates by itself.
- 💬 **Support tickets** and an **inbox** inside the app, plus **renewal reminders**.
- ⭐ **Favorites**, an Android **home-screen widget** and shortcuts.
- ⚡ **Speed test** with a shareable result, and **free DNS** servers with live latency.
- 🎨 **8 colour themes** (light, dark or pure black) and **10 languages**: English, فارسی, دری, پښتو, Türkçe, العربية, Русский, Тоҷикӣ, Türkmen, 中文.
- 🔔 Tells you when a new version is out.

### Browser extension (premium accounts)

- 🧩 Protect **Chrome, Edge, Opera, Brave or Vivaldi** with one tap, without installing the app. Only that browser goes through MitzuVPN.
- Sign in with your username and password, or paste your login QR picture.
- Locations with latency and **Auto (fastest)**, your new IP and country, a **kill switch**, **WebRTC protection**, Iranian sites without VPN and your own sites that open directly.
- Same look and the same 10 languages as the apps, in light or dark.

### Server panel (for operators)

- **Ready-made setup** at install time: the VPN cores plus one working server per protocol, named after the server's country.
- Free and premium users, plans, device and speed limits, login QR codes, and a **sales panel for resellers** with their own prices and payment methods.
- Manage the apps from the panel: settings, notifications, support tickets, in-app ads, payments and update publishing.
- Exit countries, upstream configs, and a flag, location and Trade mark for every server.

## How to install

**Android**

1. Download the APK on your phone and open it. Allow your browser or file manager to install unknown apps if Android asks.
2. If **Google Play Protect** says *"App blocked to protect your device — Play Protect hasn't seen an app from this developer before"* or *"Unsafe app blocked"*, tap **More details → Install anyway**. This only means Google doesn't know MitzuVPN's developer yet.
3. If Android offers to **send the app for a security check**, tap **Send**: it helps Google learn that MitzuVPN is safe.
4. **Samsung**: if *Auto Blocker* refuses the install, turn it off for a moment in **Settings → Security and privacy**, install, then turn it back on.
5. Open MitzuVPN and allow the **VPN connection** the first time you connect.

**Windows**

1. Run `MitzuVPN-Setup-1.0.0.exe`. If **"Windows protected your PC"** appears, click **More info → Run anyway**.
2. Allow the installer to make changes: it installs the VPN service and network driver MitzuVPN needs.

**Browser extension**

1. Extract `MitzuVPN-1.0.0-chromium.zip` to a folder you keep (don't delete it later: the browser runs the extension from it).
2. Open `chrome://extensions`, `edge://extensions` or `opera://extensions` and turn on **Developer mode**.
3. Click **Load unpacked**, choose the extracted folder, then pin MitzuVPN on the toolbar and sign in.

**iPhone and other apps**

Premium accounts have a **subscription link** (in the app: **Account → Subscription link**). Add it to any iPhone VPN app that accepts subscription links, such as *V2Box* or *Streisand*.

**Server**

Put `mitzu-panel-linux-amd64` and `install-mitzu-panel.sh` side by side on a clean 64-bit Linux server (Ubuntu 24.04 or Debian 12 recommended) and run:

```bash
sudo bash install-mitzu-panel.sh
```

Choose a real Let's Encrypt certificate for your domain: the apps only talk to a trusted HTTPS address.

## Verify your download

Each file's SHA-256 is in `SHA256SUMS.txt`.

- Linux or macOS, in the download folder: `sha256sum -c --ignore-missing SHA256SUMS.txt`
- Windows PowerShell: `Get-FileHash .\MitzuVPN-Setup-1.0.0.exe -Algorithm SHA256`

<details>
<summary>SHA-256 checksums</summary>

```text
4fee872eb9c829fc6305142b92f4ad551878ca7d0c2a31764a2a6501d0f6a0ba  MitzuVPN-1.0.0-universal.apk
1ea2fbe66143c4394c173445253ef0c0adbe8a66d6c898dcdb59a4045f993b4c  MitzuVPN-1.0.0-arm64-v8a.apk
3f8f15babae543e9b51cf55ea4ed3649ff73792aa1748703d2f691f3c06c6fc8  MitzuVPN-1.0.0-armeabi-v7a.apk
eadb1789a1f63bd45b962134773f0680088b377cf27747f9520bb474a4cb20b9  MitzuVPN-1.0.0-x86_64.apk
1ad607a3b364ff8019be04cb5f2c5050e213fe759fd61cc834c56e5e58d59c8f  MitzuVPN-Setup-1.0.0.exe
72172b3c5c4a3230d4283c7e9cd551b3fbeb957282a2f2c146f3953997ff7558  MitzuVPN-1.0.0-chromium.zip
a362207101eb1ebfc89e987b980907e263a54c55dccfd35d6a06414f929f9d6b  mitzu-panel-linux-amd64
782884f0ec6cf61e208f91bacddb0c9a853ea37e71830ad306a1e629b0f75c6f  install-mitzu-panel.sh
```

</details>

## Stay safe

Only download MitzuVPN from this page or from our Telegram channel **[@MitzuVPN](https://t.me/MitzuVPN)**. Copies from anywhere else may have been changed.

## Support

News, servers and help: **[t.me/MitzuVPN](https://t.me/MitzuVPN)**. Signed-in users can also open a support ticket inside the app.
