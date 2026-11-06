# filmai-viewer-media

Public media mirror for the [filmai-viewer](https://github.com/landogayatri/filmai-viewer)
offline catalog. The self-contained `catalog.html` SPA references every backed-up
image/video here via `raw.githubusercontent.com`, so it needs **no local files** —
it works from any host (or `file://`) as long as this repo is reachable.

## Layout

| Path | Contents |
|---|---|
| `assets/<user_ns>/<id>.{png,jpg,webp}` | still images (project assets, casting portraits) |
| `videos/<user_ns>/<id>.mp4` + `.thumb.jpg` | videos + thumbnails |
| `byteplus/asset-<id>.<ext>` | 6,763 casting stock-performer thumbnails |

Source: a personal offline study backup of publicly viewable filmai.ai learning
materials (demo templates, showcase, studio examples) plus the public BytePlus
stock-performer catalog. Rebuilt by the toolchain in the viewer repo
(`repo/scripts/` + `repo/build/`); restore scripts in `scripts/`.

All files are plain git blobs (largest ≈ 96 MiB, under GitHub's 100 MiB cap).
