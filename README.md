# nawra-data

Published prayer-time data for the Nawra app (Sri Lanka). The app downloads these files over GitHub Pages; the Nawra admin website publishes new versions here.

## Layout

```
manifest.json                 version, file list with sha256, rules (Sahr offset, high-rise adjustment, Ramadan override)
zones.json                    timetable zones and the districts in each
tt/<year>.json                yearly timetable per zone (minutes after midnight, Asia/Colombo)
wallpapers/catalog.json       wallpaper catalogue
wallpapers/<id>.jpg           wallpapers and thumbnails
history/<version>.json        change log entries
```

## Status

Placeholder only: `manifest.json` is empty (`files: []`) until the first real timetable is published from the admin website.

Do not edit files by hand. The app verifies every file against the sha256 in `manifest.json` and rejects mismatches.
