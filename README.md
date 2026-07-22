# highpapers

curated wallpaper gallery — [jahbas.github.io/walls](https://jahbas.github.io/walls)

## how releases work

| release | purpose |
|---------|---------|
| `0.0.1` | base collection — all current wallpapers |
| `0.0.2` | next time you add wallpapers, upload only the new ones here |
| `0.0.3` | and so on |

each wallpaper in `wallpapers.json` has its own URL pointing to the release it was uploaded to. this means you never re-upload a wallpaper that was already in a previous release. just add new files to the next release tag and append entries to `wallpapers.json`.

### adding new wallpapers

1. drop images into `~/Downloads/highpapers/{anime-name}/` with format `{slug}-{nn}.{ext}`
2. create a new release: `gh release create 0.0.2 --repo Jahbas/walls`
3. upload only new files: `gh release upload 0.0.2 --repo Jahbas/walls `path/to/new/file.jpg`
4. add entries to `wallpapers.json` using `https://github.com/Jahbas/walls/releases/download/0.0.2/new-file.jpg`
