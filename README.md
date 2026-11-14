# Vitals — Health Tracker

A private, minimal web app for tracking blood pressure, heart rate and a medication schedule, with optional add-ons and your own custom data sets. It's a single `index.html` file with no dependencies, build step or server.

## Features

- **Blood pressure & heart rate.** Log readings with a time and a note. Each reading gets an ACC/AHA category (Normal, Elevated, Stage 1, Stage 2, Crisis).
- **Medication schedule.** Add each medication with its dose and daily times to get a checklist on the Today page. Medications with no times count as "as needed". Missed doses are flagged as overdue, and adherence is tracked.
- **Optional add-ons (Settings):**
  - Water intake: quick-add buttons, a daily goal, and ml or oz
  - Exercise: a list of activities you can add, edit and remove, with minutes and intensity
  - Preset data sets: weight, sleep, blood glucose, blood oxygen and temperature
  - **Custom data sets:** any name and unit, summarized each day as an average, a total, or the last value
- **Trends page.** Charts and stats for 7 days, 30 days, 90 days, 1 year or all time, plus an editable history table.
- **Doctor report.** A one-page summary you can **save as PDF / print**, or **save as a PNG image** (on phones this opens the share sheet).
- **Your data.** Export a JSON backup, import it on another device, and export a CSV for spreadsheets.
- Light, dark and auto themes, and a mobile layout with a bottom tab bar.

## Files

```
index.html          the app
manifest.json       app name, colors and icons for home-screen installs
icons/              app icon in every size (iPhone, Android, browser tab)
README.md           this file
```

## Publish on GitHub Pages

1. Create a new repository on GitHub, for example `vitals`.
2. Click **Add file → Upload files** and drag in `index.html`, `manifest.json`, `README.md` **and the whole `icons` folder** (drag the folder itself so it keeps its name), then click **Commit changes**.
3. Go to **Settings → Pages → Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, and click Save.
4. After a minute or so the app is live at `https://<your-username>.github.io/vitals/`.

On a phone, open that link and use **Add to Home Screen**. It gets the Vitals icon and opens full-screen like a regular app. If you added it to your home screen before the icon existed, delete the old shortcut and add it again to pick up the new icon.

## Privacy

All data is stored in your browser's `localStorage` and never leaves your device. Your data is not uploaded to GitHub. Each browser or device keeps its own copy, so use **Export backup** to move data between devices or keep a safe copy. Clearing your browser's site data will erase your entries.

## Disclaimer

Vitals is a personal log, not a medical device, and it does not give medical advice. Talk with your clinician about your readings and medications.
