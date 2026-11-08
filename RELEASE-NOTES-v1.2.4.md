# MitzuVPN 1.2.4 — release notes

<div dir="rtl">

## فارسی

### صفحهٔ لودینگ تازه

اسپلش از نو ساخته شد: لوگو از ۱۶٪ تا ۱۴۸٪ بزرگ می‌شود، یک لحظه می‌ایستد، بعد جمع می‌شود و
«MitzuVPN» کنارش باز می‌شود و در پایان کل قفل کوچک می‌شود و می‌رود. پس‌زمینهٔ آن ثابت و تیره است
(`#0C0E14`) و با تم برنامه عوض نمی‌شود — صفحهٔ لودینگ نباید وسط راه رنگ عوض کند. پخش‌کنندهٔ قبلی که
فریم‌به‌فریم تصویر نشان می‌داد کامل حذف شد.

### کیف پول

روی حساب شما یک موجودی تومانی نشست. نماینده یا پشتیبانی می‌تواند آن را شارژ کند، و در تب
**اشتراک‌ها**، اگر موجودی برای پلن کافی باشد، **پرداخت از کیف پول** اولین گزینهٔ پرداخت است:
بدون درگاه، بدون رسید، بدون انتظار. با زدنش پلن همان لحظه فعال می‌شود.

موجودی هرگز منفی نمی‌شود و هر شارژ و هر خرج در دفتر کل ثبت می‌شود — پس هر عددی در کیف پول
قابل توضیح است.

### کد هدیه

بالای پلن‌ها یک فیلد **کد هدیه** اضافه شد. کد را وارد کنید و مبلغش فوراً به کیف پول می‌نشیند.

- کد می‌تواند برای **همه** باشد، فقط برای **کاربران یک نماینده**، یا فقط برای **حساب‌های مشخص**.
- برای هر کاربر می‌توان سقف گذاشت: یک‌بار، چند بار، یا بی‌نهایت.
- سقف کل استفاده و تاریخ انقضا هم قابل تنظیم است.
- فیلد فقط حروف و عدد **انگلیسی** و خط تیره را می‌پذیرد؛ عدد فارسی هنگام تایپ خودکار به انگلیسی
  تبدیل می‌شود و حرف فارسی اصلاً نوشته نمی‌شود (بدون پیام خطا، چون چیزی خراب نیست).
- نتیجه **زیر خود فیلد** نشان داده می‌شود: سبز برای موفقیت، و برای خطا دلیل دقیق — کد وجود ندارد،
  غیرفعال است، منقضی شده، برای این حساب نیست، قبلاً استفاده شده، یا ظرفیتش تمام شده است.

### موقعیت‌ها

زیرمجموعه‌های هر کشور (کانکشن ۱، ۲، ۳ …) حالا پرچم **کوچک‌تری** دارند: ۳۲ در برابر ۴۲ در ردیف
کشور، یعنی حدود ۲۴٪ کوچک‌تر. با یک نگاه معلوم است این‌ها داخل همان کشور هستند، بدون اینکه لازم
باشد برچسب را بخوانید.

### از نسخهٔ ۱.۲.۳ (اگر مستقیم از ۱.۲.۲ می‌آیید)

- **اتصال خودکار** فقط داخل همان بخشی کار می‌کند که باز شده — در وب‌گردی فقط سرورهای وب‌گردی را
  تست می‌کند و از دستهٔ دیگر چیزی برنمی‌دارد.
- دکمهٔ **بازگشت به چهار بخش** بزرگ‌تر و با رنگ هشدار شد.

</div>

---

## English

### A new loading screen

The splash was rebuilt from scratch: the mark scales from 16% to 148%, holds for a moment, settles
back and the **MitzuVPN** wordmark unfolds beside it, then the whole lock shrinks away. Its background
is a fixed dark `#0C0E14` — the splash never follows the theme, because a loading screen that changes
colour halfway is a bug, not a feature. The old frame-by-frame player is gone.

### Wallet

Your account now carries a balance in Toman. Your seller or support can top it up, and in the
**Plans** tab, when the balance covers a plan, **Pay from wallet** is the first payment option — no
gateway, no receipt, no waiting. The plan is active the moment you tap it.

The balance can never go negative, and every top-up and every purchase writes a ledger row, so any
number in the wallet can be explained afterwards.

### Gift codes

A **Gift code** field sits above the plans. Type a code and its amount lands in the wallet at once.

- A code can be for **everyone**, for **one reseller's customers**, or for **specific accounts**.
- Each user can be limited to one use, several, or no limit at all.
- A total cap and an expiry date can be set as well.
- The field accepts **English** letters, digits and the dash only; Persian digits are converted to
  ASCII as you type and Persian letters are simply not entered — nothing happens, which is the
  intended feedback.
- The result appears **under the field**: green for success, and for a failure the exact reason — the
  code is unknown, switched off, expired, not for this account, already used, or used up.

### Locations

The connections under a country (Connection 1, 2, 3 …) now carry a **smaller flag**: 32 dp against the
country row's 42 dp, about 24% smaller. The nesting is obvious at a glance, without reading the label.

### From 1.2.3 (if you are coming straight from 1.2.2)

- **Auto Connect** stays inside the section it was opened from — in web browsing it measures only web
  browsing servers instead of picking one from another category.
- The **back to the four sections** control is larger and warning-coloured.

---

## Files

| File | Size | SHA-256 |
|---|---|---|
| `MitzuVPN-1.2.4-universal.apk` | 101,549,084 | `60bb9fcaac65…d81cdc` |
| `MitzuVPN-1.2.4-arm64-v8a.apk` | 42,707,694 | `4722358f3eb9…65c386` |
| `MitzuVPN-1.2.4-armeabi-v7a.apk` | 42,464,854 | `3bb8bdbde2df…0666f0` |
| `MitzuVPN-1.2.4-x86_64.apk` | 44,900,868 | `f0cd26e6ab79…a3a96c` |
| `MitzuVPN-Setup-1.2.4.exe` | 96,386,841 | `fb16c7d67e92…57ebee` |

`SHA256SUMS.txt` in this release carries the full hashes.

**Requirements:** Android 7.0 or newer · Windows 10 or 11, 64-bit.

---

## Upgrading

Install the new build over the old one. Your account, settings, servers and wallet stay as they are.
This update is **optional**: 1.2.3 keeps working, and the app offers 1.2.4 when you open it.
