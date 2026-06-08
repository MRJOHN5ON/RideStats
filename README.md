<p align="center">
  <img src="./media/icon/app_icon.png" alt="RideStats app icon" width="120" />
</p>

<h1 align="center">RideStats</h1>

<p align="center">
  <strong>A personal ride logger for Android</strong><br>
  Record forces · review your rides · keep everything on your phone
</p>

<p align="center">
  <img src="https://img.shields.io/badge/platform-Android-3DDC84?style=flat-square" alt="Android" />
  <img src="https://img.shields.io/badge/built%20with-Flutter-02569B?style=flat-square&logo=flutter&logoColor=white" alt="Flutter" />
  <img src="https://img.shields.io/badge/privacy-local--only-28D7FF?style=flat-square" alt="Local only" />
  <img src="https://img.shields.io/badge/latest-1.1.2-8B9BB0?style=flat-square" alt="v1.1.2" />
</p>

<p align="center">
  <a href="https://github.com/MRJOHN5ON/RideStats/releases/tag/v1.1.2"><strong>Download v1.1.2</strong></a>
  &nbsp;·&nbsp;
  <a href="https://github.com/MRJOHN5ON/RideStats/releases/tag/v1.1.1">Download v1.1.1</a>
  &nbsp;·&nbsp;
  <a href="https://github.com/MRJOHN5ON/RideStats/releases/tag/v1.1.0">Download v1.1.0</a>
  &nbsp;·&nbsp;
  <a href="https://github.com/MRJOHN5ON/RideStats/releases/tag/v1.0.0">Download v1.0.0</a>
  &nbsp;·&nbsp;
  <a href="https://github.com/MRJOHN5ON/RideStats/releases">All releases</a>
</p>

---

## What it is

RideStats lets you **log roller coaster rides from your phone** — record a session, see your G-forces and ride timeline, save your history, and share a ride card when you want.

Everything stays **on your device**. No account, no cloud, no tracking.

The app ships with the **Six Flags Magic Mountain** coaster catalog. RideStats is an **independent fan app** and is not affiliated with any theme park.

---

## Downloads

RideStats is not on the Play Store. Sideload an APK from GitHub Releases.

