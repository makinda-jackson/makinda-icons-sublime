# Makinda Icons — Sublime Text

File-type icons for Sublime Text 3 / 4. Warm, legible glyphs that match the
Makinda design system.

## Install via Package Control

1. Open the command palette: <kbd>Cmd</kbd>/<kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd>
2. Run **Package Control: Install Package**
3. Choose **Makinda Icons**
4. Restart Sublime Text

Icons are bound to TextMate scopes (e.g. `source.js`, `source.python`) via
`.tmPreferences` files and apply automatically to matching files in the
sidebar and tabs.

## Manual install

Drop this repository's contents into a folder named `Makinda Icons` inside
your Sublime Text **Packages** directory:

- macOS: `~/Library/Application Support/Sublime Text/Packages/Makinda Icons/`
- Linux: `~/.config/sublime-text/Packages/Makinda Icons/`
- Windows: `%APPDATA%\Sublime Text\Packages\Makinda Icons\`

Then restart Sublime.

## Layout

- `icons/<name>.png` / `<name>@2x.png` / `<name>@3x.png` — 16 / 32 / 48 px
  raster variants. Sublime picks the right size for the current display scale.
- `preferences/<name>.tmPreferences` — binds a TextMate scope to the icon at
  `Packages/Makinda Icons/icons/<name>`.

## Limitations

- Bindings are scope-driven. Files whose language has no matching
  `.tmPreferences` entry won't get an icon.
- Single dark-fill rasterization. Sublime can't auto-swap icon color by theme,
  so a separate package would be needed for a light-fill variant.

## License

MIT — see [LICENSE.md](LICENSE.md).
