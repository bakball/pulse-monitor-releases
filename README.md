<p align="center"><img src="assets/icon.png" width="84" alt="Pulse Monitor icon"></p>

<h1 align="center">Pulse Monitor</h1>

<p align="center"><b>Turn an Android phone or tablet into a live hardware dashboard and remote for your PC (Windows or macOS), over your own Wi-Fi.</b><br>
CPU, GPU, memory, storage, network, fans, voltages and power, every half second. Control processes, media and shortcuts from the couch. No cloud, no account.</p>

<p align="center">
  <a href="https://github.com/bakball/pulse-monitor-releases/releases/latest"><img src="https://img.shields.io/badge/Download-PC%20Server-10B981?style=for-the-badge&logo=windows&logoColor=white" alt="Download the PC server"></a>
  <a href="https://play.google.com/store/apps/details?id=com.pulsemonitor"><img src="https://img.shields.io/badge/Get%20it%20on-Google%20Play-06B6D4?style=for-the-badge&logo=googleplay&logoColor=white" alt="Get it on Google Play"></a>
</p>

<p align="center">
  <a href="https://github.com/bakball/pulse-monitor-releases/releases/latest"><img src="https://img.shields.io/github/v/release/bakball/pulse-monitor-releases?label=release&color=10B981" alt="latest release"></a>
  <img src="https://img.shields.io/badge/PC-Windows%2010%2F11%20%C2%B7%20macOS-475569" alt="Windows 10/11 and macOS">
  <img src="https://img.shields.io/badge/Android-8.0%2B-3ddc84" alt="Android 8.0+">
  <img src="https://img.shields.io/badge/theme-Dark%20OLED%20%C2%B7%20Light-0F172A" alt="Dark OLED and Light themes">
</p>

<p align="center"><img src="assets/hero.png" width="900" alt="Pulse Monitor on two phones and two tablets, in dark and light themes, showing a Ryzen 5 5600 and Radeon RX 6700 XT system"></p>

Pulse Monitor has two parts: a small **PC server** that reads your hardware sensors, and an **Android app** that shows them.
They find each other on your local network, or talk over a USB cable, and nothing ever leaves your home.

- **Live dashboard**: CPU, GPU, memory, storage and network in a Bento grid with radial gauges and 60-second sparklines. Thermal colours turn amber at 60 °C and red at 80 °C.
- **Desk OSD**: rotate a tablet or phone to landscape for a full-screen, four-column, no-scroll dashboard that keeps the screen on. Made to sit under your monitor.
- **Processes**: the whole process list grouped by app, with search, sorting and a guarded **End** / **End all** (protected system processes can never be ended).
- **Deck**: Now Playing with transport controls and volume, plus one-tap PC shortcuts (lock, display off, mute, task manager, terminal, screenshot) and an overview of your Claude Code / Codex sessions.
- **Control without pairing**: while *Allow phone control over Wi-Fi* is on, any phone on your private network can use the Deck and Processes tabs straight away. No token to copy.
- **Dark (OLED) and Light themes**: follow the system or pick one; it switches instantly, on every screen.
- **Honest data**: if a sensor cannot be read on your hardware, Pulse Monitor shows `--`. It never estimates or invents temperatures, clocks or wattage.