| Version | APK | Notes |
|--------|-----|-------|
| **1.1.2** (latest) | [`RideStats-1.1.2.apk`](https://github.com/MRJOHN5ON/RideStats/releases/tag/v1.1.2) | Clearer force timeline labels — Up/down, Sides, Fwd/back |
| **1.1.1** | [`RideStats-1.1.1.apk`](https://github.com/MRJOHN5ON/RideStats/releases/tag/v1.1.1) | Airtime accuracy fix — peak duration, fewer false positives at rest |
| **1.1.0** | [`RideStats-1.1.0.apk`](https://github.com/MRJOHN5ON/RideStats/releases/tag/v1.1.0) | Directional G-forces, negative G, GPS speed, inversion count |
| **1.0.0** | [`RideStats-1.0.0.apk`](https://github.com/MRJOHN5ON/RideStats/releases/tag/v1.0.0) | Original release — peak G logging and ride history |

**Install steps**

1. Download **`RideStats-1.1.2.apk`** (latest) or an older version from the table above — release files are always named `RideStats-<version>.apk`
2. Open the file → **Install** (if blocked, allow installs from your browser or Files app in Android settings)
3. Before your first ride: **Settings → Pocket Recording Setup** — allow notifications and unrestricted battery

<p align="center">
  <img src="./media/screenshots/pocket-setup.jpg" alt="Pocket recording setup" width="300" />
</p>

On Samsung: **Settings → Security and privacy → Install unknown apps** for Chrome or My Files, and set RideStats battery to **Unrestricted**.

Demo build — no warranty. G-force and speed readings are phone-sensor estimates, not official park data. Use at your own risk.

---

## Release notes

### v1.1.2

**Clearer ride report**

- Force timeline toggle uses plain labels — **Up/down**, **Sides**, **Fwd/back** instead of Vert/Lat/Long
- Short description under the toggle explains what each view shows
- Peak badges read naturally — e.g. **Heaviest 4.2G**, **Strongest sway ±2.1G**
- Report stats renamed for clarity — **Lightest moment**, **Side sway peak**

> **Upgrading from 1.1.1?** No data reset — install over your existing app.

---

### v1.1.1

**Airtime fixes**

- **Peak airtime** is now the primary stat everywhere (report, share card, history badges) — e.g. **“2.4s airtime”** for the longest single stretch, not a moment count
- Fixed **vertical G sign** so a phone sitting still reads ~**+1G** instead of falsely triggering airtime/ejector labels
- **Stationary guard** — no airtime counted and sensation shows **“Normal”** when the phone isn’t moving
- Retuned airtime thresholds for more reliable detection during actual ride forces

> **Upgrading from 1.1.0?** G-force sign convention changed. Saved rides reset on first launch after install. Settings and the coaster catalog are kept.

---

### v1.1.0

**Sensor fusion & directional forces**

- Accelerometer + gyroscope fusion during recording — pocket your phone normally; rider frame calibrates automatically at the start of each ride
- **Vertical, lateral, and longitudinal G** with a timeline axis toggle on the ride report
- **Negative G** and airtime detection on the vertical axis (e.g. floater hills, ejector moments)
- **Inversion count** on the ride report (e.g. “4 inversions”)

**Speed**

- Optional **GPS peak speed** (toggle in Settings)
- **Speed timeline** on the ride report when location is enabled

**Everything else from v1.0** — catalog, history, share cards, ratings, local-only privacy

> **Upgrading from 1.0?** v1.1 uses a new ride data format. Your saved rides will reset on first launch after install. Settings and the coaster catalog are kept.

---

### v1.0.0

**First public release**

- Record rides in your pocket with foreground logging while the screen is locked
- Live **peak G** and ride duration during recording
- **Ride report** with peak, average, minimum G, airtime, and force timeline
- Compare recorded peak G against **catalog reference estimates**
- **History** grouped by coaster with personal records
- **Share cards** — Performance and Reaction variants
- Star ratings and ride notes
- **Six Flags Magic Mountain** coaster catalog (14 coasters)
- 100% **local storage** — no account, no cloud, no analytics

---

## Browse coasters

Pick a ride from the catalog, check the stats, and hit record.

<p align="center">
  <img src="./media/screenshots/home.jpg" alt="Coaster list" width="300" />
  <img src="./media/screenshots/coaster-detail.jpg" alt="Coaster detail" width="300" />
</p>

---

## Record in your pocket

Start a session, lock your phone, and ride. RideStats keeps logging in the background.

<p align="center">
  <img src="./media/screenshots/recording.jpg" alt="Active recording" width="300" />
</p>

---

## Ride report

After a ride you get peak G, stats, a force timeline, optional rating and notes, and a comparison against catalog reference estimates. Toggle **Up/down**, **Sides**, or **Fwd/back** on the timeline to see different forces on the ride.

<p align="center">
  <img src="./media/screenshots/ride-report1.jpg" alt="Ride report — peak and stats" width="300" />
  <img src="./media/screenshots/ride-report2.jpg" alt="Ride report — timeline and comparison" width="300" />
</p>

---

## History

Sessions are grouped by coaster. Personal records track your best peaks, airtime, ratings, and longest rides.

<p align="center">
  <img src="./media/screenshots/history.jpg" alt="Ride history" width="300" />
</p>

---

## Share a ride card

Export a **Performance** or **Reaction** card as an image and send it through your phone’s share menu.

<p align="center">
  <img src="./media/share-cards/performance-card.jpg" alt="Performance share card" width="280" />
  <img src="./media/share-cards/reaction-card.jpg" alt="Reaction share card" width="280" />
</p>

---

## Privacy

Your rides, ratings, and notes stay **on your phone**. RideStats does not upload your data or run a backend. Sharing only happens when you choose to. Clear everything anytime in Settings.

<p align="center">
  <img src="./media/screenshots/settings.jpg" alt="Settings and privacy" width="300" />
</p>

---

## About

I’m a **manual QA person**, not a software engineer. I vibecoded RideStats in about **half a day** with **AI-assisted development** (Cursor) — product direction, UI, copy, and testing on a real Android device.

Full Flutter app: recording, local storage, reports, history, share cards. Source is private; this page and the APKs are the public showcase.

---

<p align="center">
  <sub>Independent fan app · Not affiliated with Six Flags or any theme park</sub>
</p>
