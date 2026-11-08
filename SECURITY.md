# Security

## Reporting a problem

Please **do not** open a public issue for a security problem. Send a message to
[**@MitzuVPN**](https://t.me/MitzuVPN) on Telegram with:

- what you found and which version or platform it affects,
- the steps to reproduce it,
- and, if you have one, a proof of concept.

We will confirm that we received it and tell you what we found. Please give us time to ship a fix
before writing about it in public.

## What is in scope

- The Android app, the Windows app and the browser extension.
- The subscription and update endpoints the apps talk to.
- The panel behind the service.

## What is out of scope

- Reports that only say a file "looks suspicious" without a reproducible problem.
- Missing security headers on the marketing site.
- Anything that needs physical access to an unlocked device, or an already-rooted device with the
  attacker's code on it.
- Social engineering of our users or our staff.

## Checking a download

Every release ships a `SHA256SUMS.txt`. Compare it before installing:

```bash
sha256sum MitzuVPN-1.2.4-arm64-v8a.apk
```

On Windows:

```powershell
Get-FileHash .\MitzuVPN-Setup-1.2.4.exe -Algorithm SHA256
```

Only download from this repository's **Releases**, from [mitzuui.com](https://mitzuui.com), or from
the channel above. A file from anywhere else is not ours.
