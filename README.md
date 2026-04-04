# DronePoint — UAS Flight Log

A mobile-first progressive web app for UAS mission checklists and flight logging.

## Features
- Four-phase checklist (Pre-Mission / Launch Site / Pre-Flight / Final)
- Three-state items: done ✓, N/A ✕, or unchecked
- Flight record with auto-calculated elapsed time
- Mission history saved locally on device
- Unit converters (MPH→Knots, °F→°C, EST→UTC)
- Document links (FAA cert, insurance, manuals)
- Export missions as text reports
- Works offline after first visit

## Setup

1. Upload all files to this repo
2. Go to **Settings → Pages**, source: main branch / root
3. Your app will be live at `https://yourusername.github.io/dronepoint`

## Adding documents

Upload PDFs to the `/docs` folder. Then in the app go to:
**Tools → Documents → Add document link**

URL format:
```
https://yourusername.github.io/dronepoint/docs/your-file.pdf
```

## Files

```
dronepoint/
├── index.html       ← main app
├── sw.js            ← service worker (offline support)
└── docs/
    ├── placeholder.txt
    ├── faa-cert.pdf        (upload your own)
    ├── insurance.pdf       (upload your own)
    └── m3e-manual.pdf      (upload your own)
```