**Contents**: [Screenshots](#screenshots) · [Install](#install) · [Phone control](#phone-control-over-wi-fi) · [Themes](#themes) · [Free and PRO](#free-and-pro) · [How it works](#how-it-works) · [Troubleshooting](#troubleshooting) · [Privacy](#privacy) · [Credits](#credits)

## Screenshots

Real captures from a Ryzen 5 5600 + Radeon RX 6700 XT desktop, taken on a phone and a tablet.

### Phone

<table>
  <tr>
    <th width="25%">Metrics</th><th width="25%">Sensors &amp; storage</th><th width="25%">Processes</th><th width="25%">Deck</th>
  </tr>
  <tr>
    <td><img src="assets/screenshots/phone-dark-metrics.png" alt="Phone, dark: CPU, GPU and memory"></td>
    <td><img src="assets/screenshots/phone-dark-metrics3.png" alt="Phone, dark: storage, system sensors and top processes"></td>
    <td><img src="assets/screenshots/phone-dark-processes.png" alt="Phone, dark: process list with End buttons"></td>
    <td><img src="assets/screenshots/phone-dark-deck.png" alt="Phone, dark: now playing and PC shortcuts"></td>
  </tr>
  <tr>
    <td><img src="assets/screenshots/phone-light-metrics.png" alt="Phone, light: CPU, GPU and memory"></td>
    <td><img src="assets/screenshots/phone-light-metrics3.png" alt="Phone, light: storage, system sensors and top processes"></td>
    <td><img src="assets/screenshots/phone-light-processes.png" alt="Phone, light: process list with End buttons"></td>
    <td><img src="assets/screenshots/phone-light-deck.png" alt="Phone, light: now playing and PC shortcuts"></td>
  </tr>
</table>

### Phone, landscape (desk OSD)

Turn the phone sideways and it becomes a full-screen, no-scroll dashboard that keeps the screen on.

<p align="center">
  <img src="assets/screenshots/phone-land-dark-metrics.png" width="49%" alt="Phone landscape OSD, dark">
  <img src="assets/screenshots/phone-land-light-metrics.png" width="49%" alt="Phone landscape OSD, light">
</p>
<p align="center">
  <img src="assets/screenshots/phone-land-dark-processes.png" width="49%" alt="Phone landscape processes, dark">
  <img src="assets/screenshots/phone-land-light-processes.png" width="49%" alt="Phone landscape processes, light">
</p>
<p align="center">
  <img src="assets/screenshots/phone-land-dark-deck.png" width="49%" alt="Phone landscape deck, dark">
  <img src="assets/screenshots/phone-land-light-deck.png" width="49%" alt="Phone landscape deck, light">
</p>

### Tablet (desk OSD)

<p align="center">
  <img src="assets/screenshots/tablet-dark-metrics.png" width="49%" alt="Tablet OSD, dark">
  <img src="assets/screenshots/tablet-light-metrics.png" width="49%" alt="Tablet OSD, light">
</p>
<p align="center">
  <img src="assets/screenshots/tablet-dark-processes.png" width="49%" alt="Tablet processes, dark">
  <img src="assets/screenshots/tablet-light-processes.png" width="49%" alt="Tablet processes, light">
</p>
<p align="center">
  <img src="assets/screenshots/tablet-dark-deck.png" width="49%" alt="Tablet deck, dark">
  <img src="assets/screenshots/tablet-light-deck.png" width="49%" alt="Tablet deck, light">
</p>

## Install

**Requirements:** Windows 10 or 11 (64-bit) or macOS, a phone or tablet with Android 8.0+, and both on the same network (or connected by USB).

### Windows

1. Download **`PulseMonitor-Setup-*.exe`** from the **[latest release](https://github.com/bakball/pulse-monitor-releases/releases/latest)**.
2. Run it and accept the administrator prompt. Sensor access needs administrator rights.
3. Leave the options you want ticked:
   - *Start Pulse Monitor automatically when I sign in*: runs hidden in the tray, no console window.
   - *Install the PawnIO driver*: lets the server read **CPU temperature, power and voltage** on many processors. Skipped if PawnIO is already installed.
4. Finish the setup. A pulse icon appears in the system tray.
5. Install the **[Android app](https://play.google.com/store/apps/details?id=com.pulsemonitor)**, tap your PC in the **Nearby PCs** list, and you are live.

### macOS

Download `PulseMonitor-macOS.zip` from the [latest release](https://github.com/bakball/pulse-monitor-releases/releases/latest) and run the server from the extracted folder. Available sensors depend on your Mac.

### Over USB

Install Android's `adb` (platform-tools) on the PC, turn on USB debugging on the phone and plug it in. The server sets up an `adb reverse` tunnel every few seconds, and the app connects on its own (a **USB** badge shows in the top bar). Control commands over USB are always allowed.

## Phone control over Wi-Fi

The **Processes** and **Deck** tabs can end processes, run shortcuts and control media. Over the network this needs only that the phone is on a **private network** (`192.168.x.x`, `10.x.x.x`, `172.16-31.x.x`) and that **Allow phone control over Wi-Fi** is ticked in the tray menu (it is on by default). There is no token to copy and no pairing dialog.

> Anyone on your private network can then control the PC from a phone with the app. On a network you do not trust, untick *Allow phone control over Wi-Fi* in the tray menu, or set `"allow_lan_control": false` in `control.json`. Public addresses are never allowed, whatever the setting. Telemetry itself is read-only either way.

The pairing token (`pulse-daemon --print-token`, or *Copy Wi-Fi pairing token* in the tray) is still accepted, so older app versions keep working.

## Themes

Pick **System (Auto)**, **Dark (OLED)** or **Light** from the sun / moon icon in the top bar, or in **Settings**. The choice is remembered and applies instantly to the dashboard, Processes, Deck, Connect screen and every dialog, with no restart. Accent colours are tuned per theme so gauges and temperatures stay readable on both.

## Free and PRO

| | Free | PRO |
|---|:---:|:---:|
| Live dashboard (CPU, GPU, memory, storage, network, ping and packet loss) | ✓ | ✓ |
| Automatic discovery, USB link, Dark and Light themes | ✓ | ✓ |
| Now Playing with volume, AI sessions | ✓ | ✓ |
| Processes: top rows by CPU | ✓ | ✓ |
| Full process list, search, sorting, End / End all | | ✓ |
| PC shortcuts | | ✓ |
| Detail sheets, per-core view, full system sensors | | ✓ |
| Landscape desk OSD | | ✓ |
| Thermal alarms, °C / °F | | ✓ |

## How it works

```
 PC server (Rust)                              Android app (Kotlin, Compose)
 ┌────────────────────────┐   WebSocket 8765   ┌────────────────────────────┐
 │ sensors → JSON frame   │ ────────────────▶  │ live gauges & sparklines   │
 │ every 500 ms           │                    │                            │
 │ control commands       │ ◀────────────────  │ processes, media, shortcuts │
 │ UDP discovery 45454    │ ◀─ PULSE_DISCOVER  │ finds your PC automatically│
 └────────────────────────┘                    └────────────────────────────┘
```

- The server samples hardware on its own background thread, so frames go out on time without blocking.
- Telemetry is pushed over a WebSocket on **TCP 8765**. Discovery uses **UDP 45454**.
- Everything stays on your local network. There are no servers, accounts or analytics.

## Troubleshooting

**The app can't find my PC.**
Both devices must be on the same network. Allow the server through the firewall: it uses **TCP 8765** (telemetry) and **UDP 45454** (discovery). You can also type the PC's IP address in the app. Guest and "client isolation" Wi-Fi networks block device-to-device traffic.

**CPU temperature or power shows `--`.**
That sensor isn't available without the PawnIO driver on most CPUs. Re-run the setup and tick *Install the PawnIO driver*, then restart Pulse Monitor. Some processors don't expose a power sensor at all; in that case `--` is the correct answer.

**I play games with an anti-cheat (FACEIT, Vanguard, Easy Anti-Cheat, BattlEye).**
While one of them is running, Pulse Monitor stops using the kernel driver and falls back to user-mode sensors only, so CPU temperature and power may show `--` during the game.

**Collecting diagnostics for a bug report.**
Run, from an administrator PowerShell:

```powershell
Start-Process -Wait -FilePath "C:\Program Files\PulseMonitor\pulse-daemon.exe" -ArgumentList '--once','--out','C:\pulse-frame.json'
```

This writes the telemetry frame, the raw sensor tree and the sensor-engine state next to `C:\pulse-frame.json`. Open an [issue](https://github.com/bakball/pulse-monitor-releases/issues) and attach them.

## Privacy

Telemetry is sent only between your PC and your own device over your local network. Pulse Monitor does not collect, store or upload personal data or hardware readings to any server. The Android app uses the network permission for local connections and Google Play Billing for the optional PRO subscription.

## Credits

Hardware sensor access is powered by [LibreHardwareMonitor](https://github.com/LibreHardwareMonitor/LibreHardwareMonitor) (MPL-2.0). The optional CPU driver is [PawnIO](https://pawnio.eu/) by namazso.

---

<p align="center">Made by <b>ForgeBit Labs</b></p>
