# bird-2026

Web-sized 2026 bird photos, served with GitHub Pages for
the photography site at https://ronghao-zhang-gallery.github.io.

This repo holds image files only. Titles, species, places and camera settings live in
the site's data (repo `ronghao-zhang-gallery.github.io`); the filename repeats the species
and place so the files are readable on their own.

## Layout

```
bird-2026/
  large/20260503-001_american-robin_2026_central-park.webp   # up to 3840 px (4K) long edge, never enlarged; ~0.4–1.5 MB: full-screen view
  thumb/20260503-001_american-robin_2026_central-park.webp   # 800 px long edge, ~15–100 KB: cards and grids
```

Each photo has one file in `large/` and one with the same name in `thumb/`.

Photo URL: `https://ronghao-zhang-gallery.github.io/bird-2026/large/<name>.webp`

## Naming

`id_bird-name_year_place.webp` (user, 2026-10-25), e.g.
`20260503-001_american-robin_2026_central-park.webp`.

Underscores separate the four parts; hyphens join words inside a part.

- **id** = `YYYYMMDD-NNN`: the date the photo was taken (EXIF `DateTimeOriginal`) plus a
  3-digit counter that restarts at `001` each day, in the order the photos were taken.
  A photo added later gets the next free number for its date, even if it was taken
  earlier that day. The id alone is unique; the counter ignores species and place.
- **bird-name**: English common name, lowercase, words joined by hyphens, letters and
  digits only (`Cooper's Hawk` → `coopers-hawk`, `Black-crowned Night Heron` →
  `black-crowned-night-heron`). Unidentified: `unknown`. Several species in one photo:
  the main one in the name; all of them in the site data.
- **year**: 4-digit year taken (`2026`).
- **place**: short English place name, same style (`central-park`, `jamaica-bay`).
- Chinese names, full species lists and exact locations live in the site data, not the
  filename.

## Rules

- **No originals.** CR3 raws and full-size exports stay on local disk and backup.
- **Never rename, renumber, overwrite or re-export a published file.** The site links to
  these URLs, and git keeps every version forever, so a rewrite costs space for good.
- Files are added by the site's import script (`scripts/import_photos.py` in the site
  repo), not by hand.
- Only 2026 bird photos. Other years or subjects go in their own repos.

## Size budget

About 0.5–1.5 MB per photo (large + thumb), so roughly 1,000 photos before the 1 GB
GitHub Pages limit.
