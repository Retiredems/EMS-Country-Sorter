<!-- ems-callout -->
> **v1.0.6 — refreshed brand and a polished activation flow.** Same software, sharper edges. [→ Download the latest build](https://github.com/Retiredems/EMS-Country-Sorter/releases/latest)
<!-- ems-callout -->
<p align="center">
  <img src="assets/icon.png" alt="EMS Country Sorter" width="96"/>

  <img width="835" height="559" alt="IMG_5532" src="https://github.com/user-attachments/assets/f745766f-bb83-4263-9bbc-5f9844c0c934" />

</p>

<h1 align="center">EMS Country Sorter</h1>

<p align="center">
  <strong>Precision Address Intelligence</strong><br/>
  A professional desktop tool that sorts bulk email lists by country — instantly, accurately, at any scale.
</p>

<p align="center">

</p>

---

## What Is EMS Country Sorter?

EMS Country Sorter is a native desktop application that takes a raw email list — any size — and sorts every address into country-specific files automatically. No manual work, no scripting, no cloud upload required.

Built for **email marketers**, **mailer operators**, and **list managers** who need clean, geo-segmented lists fast — on any Windows or macOS machine.

---

## Screenshots
<img width="1066" height="667" alt="Screenshot 2026-05-03 at 05 43 16" src="https://github.com/user-attachments/assets/560c1df8-74ea-4712-92a8-d75ae19598c4" />
<img width="1063" height="671" alt="Screenshot 2026-05-03 at 11 39 17" src="https://github.com/user-attachments/assets/2c8017e3-3678-48f6-b3e0-577ffb1c11c1" />
<img width="1063" height="670" alt="Screenshot 2026-05-03 at 11 39 38" src="https://github.com/user-attachments/assets/2e193315-9349-4d80-bfcb-387208495c81" />
<img width="1064" height="670" alt="Screenshot 2026-05-03 at 11 40 11" src="https://github.com/user-attachments/assets/9cb3543f-5237-4608-b290-e45660d989fe" />
<img width="1064" height="671" alt="Screenshot 2026-05-03 at 11 40 36" src="https://github.com/user-attachments/assets/34460478-7746-4daa-be93-fe24d9a61063" />
<img width="1062" height="675" alt="Screenshot 2026-05-03 at 14 43 03" src="https://github.com/user-attachments/assets/77ada22f-3076-49f9-8f6d-0e7d5303fd9c" />
<img width="1142" height="599" alt="Screenshot 2026-05-03 at 15 17 10" src="https://github.com/user-attachments/assets/b07b602d-daf6-4dd0-80bd-678a70f06e08" />

---

## Key Features

### Triple-Layer Country Detection
| Method | How It Works |
|--------|-------------|
| TLD Resolver | Instantly maps `.uk`, `.de`, `.br` and 250+ ccTLDs to countries — zero network calls |
| DNS / MX Lookup | Resolves the mail server for any domain and geolocates the hosting IP |
| GeoIP (MaxMind) | Local offline database — no rate limits, works for any IP, no internet required |

All three layers work together. If TLD gives a confident match, it's used instantly. DNS and GeoIP fill in the rest — including generic TLDs like `.com`, `.net`, `.org`.

### Bulk Processing
- Load email lists from `.txt`, `.csv`, or `.xlsx` — one address per line, any size
- Drag and drop files directly onto the window
- Automatic deduplication before sorting
- Configurable thread count (1–10) for tuning speed vs. resource use

### Live Country Table
- All 249 ISO countries pre-loaded — you see everything at once, not just what was found
- Rows flash green as emails are sorted in real-time
- Final sort: countries with matches move to the top, ordered by count
- Double-click any completed row to open its output file directly

### Output
- One `.txt` file per country, named `CountryName.txt` (or ISO code, or both — configurable)
- Unknown / unresolved addresses written to `Unknown.txt` — nothing is lost
- Export all output files as a single ZIP archive in one click

### Domain Cache
- Every resolved domain is stored in a local SQLite cache
- Repeat runs on the same domain list are near-instant
- Cache survives app restarts; clear it from Settings when needed

### Status Bar
- Live counters: Loaded · Sorted · Countries Found · Cached · Threads
- State indicator: Idle → Running → Paused → Done

### Dark & Light Themes
- Premium dark UI (default) with glowing teal accents
- Clean light theme — switch instantly from the toolbar

---

## Installation

### Windows

1. Download `EMS-Country-Sorter-Setup.exe` from the [latest release](../../releases/latest)
2. Run the installer — follow the setup wizard
3. A desktop shortcut is created automatically
4. Enter your license key on first launch

> Installs per-user (no admin required). Works on any Windows 10 / 11 desktop, laptop, VPS, or RDP environment.

### macOS

1. Download `EMS_Country_Sorter_macOS.zip` from the [latest release](../../releases/latest)
2. Unzip and drag `EMS Country Sorter.app` to your Applications folder
3. Right-click → Open on first launch (Gatekeeper bypass for unsigned builds)
4. Enter your license key

---

## Getting a License

EMS Country Sorter is a **commercial product**. Licenses are hardware-tied — no cloud check-in required after activation.

👉 **Telegram: [@retiredems](https://t.me/retiredems)**
🤖 **Bot: [@emsmailerbot](https://t.me/emsmailerbot)**

**Plans available:**
| Plan | Devices |
|------|---------|
| Monthly | 1 PC |
| Yearly | 2 PCs |
| Lifetime | 3 PCs |

---

## How to Get a License Key

1. Open EMS Country Sorter — your Hardware ID (HWID) is shown in the Activation screen
2. Copy your HWID
3. Open Telegram → [@emsmailerbot](https://t.me/emsmailerbot)
4. Select **🌍 EMS Country Sorter** → submit your HWID and name
5. Complete payment → receive your key → paste it into the app

Your license is tied to your machine hardware. If you reinstall Windows or move to a new machine, contact [@retiredems](https://t.me/retiredems) to transfer it.

---

## Input File Format

Load a plain text, CSV, or Excel file — one email per line:

```
user@example.co.uk
hello@gmail.com
contact@empresa.com.br
info@firma.de
```

Mixed formats and headers are handled automatically. Duplicates are removed before sorting begins.

---

## System Requirements

| | Windows | macOS |
|-|---------|-------|
| OS | Windows 10 / 11 (64-bit) | macOS 11+ (Intel or Apple Silicon) |
| RAM | 256 MB minimum | 256 MB minimum |
| Disk | 200 MB | 200 MB |
| Network | Required for DNS/MX detection | Required for DNS/MX detection |

> Works fully offline for TLD-based detection. Network is only needed for DNS lookups on generic TLDs (`.com`, `.net`, etc.).

---

## Changelog

### v1.0.0 — May 2026

- Initial public release
- Triple-layer detection: TLD resolver, DNS/MX lookup, MaxMind GeoIP
- 250+ ccTLD mappings for instant offline detection
- MaxMind GeoLite2 local database — no rate limits, no API keys
- All 249 ISO countries pre-loaded in the live table
- Configurable thread count (1–10)
- TXT, CSV, XLSX input support with drag & drop
- Per-country `.txt` output with ZIP export
- Local SQLite domain cache for repeat-run speed
- Dark / light theme
- Hardware-tied license with offline validation

---

## Other EMS Tools

| Tool | Description |
|------|-------------|
| [EMS Mailer](https://github.com/Retiredems/Ems-Mailer) | Bulk email sending — SMTP, rotating accounts, templates |
| [EMS Mail Fetcher](https://github.com/Retiredems/EMS-Mail-Fetcher) | Bulk IMAP/POP3 account tester and email archiver |

---

## Support

Open an issue on GitHub for bug reports and feature requests.

---

<p align="center">
  Built with precision by <strong>Retiredems</strong> &nbsp;·&nbsp; Powered by PyQt6
</p>
