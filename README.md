# Amélie Dark theme for ARGVUS

ARGVUS Dark theme, `amelie-dark`, with its Sticky and Float layouts.

## Theme identity

| Field | Value |
| --- | --- |
| Theme ID | `amelie-dark` |
| Display name | Amélie Dark |
| Mode | `dark` |
| Package | `argvus-theme-amelie-dark` |
| Wallpaper | `/usr/share/backgrounds/argvus/abstract/dark/amelie-dark-abstract-dark.jxl` |

The theme is `src/usr/share/argvus/themes/amelie-dark/theme.toml`: its name,
category, wallpaper and palette. Every component of the desktop renders its
files from that palette when the theme is applied, so the manifest and the
wallpaper are the whole package.

Amélie Dark pairs a plum background (`#382731`) with cream text (`#FFFCE5`)
and pink highlights (`#FAA2CA`). The original abstract wallpaper features pink
satin ribbons over a dark plum field and was generated with ImageGen.

## Working on the theme

```sh
make check     # render every component in both layouts and report errors
make try       # install it as your own theme, then: argvus theme apply amelie-dark
make untry     # remove that copy
make validate  # repository and packaging checks
make build     # build the package into build/dist/
make install   # install the package (sudo pacman -U)
```

Git installation reads the theme files from `src/`; `packaging/` is optional and only used to build Arch Linux packages. Publish this repository with its wallpaper. Users can install it with
`argvus theme install https://HOST/USER/argvus-theme-amelie-dark.git`,
apply it with `argvus theme apply amelie-dark`, and remove it with
`argvus theme uninstall amelie-dark`. Installed themes appear in Custom themes.

See [DEVELOPMENT.md](DEVELOPMENT.md) for the build and release details.

## License

GPL-3.0-only. See [LICENSE](LICENSE).
