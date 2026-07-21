# walls

drop wallpapers here. add their urls to `wallpapers.json`.

## adding wallpapers

each entry in `wallpapers.json`:

```json
{
  "name": "your-wallpaper-name",
  "url": "https://path-to-your-image.jpg",
  "resolution": "2560x1440"
}
```

### hosting with github releases (unlimited storage)

1. go to the repo's [Releases](https://github.com/Jahbas/walls/releases) page
2. create a new release, attach your wallpaper files
3. use the release asset url in `wallpapers.json`:
   `https://github.com/Jahbas/walls/releases/download/v1.0/your-wallpaper.png`

release assets don't count toward repo storage limits and support files up to 2gb each.

### hosting in repo

drop images into `/wallpapers/` and use relative paths:

```json
{ "name": "my wall", "url": "wallpapers/my-wall.png" }
```

repo limit is 1gb total.

## editing

edit `wallpapers.json` directly on github or clone the repo, add your changes, and push.
the site updates automatically.
