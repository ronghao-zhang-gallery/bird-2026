# bird-2026

Web-sized 2026 bird photos, served with GitHub Pages for
the photography site at https://ronghao-zhang-gallery.github.io.

This repo holds image files only. Titles, species, places and camera settings live in
the site's data (repo `ronghao-zhang-gallery.github.io`), not here.

## Layout

```
bird-2026/
  large/2026-05-03_001.webp   # 2560 px long edge, ~70–700 KB: full-screen view
  thumb/2026-05-03_001.webp   # 800 px long edge, ~15–100 KB: cards and grids
```

Each photo has one file in `large/` and one with the same name in `thumb/`.

Photo URL: `https://ronghao-zhang-gallery.github.io/bird-2026/large/<name>.webp`

## Naming

`YYYY-MM-DD_NNN.webp`, e.g. `2026-05-03_001.webp`, `2026-05-03_002.webp`.

- `YYYY-MM-DD` is the date the photo was taken (EXIF `DateTimeOriginal`).
- `NNN` is a counter that restarts at `001` each day, in the order the photos were taken.
- A photo added later gets the next free number for its date, even if it was taken
  earlier that day.

## Rules

- **No originals.** CR3 raws and full-size exports stay on local disk and backup.
- **Never rename, renumber, overwrite or re-export a published file.** The site links to
  these URLs, and git keeps every version forever, so a rewrite costs space for good.
- Files are added by the site's import script (`scripts/import_photos.py` in the site
  repo), not by hand.
- Only 2026 bird photos. Other years or subjects go in their own repos.

## Size budget

About 0.5 MB per photo (large + thumb), so roughly 2,000 photos before the 1 GB
GitHub Pages limit.
