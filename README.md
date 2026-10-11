# FitTrack PWA

A small, responsive, installable fitness tracker. No account or backend required.

## Features
- Daily logs for weight, sleep, resting heart rate, energy, soreness, digestion, training, run distance/pace/heart rate, steps, protein, water and notes.
- Editable daily habit checklist and personal goals.
- Dashboard with 7-day weight average, activity minutes, sleep, habit completion and weekly activity bars.
- Trend charts, recent entries, CSV export and JSON backup/import.
- Local browser storage and an offline app shell via service worker.
- Mobile-friendly layout.

## Run locally
A service worker requires localhost or HTTPS. From this folder run:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Publish as a PWA
Deploy the contents of this folder to any static host that serves HTTPS, such as GitHub Pages, Netlify or Cloudflare Pages. Open the deployed URL on your phone and use the browser's **Add to Home Screen / Install app** option.

For iPhone: open the HTTPS site in Safari → Share → Add to Home Screen. The browser may not show the in-page Install button on iOS.

## Data and privacy
Entries are saved in localStorage on the current browser profile and device. There is no cloud sync. Use **Backup JSON** or **Export CSV** regularly. Clearing site data or changing browsers/devices may remove or hide your entries. Avoid entering sensitive information on a shared device.

## Notes
- Starter defaults (75 kg, 130 g protein, 150 aerobic minutes/week, 7,000 steps/day) are editable and should be personalized.
- Charts are lightweight canvas charts with no charting dependency.
- The app uses no remote API. The stylesheet references Google Fonts for typography; the app's core features work without them.
