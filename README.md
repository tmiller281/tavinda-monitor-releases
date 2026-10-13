# Tavinda Monitor — download and install

Tavinda Monitor watches the temperature of your fridges and freezers all day and night. It keeps the HACCP
temperature log for you, and sends an alert by email, WhatsApp or Telegram when a unit stays too warm or too cold.
It runs on a Windows PC in your restaurant and reads wireless temperature sensors (Shelly Pill with probes).

This page only holds the installer and its updates. The program itself is not open source.

**Pilot software.** Tavinda Monitor is still being tested in a real restaurant. It works, but expect changes, and
keep your own checks going while you try it.

## Download

**[Download the latest version](https://github.com/tmiller281/tavinda-monitor-releases/releases/latest)** — on that
page, click the file named `TavindaMonitor-Setup-<version>.exe` under **Assets**.

## What you need

- A Windows 10 or 11 PC that stays on (for example the till or office PC), and a Windows login that may install
  programs (an administrator).
- To measure temperatures: a **Shelly Pill** and **DS18B20 probes**, one per
  fridge or freezer, on the same Wi-Fi as the PC. The app finds the Pill and its probes for you.
- **No Pill yet?** You can still install it and look around: the screens, settings, alerts set-up and the HACCP log
  all open. There are simply no temperatures to show, and the app tells you it can't find a Pill.

## Install

1. Double-click `TavindaMonitor-Setup-<version>.exe`.
2. If a blue box says **Windows protected your PC**: this is expected, because the installer isn't code-signed yet.
   Click **More info**, then **Run anyway**.
3. Windows asks **Do you want to allow this app to make changes to your device?** Click **Yes**.
4. Click **Install**, then **Finish**. The app opens by itself.

You now have a **Tavinda Monitor** icon on the desktop and in the Start menu, and a small shield next to the clock
(Windows may hide it under the **^** arrow). Monitoring runs in the background, even when the window is closed or
nobody is logged in, and starts again by itself after the PC restarts.

## First steps

1. **Choose an admin password** when the app asks. You need it to change things; looking is free.
2. **Add your Pill**: press **＋ Add a Pill** and follow the steps. The app sets up the Pill's Wi-Fi for you over Bluetooth, so the PC needs Bluetooth.
3. **Name each probe**: tell the app which fridge or freezer each probe is in, and its safe range
   (for example a freezer at −18 °C or colder).
4. **Set up alerts** on the **Alerts** page: who gets them, and by which channel.
5. **Check the HACCP log** on the **HACCP** page: readings are filled in at your log times (you choose them in
   **Settings**). A missed reading is shown as "no reading" — the app never makes one up.

## The tray shield

| What you see | What it means |
|---|---|
| Green dot | All fine |
| Red dot | A unit has been out of range long enough to raise an alert |
| Grey dot | Needs a look: a unit has just gone out of range, a Pill or probe isn't reporting, or logs aren't being sent |
| Faded shield | Tavinda Monitor isn't running — right-click the shield and choose **Start monitoring** |

Right-click the shield for **Start**, **Restart** and **Stop monitoring** (stopping asks an administrator first).

## Updates

The app checks this page for a new version and installs it by itself at night (03:00 by default), staying clear of
your log times. You can also go to **Settings → Updates** and press **Check now**, then **Install now**.
Monitoring pauses for about a minute while an update installs. If an update ever fails, the app says why and puts
the previous version back.

## If something's wrong

- **Settings → Logs** shows what the app and the updater have been doing (passwords are never shown).
  The same warnings also appear in Windows **Event Viewer → Windows Logs → Application**, source "Tavinda Monitor".
- **A page says "Tavinda Monitor isn't running"**: click **Start it**, or restart the PC.
- **Reinstalling** (running the installer again) keeps all your data.

## Uninstall

Windows **Settings → Apps → Installed apps → Tavinda Monitor → Uninstall**. The uninstaller suggests a backup
first, then asks whether to delete your records. Choose **No** to keep them: they stay in
`C:\ProgramData\Tavinda Monitor`, and a later install picks up where you left off.

## Suggestions and problems

We'd love to hear what you think. Send your ideas, questions or problems to the person who gave you this link —
a screenshot and the time it happened help a lot.
