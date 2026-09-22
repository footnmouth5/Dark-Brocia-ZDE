# Dark-Brocia-ZDE

Dark Broica CDE theme for Zen Browser. Vertical tabs  compact mode  userChrome.css.

## Preview

![screenshot](screenshot.png)

## Files

| File |  |
|---|---|
| [`userChrome.css`](userChrome.css) | Main theme. Full CDE styling with the stamped-border chrome, per-region palettes, and compact-mode handling. |
| [`flatbase_userChrome.css`](flatbase_userChrome.css) | Flat alternative. Same palette and layout, but strips the raised/inverted border treatment on toolbars and buttons. One palette. |
| [`CDE-Brocia-Dark-stylus-2026-09-22.json`](CDE-Brocia-Dark-stylus-2026-09-22.json) | Web-content companion for the [Stylus extension](https://addons.mozilla.org/en-US/firefox/addon/styl-us/). Restyles website CSS (backgrounds, text, links, code blocks) to match the browser chrome. Import via Stylus → Manage → Import. Updates may be pushed here first: https://userstyles.world/style/30305|

You only need `userChrome.css` to get the browser chrome theme. The other two are optional add-ons depending on how deep you want to go.

## Palette

| Color | Hex | Use |
|---|---|---|
| Putty | `#c6b2a8` | URL bar, text |
| Muted | `#999999` | Secondary text |
| Slate | `#8998aa` | Sidebar |
| Slate-dark | `#686f82` | Titlebar, nav bar |
| Orange | `#eda870` | Hover, accents, active tab stripe |
| Teal | `#4992a7` | Active tab, focus |
| Rose | `#b7878d` | App menu |
| Steel | `#93abbf` | Idle tabs |

Extended darks: `#1e222a`, `#2a2e38`, `#3a4050`, `#4a5160`, `#6a7285`

## Install

### Browser theme (`userChrome.css`)

1. In Zen, go to `about:support` and click **Open Profile Folder**.
2. Create a folder named `chrome` if it doesn't exist.
3. Copy `userChrome.css` into that `chrome` folder.
4. In `about:config`, set `toolkit.legacyUserProfileCustomizations.stylesheets` to `true`.
5. Restart Zen.

### Web content (`Stylus` userstyle)

1. Install the [Stylus extension](https://addons.mozilla.org/en-US/firefox/addon/styl-us/) if you don't have it.
2. Open Stylus → **Manage** → **Import**.
3. Select the `.json` file from this repo.
4. Enable the style. It applies globally to all HTTP/HTTPS pages.

You can also install the userstyle directly from [userstyles.world](https://userstyles.world/style/30305).

## Notes

- Built and tested on Zen Browser. Not compatible with stock Firefox.
- Designed for compact mode with vertical tabs.
- If you have the **Smaller Compact Mode** Zen Mod installed, disable it before using this theme. The theme handles compact-mode spacing itself, and the mod will fight it.
- The two `userChrome.css` variants are mutually exclusive. Only one should be in your `chrome` folder at a time. Rename the other to something like `userChrome.css.bak` to keep it around without loading it.
- `toolkit.legacyUserProfileCustomizations.stylesheets` is the only `about:config` preference required to load the theme. If you want to edit the CSS live without restarting, also enable `devtools.debugger.remote-enabled` and `devtools.chrome.enabled` to unlock Zen's Browser Toolbox and Style Editor. Recent Zen versions may load `userChrome.css` regardless of the legacy preference, so if it keeps working after you toggle it off, that's expected.

## Credits

- **DeepSeek-v4-flash**  

## License

MIT
