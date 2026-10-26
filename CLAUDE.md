# bird-2026: notes for Claude

Image repo for the photography site. Read [README.md](README.md) for the layout,
naming and rules; they apply to every change here.

- Only web copies: `large/` (up to 3840 px long edge, full crop size if smaller, never enlarged) and `thumb/` (800 px), WebP, same filename in both.
- Filenames: `id_bird-name_year_place.webp`, e.g.
  `20260503-001_american-robin_2026_central-park.webp` (user, 2026-10-25). Full rules in
  README "Naming". A wrong species or place is fixed in the site data, not by renaming.
- Never rename, overwrite, re-export or delete a published photo. Ask the user first if
  something seems to need it.
- Never add originals (CR3, TIFF, full-size JPEG exports).
- Photos are written by the site repo's `scripts/import_photos.py`
  (`../ronghao-zhang-gallery/`). That repo's `CLAUDE.md` ("Photo workflow") is the
  source of truth for the workflow; this repo only stores the files.
- Ask before pushing.
