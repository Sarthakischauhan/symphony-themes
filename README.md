# Symphony Themes

A marketplace of native, data-only color themes for the [Symphony coding agent](https://github.com/Sarthakischauhan/symphony). Theme plugins contain no skills, tools, or executable addon code.

## Install

Use a Symphony build with support for theme plugins.

```sh
# Register the catalog once; this does not install a theme family.
symphony plugins marketplace add Sarthakischauhan/symphony-themes

# Install only the families you want (each includes its variants).
symphony plugins add gruvbox@symphony-themes
symphony plugins add monokai@symphony-themes
symphony plugins add github@symphony-themes
symphony plugins add anysphere@symphony-themes
symphony plugins add zed@symphony-themes
symphony plugins add hasakura@symphony-themes
symphony plugins add bubblegum@symphony-themes
symphony plugins add cpp@symphony-themes
symphony plugins add sakura@symphony-themes
symphony themes list
symphony
```

Inside Symphony, open `/theme` to preview and select a theme, or use `/theme gruvbox:Gruvbox Dark` directly. Restart a running session after installing a family.

The marketplace registration copies its catalog repository into Symphony's cache; it does not make any family available in `/theme` until you install that family. Installing a family copies its theme TOMLs and makes all its variants available; selecting a variant does not download anything further.

```sh
symphony plugins marketplace update symphony-themes
symphony plugins update gruvbox
symphony plugins remove gruvbox
```

If you installed the old single `symphony-themes` plugin, remove it with `symphony plugins remove symphony-themes`, then use the marketplace commands above. An existing `$SYMPHONY_HOME/theme.toml` (or `~/.symphony/theme.toml`) overrides the chosen theme and is never overwritten.

## Theme families

| Plugin | Variants | Palette inspiration |
| --- | --- | --- |
| `gruvbox` | Gruvbox Dark, Gruvbox Light | [Gruvbox](https://github.com/morhetz/gruvbox) |
| `monokai` | Monokai | [Monokai](https://monokai.nl/) |
| `github` | GitHub Dark | [GitHub color themes](https://github.com/primer/github-vscode-theme) |
| `kanagawa` | Kanagawa Wave | [Kanagawa](https://github.com/rebelot/kanagawa.nvim) |
| `one-dark` | One Dark | [Atom One Dark](https://github.com/atom/one-dark-syntax) |
| `symphony` | Symphony Dusk, Symphony Daylight | Original Symphony palettes |
| `anysphere` | Anysphere Dark, Anysphere Light | Minimal Anysphere/Cursor-inspired neutrals |
| `zed` | Zed Dark, Zed Light | Zed editor-inspired palettes |
| `rose-pine` | Rosé Pine Moon | [Rosé Pine](https://rosepinetheme.com/) |
| `catppuccin` | Catppuccin Mocha | [Catppuccin](https://catppuccin.com/) |
| `tokyo-night` | Tokyo Night Storm | [Tokyo Night](https://github.com/enkia/tokyo-night-vscode-theme) |
| `nord` | Nord Polar | [Nord](https://www.nordtheme.com/) |
| `oxocarbon` | Oxocarbon Dark, Oxocarbon Light | High-contrast monochrome and crisp blue accents inspired by IBM Carbon. |
| `everforest` | Everforest Dark, Everforest Light | Soft forest greens, warmer neutrals, and low-glare surfaces. |
| `solarized` | Solarized Dark, Solarized Light | Classic Solarized hue relationships adapted for Symphony. |
| `ayu` | Ayu Mirage, Ayu Light | Warm amber accents with a polished, modern editor surface. |
| `flexoki` | Flexoki Dark, Flexoki Light | Ink-and-paper inspired palettes with subtle warm accents. |
| `hasakura` | haSakura-theme | [haSakura-theme](https://marketplace.visualstudio.com/items?itemName=HashiramaNaiff.haSakura-theme) |
| `bubblegum` | bubblegum | [bubblegum](https://vscodethemes.com/e/connieth.bubblegum/bubblegum) |
| `cpp` | C/C++ Dark, C/C++ Light, C/C++ 2017 Dark, C/C++ 2017 Light | [Visual Studio C/C++ Themes](https://github.com/microsoft/vscode-cpptools/tree/main/Themes/themes) |
| `sakura` | Sakura | [Ghostty Sakura](https://github.com/mbadolato/iTerm2-Color-Schemes/blob/master/ghostty/Sakura) |

These are Symphony-native adaptations, not pixel-perfect ports of another application. The existing PNG screenshots below are captured from the Symphony TUI with representative transcript and code content. **New SVG previews are illustrative palette mockups, not live TUI captures.**

<details>
<summary>Gruvbox Dark</summary>

![Gruvbox Dark](screenshots/gruvbox-dark.png)
</details>

<details>
<summary>Gruvbox Light</summary>

![Gruvbox Light](screenshots/gruvbox-light.png)
</details>

<details>
<summary>Monokai</summary>

![Monokai](screenshots/monokai.png)
</details>

<details>
<summary>GitHub Dark</summary>

![GitHub Dark](screenshots/github-dark.png)
</details>

<details>
<summary>Kanagawa Wave</summary>

![Kanagawa Wave](screenshots/kanagawa-wave.png)
</details>

<details>
<summary>One Dark</summary>

![One Dark](screenshots/one-dark.png)
</details>

<details>
<summary>Symphony Dusk</summary>

![Symphony Dusk](screenshots/symphony-dusk.png)
</details>

<details>
<summary>Symphony Daylight</summary>

![Symphony Daylight](screenshots/symphony-daylight.png)
</details>

## New theme previews

<details>
<summary>Anysphere Dark (illustrative palette preview)</summary>

![Anysphere Dark palette preview](screenshots/anysphere-dark.svg)
</details>

<details>
<summary>Anysphere Light (illustrative palette preview)</summary>

![Anysphere Light palette preview](screenshots/anysphere-light.svg)
</details>

<details>
<summary>Zed Dark (illustrative palette preview)</summary>

![Zed Dark palette preview](screenshots/zed-dark.svg)
</details>

<details>
<summary>Zed Light (illustrative palette preview)</summary>

![Zed Light palette preview](screenshots/zed-light.svg)
</details>

<details>
<summary>Rosé Pine Moon (illustrative palette preview)</summary>

![Rosé Pine Moon palette preview](screenshots/rose-pine-moon.svg)
</details>

<details>
<summary>Catppuccin Mocha (illustrative palette preview)</summary>

![Catppuccin Mocha palette preview](screenshots/catppuccin-mocha.svg)
</details>

<details>
<summary>Tokyo Night Storm (illustrative palette preview)</summary>

![Tokyo Night Storm palette preview](screenshots/tokyo-night-storm.svg)
</details>

<details>
<summary>Nord Polar (illustrative palette preview)</summary>

![Nord Polar palette preview](screenshots/nord-polar.svg)
</details>

## More editor palette previews

The following previews are generated palette mockups, not captures from a running Symphony TUI.

<details>
<summary>Oxocarbon Dark (illustrative preview)</summary>

![Oxocarbon Dark palette preview](screenshots/oxocarbon-dark.svg)
</details>

<details>
<summary>Oxocarbon Light (illustrative preview)</summary>

![Oxocarbon Light palette preview](screenshots/oxocarbon-light.svg)
</details>

<details>
<summary>Everforest Dark (illustrative preview)</summary>

![Everforest Dark palette preview](screenshots/everforest-dark.svg)
</details>

<details>
<summary>Everforest Light (illustrative preview)</summary>

![Everforest Light palette preview](screenshots/everforest-light.svg)
</details>

<details>
<summary>Solarized Dark (illustrative preview)</summary>

![Solarized Dark palette preview](screenshots/solarized-dark.svg)
</details>

<details>
<summary>Solarized Light (illustrative preview)</summary>

![Solarized Light palette preview](screenshots/solarized-light.svg)
</details>

<details>
<summary>Ayu Mirage (illustrative preview)</summary>

![Ayu Mirage palette preview](screenshots/ayu-mirage.svg)
</details>

<details>
<summary>Ayu Light (illustrative preview)</summary>

![Ayu Light palette preview](screenshots/ayu-light.svg)
</details>

<details>
<summary>Flexoki Dark (illustrative preview)</summary>

![Flexoki Dark palette preview](screenshots/flexoki-dark.svg)
</details>

<details>
<summary>Flexoki Light (illustrative preview)</summary>

![Flexoki Light palette preview](screenshots/flexoki-light.svg)
</details>

## Contribute

Each family under `plugins/` has a `plugin.json` and a `themes/` directory. Add a uniquely named TOML with `name`, `base` (`dark` or `light`), and a `[colors]` table. Existing files show all supported tokens. Specify every token for predictable colors; missing tokens fall back to the selected base palette. Add new families to `.agents/plugins/marketplace.json`. Only theme data is read; CSS and executable code are not loaded from theme files.

Some Symphony widgets still use fixed colors, and transcript text already rendered before switching themes may keep its old colors. Contributions must be your own or include clear licensing and attribution.
